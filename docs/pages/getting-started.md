# __BRAND_NAME__ Library - Quickstart

Get started with __BRAND_NAME__ by including it into your project using NPM

__BRAND_NAME__ is a library of components built on top of the utility-classes from Tailwind CSS.

## Require via NPM

Make sure that you have [Node.js](https://nodejs.org/en/) and [Tailwind CSS](https://tailwindcss.com/) installed.

1. Install `@__GITHUB_USERNAME__/__PACKAGE_NAME__` as a dependency using NPM by running the following command:

```bash
npm i @__GITHUB_USERNAME__/__PACKAGE_NAME__
```

2. Add  @datadayrepos/__PACKAGE_NAME__ dist folder to tailwind content:

```javascript
module.exports = {
  content: [
    'node_modules/@__GITHUB_USERNAME__/__PACKAGE_NAME__/**/*.{js,mjs,cjs,jsx,ts,tsx,vue}',
  ],
  plugins: [
  ],
  theme: {}
}
```

3. Import __BRAND_NAME__ Vue styles:
```javascript
// in your `main.js` file
// eslint-disable-next-line antfu/no-import-node-modules-by-path, antfu/no-import-dist
import '../node_modules/@__GITHUB_USERNAME__/__PACKAGE_NAME__/dist/index.css' // only is using JS components
```
```css
/* or in your `app.css` file */
@import '/node_modules/@__GITHUB_USERNAME__/__PACKAGE_NAME__/dist/index.css';
```

4. Now you can use `@__GITHUB_USERNAME__/__PACKAGE_NAME__` anywhere in your project and build awesome interfaces:
```vue
<template>
  <CoolComponent text="Click me" placement="top">
  </CoolComponent>
</template>

<script setup>
import { CoolComponent } from '@__GITHUB_USERNAME__/__PACKAGE_NAME__'
</script>
```

> Make sure you have tailwind css imported. https://tailwindcss.com/docs/guides/vite

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
