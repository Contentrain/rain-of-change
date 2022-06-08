
[![Change Of Rain](https://github.com/Contentrain/rain-of-change/blob/main/static/cover.png?raw=true)](https://change-log-red.vercel.app/)

# Rain of Change
A free Changelog template created with [Nuxt 3.0](https://nuxtjs.org) & [Nuxt Content 2.0](https://content.nuxtjs.org) that you can use for your projects.

## Contentrain

- Create pages in Markdown in the `content/` directory
- Generated navigation based on your pages
- Create Vue components and use them in your Markdown
- Deploy on any Node or Static hosting: GH Pages, Vercel, Netlify, Heroku, etc.

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
