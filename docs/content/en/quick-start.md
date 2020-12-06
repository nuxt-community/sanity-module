---
title: Quick start
description: 'Access text, images, and other media with Nuxt and the Sanity headless CMS.'
category: Getting started
position: 2
---

## Setup

### Install Sanity integration

<code-group>
  <code-block label="Yarn" active>

```bash
yarn add @nuxtjs/sanity
```

  </code-block>
  <code-block label="NPM">

```bash
npm install @nuxtjs/sanity --save
```

  </code-block>

</code-group>

### Enable the module in your Nuxt configuration

<code-group>
  <code-block label="Nuxt 2.9+" active>

```js{}[nuxt.config.js]
{
  buildModules: ['@nuxtjs/sanity']
}
```

  </code-block>
  <code-block label="Nuxt < 2.9">

```js{}[nuxt.config.js]
{
  modules: ['@nuxtjs/sanity']
}
```

  </code-block>

</code-group>

### Add Sanity configuration

`@nuxtjs/sanity` will look for a `sanity.json` file in your project root directory. Just copy over the `sanity.json` from your CMS - and you're fully configured!

Alternatively, you can pass in an object in your Nuxt config with key details.

```js{}[nuxt.config.js]
{
  sanity: {
    projectId: 'myProject'
  }
}
```

<alert type="info">You can find more about configuring `@nuxtjs/sanity` [here](/configuration).</alert>

4. **You're good to go!**

   Check out [how to use Sanity](/usage).

## TypeScript

`@nuxtjs/sanity` offers type definitions. Just add an entry in `tsconfig.json`.

<code-group>
  <code-block label="Nuxt 2.9+" active>

```json{}[tsconfig.json]
{
  "compilerOptions": {
    "types": ["@nuxt/types", "@nuxtjs/sanity"]
  }
}
```

  </code-block>
  <code-block label="Nuxt < 2.9">

```json{}[tsconfig.json]
{
  "compilerOptions": {
    "types": ["@nuxt/vue-app", "@nuxtjs/sanity"]
  }
}
```

  </code-block>

</code-group>
