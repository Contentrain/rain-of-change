---
ID: "39e99355-bba0-4518-96de-59a968e2707c"
slug: "readme"
relaseDate: "2022-04-26 12:00"
publish: true
createdAt: 1654690525019
tags:
  - ID: "508dc3fa-59e8-4e29-8163-78e3916c151e"
    text: "readme"
    color: "red"
    createdAt: 1654690608465
updatedAt: 1654770701146

---

[![Change Of Rain](https://github.com/Contentrain/rain-of-change/blob/main/static/cover.png?raw=true)](https://change-log-red.vercel.app/)

# Rain of Change
A free Changelog template created with [Nuxt 3.0](https://nuxtjs.org) & [Nuxt Content 2.0](https://content.nuxtjs.org) that you can use for your projects.

## Headless CMS
[![Use with Contentrain](https://imagedelivery.net/yx26LyQGM_miwnGU8RnEaw/721c176e-f4b1-4495-1d6c-87a4b9ffa100/public)](https://app.contentrain.io)

Contentrain'de bu template için tüm entegrasyonu tamamlanmış koleksiyonları oluşturduk. Dilersen Contentrain'e ücretsiz olarak kayıt olarak Github repona aldığın template'ine bağlanabilir ve Shared Collections bölünümden Logs koleksiyonunu seçerek kullanabilirsin.
Bu sayede tüm loglarını Contentrain ile kolayca yönetebilirsin.
Contentrain ile bu template'in kullanımına ilişkin videoyu çok yakında paylaşacağız.

## Frontmatter
#### Default
|variable|description|options|
|-|-|-|
|publish|İçeriğinin yayınlanması için kontrol sağlar.| true or false|
|relaseDate|Logların için tarih belirlemeni sağlar| -|
|tags|Sürüm etiketini ve etiket renklerini belirlemeni sağlar. | -|

#### Tag Object
|variable|description|options|
|-|-|-|
|text| "Features, Bug Fix" gibi sürüm etiketleri oluşturabilirsiniz| -|
|color| Etiket için renk seçebilirsin | blue,red, yellow, gray, zinc, green, purple, orange, pink, teal, indigo, cyan, brown, slate, amber, lime, emerald, sky |

## Setup

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Deployment

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Contentrain/rain-of-change) [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Contentrain/rain-of-change)


### Static Hosting

Pre-render the website to be deployed on any static hosting:

```bash
npm run generate
```

The `dist/` directory is ready to be deployed (symlink to `.output/public`), [learn more on Nuxt docs](https://v3.nuxtjs.org/guide/deploy/static-hosting).

### Node server

Build the application for production:

```bash
npm run build
```

Start the server in production:

```bash
node .output/server/index.mjs
```

Learn more on [Nuxt docs](https://v3.nuxtjs.org/guide/deploy/node-server) for more information.