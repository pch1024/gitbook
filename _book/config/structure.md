
# GitBook 目录结构如下
```
├── .gitignore  // 忽略文件
├── book.json   // 打包配置文件（可选，自建）
├── README.md   // 序言（必备）
├── SUMMARY.md  // 文件目录信息
├── GLOSSARY.md // 词汇表文件,出现该文件中的词汇，鼠标放到词汇上会给出词汇示意。（可选，自建）
├── LANGS.md/  // 多语言配置文件
├── others/*    // 根目录里除了 .ignored 都会拷贝到打包文档里
├── chapter-1/  // 大标题
|   ├── README.md
|   └── something.md
└── chapter-2/
    ├── README.md
    └── something.md
```

## Glossary 实例：
```
## Git
分散式版本控制软件

## Markdown
Aaron Swartz 跟John Gruber共同设计的排版语言
```

## Summary 实例：

```
* [Introduction](README.md)

* [article-1](chapter-1/article-1.md)
    * [article-2](chapter-1/article-2.md)

### Part II
* [article-3](chapter-2/article-3.md)
* [article-4](chapter-2/article-4.md)


### Part III
* [Part III](chapter-3/README.md)
    * [article-3](chapter-3/article.md)
```

### 多语言

gitbook支持多语言。每一种语言都应该按照正常的gitbook子目录和文件命名格式，LANGS.md 放在根目录下：

```
# Languages

* [English](en/)
* [中文](zh/)
```
