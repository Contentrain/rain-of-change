
[![Change Of Rain](https://imagedelivery.net/yx26LyQGM_miwnGU8RnEaw/161e2520-980c-4c92-c953-a7080a77a800/public)](https://change-log-red.vercel.app/)

# Rain of Change [![Netlify Status](https://api.netlify.com/api/v1/badges/86ca144b-95be-4813-ae57-5d1ef8f23856/deploy-status)](https://app.netlify.com/sites/delicate-empanada-f78c32/deploys)
A free Changelog template created with [**Nuxt 3.0**](https://nuxtjs.org) & [**Nuxt Content 2.0**](https://content.nuxtjs.org) that you can use for your projects.

We are very pleased to share our first free template. We hope Rain of Change will help anyone who needs to keep a Changelog for their projects.

You can customize this template as you wish by copying it to your own repository and pulling it to your local.


## Headless CMS
[![Use with Contentrain](https://imagedelivery.net/yx26LyQGM_miwnGU8RnEaw/721c176e-f4b1-4495-1d6c-87a4b9ffa100/public)](https://app.contentrain.io)


To manage the content of this template, we recommend you use [**Contentrain**](Contentrain).

We have created the collection template that you need. You can find and use this collection in “Shared Collections”.

After free registration with [Contentrain](**Contentrain**), you need to start a manual project installation and continue the installation by selecting the Rain of Change repo on Github.

During the installation, it is enough to delete the sample collections in the Collections step, select the Logs collection from the Shared Collections section and complete the installation.

This way you can easily manage all your logs with Contentrain.

If you have any question with the installation, you can send us your questions via [Discord](**Discord**).

We will soon publish a video about how to use this template with Contentrain.


## Frontmatter
#### Default
|variable|description|options|
|-|-|-|
|publish|It provides publication control for your logs| true or false|
|relaseDate|Allows you to set dates for your logs| -|
|tags|Allows you to set the version label and label colors. | -|

#### Tag Object
|variable|description|options|
|-|-|-|
|text| You can create release tags like "Features, Bug Fix"| -|
|color| You can choose the color for the tags | blue,red, yellow, gray, zinc, green, purple, orange, pink, teal, indigo, cyan, brown, slate, amber, lime, emerald, sky |

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
