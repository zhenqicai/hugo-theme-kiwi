[中文](#) | [English](https://github.com/zhenqicai/hugo-theme-kiwi/blob/main/README.md)

<a title="Hugo kiwi 站点" href="https://qiucode.cn">
  <img align="right" alt="NexT logo" width="266" src="https://qiucode.cn/static/front/images/qiu-logo.png">
</a>

## Hugo kiwi

«Hugo kiwi» 是一款清新并不俗气的 [Hugo](https://gohugo.io) 主题，它的设计理念源于 [秋码记录](https://qiucode.cn) （在没有使用 ```Hugo``` 来部署的，也就是说使用云服务器和自建服务端程序所构建出来的那个版本），当然咯，我本人还是比较喜欢首页列表以图文来展示。

## 👀 在线预览

[秋码记录](https://qiucode.cn) 现在便是使用该主题。


## 👣 快速开始

在使用 `Hugo kiwi` 主题之前，请确认您的电脑上已经安装 `Git` 和 `Hugo Extened` 两款软件。


### 📐 直接引用

如果您已经有站点，可通过 `submodule` 模式引用本主题，参考如下命令：

```shell
$ cd hugo-kiwi-exmaple
$ git submodule add https://github.com/zhenqicai/hugo-theme-kiwi.git themes/hugo-theme-kiwi
$ cp themes/hugo-theme-kiwi/exampleSite/config.yaml .
$ mv config.toml config.toml.backup
```

### 💻 本地预览

```shell
$ cd hugo-kiwi-exmaple
$ hugo server
```

打开浏览器，在地址栏输入 http://127.0.0.1:1313/ 查看主题效果，祝你好运！:tada::tada::tada:

> **Note**
> 要注意下 `hugo server` 命令只是用于本地开发或写文章时预览，并非是将其直接对外网开放访问。在正式发布时，可通过 `hugo` 命令生成全站静态文件，然后部署到类似 `Nginx` 的 Web 服务器即可。

### 🔄 主题更新

后续更新主题只需要在您的站点目录中，执行如下命令：

```shell
$ cd hugo-kiwi-exmaple
$ git submodule update --remote
```

## 📝 发表新文章

主题已经配置了默认的文章模板，建议使用如下 Hugo 命令快速创建新的文章：

```sh
$ hugo new posts/hello-world.md
```

> **Note**
> 其中 `posts` 路径是 `content` 根目录下的子文件夹，可依据自己的文件管理形态调整。

关于文章头部那些参数作用的说明参考如下：


```yml
---
# 文章标题
title: "{{ replace .Name "-" " " | title }}"
# 文章内容摘要
description: "{{ .Name }}"

# 发表日期
date: {{ .Date }}
# 最后修改日期
lastmod: {{ .Date }}
# 分类
categories:
 - 
# 标签
tags:
 - 

#文章是否开启评论
comment:
  enable: true
# 用于对外访问的地址
url: article/175
# 是否显示目录
toc: true

# 文章封面图片相关属性
cover:
   image: "" #图片路径例如：posts/tech/123/123.png
   zoom: 50% # 图片大小，例如填写 50% 表示原图像的一半大小
   caption: "" #图片底部描述
   alt: ""
   relative: false


---


```

## 🎉 用户案例

- [秋码记录](https://qiucode.cn)

如您也正在使用 `Hugo kiwi` 主题，欢迎在 [flinks.yaml]((https://github.com/zhenqicai/hugo-theme-kiwi/tree/main/exampleSite/data/flinks.yaml)  文件底部提交贵站的名称、描述、头像、链接等信息，具体格式内容参考如下：

```yaml
- name: 秋码记录
  desc: 一个游离于山间之上的Java爱好者
  avatar: https://qiucode.cn/static/front/images/qiu-logo.png
  link: https://qiucode.cn
```

## 🙋 使用反馈

- 加入 [GitHub Discussions](https://github.com/zhenqicai/hugo-theme-kiwi/discussions) 或 [Gitter](https://github.com/zhenqicai/hugo-theme-kiwi/community) 在线讨论 :beers:
- [GitHub Issues](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Bug&template=bug-report.md) 提交错误报告 :bug:
- [GitHub Feature](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Feature+Request&template=feature-request.md) 表新功能的想法 :sparkles:

> 当然，也可以加入```QQ群```：616127224 进行讨论。
