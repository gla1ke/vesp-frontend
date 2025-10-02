# Vesp Frontend (Personal Fork)

> **Note:** This is a personal optimized fork of the original [Vesp Frontend](https://github.com/bezumkin/vesp-frontend) by bezumkin. This version is tailored for personal use with optimizations and customizations.

This library add default modules, plugins and settings to your **Nuxt 3** project to make it easier to start.

## Dependencies
- [Bootstrap Vue Next](https://github.com/bootstrap-vue-next/bootstrap-vue-next) as a main components library
- [Nuxt i18n](https://i18n.nuxtjs.org) for internalization
- [Fontawesome Icons](https://fontawesome.com/) famous icons (only solid pack)
- [Vue Toastification](https://github.com/Maronato/vue-toastification) for displaying handy popup messages
- [Date-Fns](https://date-fns.org/) modern JavaScript date utility library
- [Vue Pinia](https://pinia.vuejs.org/) for central data storage
- [Eslint](https://eslint.org) and [Prettier](https://prettier.io) to add rules for your code style

## Quick Start

1. Create a [new Nuxt 3 project](https://nuxt.com/docs/getting-started/installation)

2. Then add the dependency:
```npm
yarn add @gla1ke/vesp-frontend
```
or
```npm
npm i @gla1ke/vesp-frontend --save
```

3. Add `@gla1ke/vesp-frontend` module into your nuxt.config.ts modules
```js
export default defineNuxtConfig({
  css: ['~/assets/scss/index.scss'],
  // ...
  modules: ['@gla1ke/vesp-frontend'],
  vesp: {
    icons: {
      solid: ['faUser', 'faPowerOff', 'faRightToBracket'],
    },
  },
})
```

4. Add SCSS and CSS assets into your root style file
```scss
// ~/assets/scss/index.scss
@import 'bootstrap-scss/bootstrap';
@import '@gla1ke/vesp-frontend/assets/components';
@import '@gla1ke/vesp-frontend/assets/toast';
@import '@fortawesome/fontawesome-svg-core/styles.css';
```

5. Now you can use Vesp components in your Nuxt project

## Components
@TODO add more detailed description of components

### Vesp-Table
This component extends BootstrapVue's `b-table` component and add a lot of features, including row actions and filters. 

### Vesp-Modal
This component extends BootstrapVue's `b-modal` component and add ability to submit forms.

### Vesp-Change-Locale
Simple component to change the current locale of project. 
You can use `#default` slot to change how it looks.

### Vesp-Input-Remote-Links
Component for adding a list of links in JSON object, where key will be the name of service and value is a link to it.
Very useful for submitting a list of social networks for user.

### Vesp-Input-Combo-Box
`b-form-input` with popup list containing variants from remote API.

### Vesp-Input-Date-Picker
`vue-datepicker-next` with some settings

## Examples

This module is used in [main Vesp package](https://github.com/bezumkin/vesp), please follow the link for examples.

## Fork Optimizations

This personal fork includes the following optimizations and customizations:

- **Personalized Configuration**: Tailored default settings for personal use cases
- **Repository Ownership**: Updated to reflect fork ownership by gla1ke
- **Custom Enhancements**: Additional optimizations for specific workflows

For the original project, see [bezumkin/vesp-frontend](https://github.com/bezumkin/vesp-frontend).