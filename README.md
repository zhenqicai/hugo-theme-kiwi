[Chinese](https://github.com/zhenqicai/hugo-theme-kiwi/blob/main/README_zh.md) | [English](#)

<a title="Hugo kiwi site" href="https://qiucode.cn">
   <img align="right" alt="NexT logo" width="266" src="https://qiucode.cn/static/front/images/qiu-logo.png">
</a>

## Hugo kiwi

«Hugo kiwi» is a fresh and not tacky [Hugo](https://gohugo.io) theme. Its design concept is derived from [Qiucode Record](https://qiucode.cn) (when not used Deployed with ```Hugo```, that is to say, the version built using cloud servers and self-built server programs). Of course, I personally prefer to display the homepage list with pictures and text.

## 👀 Online preview

[Qiucode Record](https://qiucode.cn) This theme is used now.


## 👣 Quick Start

Before using the `Hugo kiwi` theme, please make sure that `Git` and `Hugo Extended` are installed on your computer.


### 📐 Direct quote

If you already have a site, you can reference this topic through `submodule` mode, refer to the following command:

```shell
$ cd hugo-kiwi-exmaple
$ git submodule add https://github.com/zhenqicai/hugo-theme-kiwi.git themes/hugo-theme-kiwi
$ cp themes/hugo-theme-kiwi/exampleSite/config.yaml .
$ mv config.toml config.toml.backup
```

### 💻 Local preview

```shell
$ cd hugo-kiwi-exmaple
$ hugo server
```

Open the browser and enter http://127.0.0.1:1313/ in the address bar to check the theme effect. I wish you good luck! :tada::tada::tada:

> **Note**
> Please note that the `hugo server` command is only used for local development or preview when writing articles, and is not intended to directly open access to the external network. When officially released, you can use the `hugo` command to generate static files for the whole site, and then deploy them to a web server like `Nginx`.

### 🔄 Theme update

To subsequently update the theme, you only need to execute the following command in your site directory:

```shell
$ cd hugo-kiwi-exmaple
$ git submodule update --remote
```

## 📝 Post a new article

The theme has been configured with a default article template. It is recommended to use the following Hugo command to quickly create new articles:

```sh
$ hugo new posts/hello-world.md
```

> **Note**
> The `posts` path is a subfolder under the root directory of `content`, which can be adjusted according to your own file management form.

For an explanation of the functions of the parameters at the head of the article, please refer to the following:


```yml
---
# Article title
title: "{{ replace .Name "-" " " | title }}"
# Summary of article content
description: "{{ .Name }}"

# Publication date
date: {{ .Date }}
# Last modified date
lastmod: {{ .Date }}
# Classification
categories:
  -
# Label
tags:
  -

#Whether comments are enabled for the article
comment:
   enable: true
#Address for external access
url: article/175
# Whether to display the directory
toc: true

# Article cover image related attributes
cover:
    image: "" #Image path example: posts/tech/123/123.png
    zoom: 50% # Image size, for example, filling in 50% means half the size of the original image
    caption: "" #Description at the bottom of the picture
    alt: ""
    relative: false


---


```

## 🎉User Case

- [Qiucode Record](https://qiucode.cn)

If you are also using the `Hugo kiwi` theme, please submit it at the bottom of the [flinks.yaml](https://github.com/hugo-next/hugo-next-docs/blob/develop/data/flinks.yaml) file The name, description, avatar, link and other information of your site. The specific format content is as follows:

```yaml
 - name: Autumn code record
   desc: A Java enthusiast who lives in the mountains
   avatar: https://qiucode.cn/static/front/images/qiu-logo.png
   link: https://qiucode.cn
```

## 🙋 Usage feedback

- Join [GitHub Discussions](https://github.com/zhenqicai/hugo-theme-kiwi/discussions) or [Gitter](https://github.com/zhenqicai/community) online discussions :beers:
- [GitHub Issues](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Bug&template=bug-report.md) Submit a bug report :bug:
- [GitHub Feature](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Feature+Request&template=feature-request.md) expresses ideas for new features :sparkles:

> Of course, you can also join the ```QQ group```: 616127224 for discussion.
​