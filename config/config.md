记录Gitbook的一些配置信息

> GitBook 提供了三类文档主题： Book 文档、API文档、FAQ文档。我们常用的就是 Book 文档模式，如果我们需要使用 API 文档模式或者 FAQ 文档模式，需引入文档对应的主题插件。

```
{
    "title": "标题",
    "description": "书本描述",
    "author": "作者信息",
    "output.name": "site",
    "language": "使用的语言",
    "gitbook": "指定gitbook版本 '>=3.2.3' ",
    "root": "指定存放 GitBook 文件的根目录 '.' ",
    "structure": { // 设置 Readme, Summary, Glossary等对应的文件
        "readme": "introduction.md"
    },
    "links": { // 在侧边栏添加链接
        "sidebar": {
            "Blog": "http://www.peichenhu.cn",
            "GitHub": "http://www.peichenhu.cn",
            "repository": "http://www.peichenhu.cn",
        }
    },
    "plugins": [  //提前配置 gitbook install 安装，插件地址https://plugins.gitbook.com/
        "-lunr", // 去除默认加载插件加前缀“-”
        "chart" // 添加插件
    ],

    "pluginsConfig": { // 插件配置
        "theme-default": {
            "showLevel": true // true 显示标题前面的数字索引，默认不显示。
        }
       }
    }
}

```

插件网址：[https://plugins.gitbook.com/](https://plugins.gitbook.com/)
常用插件
```
theme-faq FAQ文档
theme-api API文档
Disqus - Disqus 评论
Search Plus - 支持中文搜索
Prsim - 使用 Prism.js 高亮代码
Advanced Emoji - 支持 emoji 表情
Github - 添加github图标
Github Buttons - 添加项目在 Github 上的 star、fork、watch 信息
Ace Plugin - 支持ace
Emphasize - 为文字加上底色
KaTex - 支持数学公式
Include Codeblock - 用代码块显示包含文件的内容
Splitter - 使侧边栏的宽度可以自由调节
Mermaid-gb3 - 支持渲染 Mermaid 图表
Puml - 支持渲染 uml 图
Graph - 使用 function-plot 绘制数学函数图
Chart - 绘制图形
Sharing-plus - 分享当前页面
Tbfed-pagefooter - 为页面添加页脚
Expandable-chapters-small - 使左侧的章节目录可以折叠
Sectionx - 将页面分块显示
GA - Google 统计
3-ba - 百度统计
Donate - 打赏插件
Local Video - 使用 Video.js 播放本地视频
Simple-page-toc - 自动生成本页的目录结构
Anchors - 添加 Github 风格的锚点
Anchor-navigation-ex - 添加Toc到侧边悬浮导航以及回到顶部按钮
Edit Link - 链接到当前页源文件上
Sitemap-general - 生成sitemap
Favicon - 更改网站的 favicon.ico
Todo - 添加 Todo 功能
Terminal - 模拟终端样式
Copy-code-button - 为代码块添加复制按钮
Alerts - 添加不同 alerts 样式的 blockquotes
Include-csv - 显示 csv 文件内容
Musicxml - 支持 musicxml 格式的乐谱渲染
Klipse - 集成 Kplise (online code evaluator)
Versions-select - 添加版本选择的下拉菜单
Rss - 添加 rss 订阅功能
```