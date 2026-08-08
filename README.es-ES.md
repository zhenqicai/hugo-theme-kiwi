

[Chinese](https://github.com/zhenqicai/hugo-theme-kiwi/blob/main/README_zh.md) | [English](#)

<a title="Hugo kiwi site" href="https://qiucode.cn">
   <img align="right" alt="NexT logo" width="266" src="https://qiucode.cn/static/front/images/qiu-logo.png">
</a>

## Hugo kiwi

«Hugo kiwi» es un tema de [Hugo](https://gohugo.io) fresco y elegante. Su concepto de diseño se deriva de [Qiucode Record](https://qiucode.cn) (cuando no se despliega usando `Hugo`, es decir, la versión construida con servidores en la nube y programas de servidor autoconstruidos). Por supuesto, personalmente prefiero mostrar la lista de la página de inicio con imágenes y texto.

## 👀 Vista previa en línea

[Qiucode Record](https://qiucode.cn) Este tema se está utilizando actualmente.

## 👣 Inicio rápido

Antes de utilizar el tema `Hugo kiwi`, asegúrate de que `Git` y `Hugo Extended` estén instalados en tu equipo.

### 📐 Referencia directa

Si ya tienes un sitio web, puedes referenciar este tema mediante el modo `submodule`, consulta el siguiente comando:

```shell
$ cd hugo-kiwi-exmaple
$ git submodule add https://github.com/zhenqicai/hugo-theme-kiwi.git themes/hugo-theme-kiwi
$ cp themes/hugo-theme-kiwi/exampleSite/config.yaml .
$ mv config.toml config.toml.backup
```

### 💻 Vista previa local

```shell
$ cd hugo-kiwi-exmaple
$ hugo server
```

Abre el navegador e introduce http://127.0.0.1:1313/ en la barra de direcciones para verificar el efecto del tema. ¡Te deseo mucha suerte! :tada::tada::tada:

> **Nota**
> Ten en cuenta que el comando `hugo server` solo se utiliza para el desarrollo local o la vista previa al escribir artículos, y no está destinado a abrir directamente el acceso a la red externa. Cuando se lance oficialmente, puedes usar el comando `hugo` para generar los archivos estáticos de todo el sitio y, a continuación, implementarlos en un servidor web como `Nginx`.

### 🔄 Actualización del tema

Para actualizar el tema posteriormente, solo necesitas ejecutar el siguiente comando en el directorio de tu sitio:

```shell
$ cd hugo-kiwi-exmaple
$ git submodule update --remote
```

## 📝 Publicar un nuevo artículo

El tema tiene configurada una plantilla de artículo predeterminada. Se recomienda usar el siguiente comando de Hugo para crear nuevos artículos rápidamente:

```sh
$ hugo new posts/hello-world.md
```

> **Nota**
> La ruta `posts` es una subcarpeta bajo el directorio raíz de `content`, la cual puede ajustarse según tu propia estructura de gestión de archivos.

Para una explicación de las funciones de los parámetros en la cabecera del artículo, consulta lo siguiente:

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

## 🎉 Casos de uso

- [Qiucode Record](https://qiucode.cn)

Si también estás utilizando el tema `Hugo kiwi`, envía el nombre, descripción, avatar, enlace y otra información de tu sitio en la parte inferior del archivo [flinks.yaml](https://github.com/hugo-next/hugo-next-docs/blob/develop/data/flinks.yaml). El contenido del formato específico es el siguiente:

```yaml
 - name: Autumn code record
   desc: A Java enthusiast who lives in the mountains
   avatar: https://qiucode.cn/static/front/images/qiu-logo.png
   link: https://qiucode.cn
```

## 🙋 ComentariosComentarios y retroalimentación

- Únete a las discusiones en línea de [GitHub Discussions](https://github.com/zhenqicai/hugo-theme-kiwi/discussions) o [Gitter](https://github.com/zhenqicai/community) :beers:
- [GitHub Issues](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Bug&template=bug-report.md) para enviar un informe de error :bug:
- [GitHub Feature](https://github.com/zhenqicai/hugo-theme-kiwi/issues/new?labels=Feature+Request&template=feature-request.md) para expresar ideas para nuevas características :sparkles:

> Por supuesto, también puedes unirte al ```grupo QQ```: 616127224 para discutir.
