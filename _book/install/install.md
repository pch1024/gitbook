
# 安装Gitbook

## 本地安装

### 环境和依赖
* NodeJS (v4.0.0 and above is recommended)
* Windows, Linux, Unix, or Mac OS X

### 使用 NPM 安装

```
$ npm uninstall gitbook gitbook-cli -g // 卸载旧版
$ npm install gitbook-cli gitbook -g // 安装新版（2018年4月6日03:34:49）
$ gitbook -V
  CLI version: 2.3.2
  GitBook version: 3.2.3  
```
### 测试

初始化项目文档

```
$ gitbook init ./directory // 创建文件并初始化项目
$ cd directory
```

初始化完成后，直接使用 `serve` 命令创建网页版书进行本地预览

```
$ gitbook serve  // 项目运行在  http://localhost:4000
```

至此，不出意外项目基本跑通。回顾扩展常用命令：

```
gitbook init ./directory // 创建文件并初始化项目
gitbook install 目录  (安装gitbook需要的插件)
gitbook serve 文件目录 生成目录 (启用gitbook 可以在 http://localhost:4000/ 访问)
gitbook build 文件目录 生成目录 (生成站点)
gitbook pdf 文件目录 生成目录 (生成pdf)

gitbook help //列出gitbook所有的命令
gitbook --help //输出gitbook-cli的帮助信息

gitbook ls //列出本地所有的gitbook版本
gitbook ls-remote //列出远程可用的gitbook版本
gitbook fetch 标签/版本号 //安装对应的gitbook版本
gitbook update //更新到gitbook的最新版本
gitbook uninstall 2.0.1 //卸载对应的gitbook版本

gitbook build --gitbook=2.0.1 //生成时指定gitbook的版本, 本地没有会先下载
gitbook build --log=debug //指定log的级别
gitbook builid --debug //输出错误信息
```