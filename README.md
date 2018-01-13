# 

# Features
**Quick scaffolding**

Create components, connected components, modules - and their tests - right from the CLI!

**Instant feedback**

Enjoy the best DX (Developer eXperience) and code your app at the speed of thought!
Your saved changes to the CSS and TypeScript are reflected instantaneously without refreshing the page.
Preserve application state even when you update something in the underlying code!

**SEO** (with [vue-meta](https://github.com/declandewet/vue-meta))

We support SEO (document head tags management) and server-side-rendering for search engines
that support indexing of JavaScript content. (eg. Google)

**Progressive-Web-App**

Offline-first support with service-workers and a lighthouse score as high as possible (for me - 90+).

**Enterprise ready**

Common style guide, TypeScript and the best test setup: Automatically guarantee code quality and non-breaking changes.

**Animations** (with [anime.js](http://animejs.com/))

A stable animations set up already included.

**Components**

A flexible component library that'll be extended over time.


**Industry-standard i18n internationalization support**

Scalable apps need to support multiple languages, easily add and support multiple languages with [vue-i18n](https://github.com/kazupon/vue-i18n).

**Predictable state management** 

With [vuex](https://github.com/vuejs/vuex).

**Routing with data prefetching**

Server-side-rendering of prefetched data and transferring state from server to client.

# Quick start

1. Install Node.js 8.7.x or higher. Use [nvm](https://github.com/creationix/nvm) to maintain multiple Node.js versions
2. Install npm version 5.4.x or higher
3. clone repository `git clone https://github.com/devCrossNet/vue-starter`
4. Install dependencies: `npm install`
5. Run `npm run dev`. The server runs on port `3000` by default, set `PORT` environment variable to configure a different port

# Documentation (WIP)

### Run unit tests
- `npm test` runs tests once
- `npm run test:coverage` runs tests with coverage once

Find a detailed coverage report in `coverage/iconv-report/index.html`

### Run e2e tests

For more information about the e2e test set up, have a look at [cypress.io](https://www.cypress.io/).

- run `npm run dev`
- open a second terminal window
- run `npm run e2e`

### Generators
This boilerplate comes with the possibility to generate modules, components and connected components
to keep a common style guide and to make development faster.

To generate code just run `npm run generate` or `npm run g` and follow the instructions.

### i18n and extracting messages

To extract all your i18n IDs run `npm run extract-i18n-messages`.
This will generate the languages files in the folder `./i18n`,
to add new language files add a new entry to `package.json -> config."supported-languages"`.

This script also enables you to define default messages with a magic comment:

`$t('App.nav.components' /*Components*/)`,
this will add `'Components'` as default value to all `'App.nav.components'` keys, 
but will keep previously added values.

## Release
To release a new version of your project run one of the following commands:

- `npm run release:major`
- `npm run release:minor`
- `npm run release:patch`

This will also automatically generate a change log.
