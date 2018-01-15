# React template with Cerebral state management

Small React app template with everything you need.

[![style: styled-components](https://img.shields.io/badge/style-%F0%9F%92%85%20styled--components-orange.svg?colorB=daa357&colorA=db748e)](https://github.com/styled-components/styled-components)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
[![tested with jest](https://img.shields.io/badge/tested_with-jest-99424f.svg)](https://github.com/facebook/jest)

**What's inside?**

* `react`
* `cerebral`
* `styled-components`

Setup is based on create-react-app (not ejected) and uses react-app-rewire for customization options.

## Getting started

Clone and install deps

```
git clone git@github.com:tkivela/cerebraltemplate.git
cd cerebraltemplate
yarn
yarn start
```

Then open `http://localhost:3000` and edit `./src/` -files and press save. Webpack 
will automagically hot reload you files whenever you make changes.

## Directory structure

Majority of code lives in src directory:

```
src/
├── components
├── index.js
└── modules
    └── app
        ├── actions
        ├── computes
        ├── index.js
        └── signals
```

* components: React components
* index.js: Root container component
* modules: Cerebral modules, one example module called app included
* modules/app/index.js: App initial state & signals 
* modules/app/actions: Cerebral actions
* modules/app/computes: Cerebral computes which calculate derived state entries
* modules/app/signals: Cerebral signals

## Building for Production

```
yarn build
```

This will compile your JS and copy your assets to the `build` folder which
you can deploy wherever as a webpage.

## Testing

```
yarn test
```

Running tests runs Javascript Standard Style (https://standardjs.com/) linting rules before running unit tests with Jest.
I've included example tests for Cerebral signals and computes.

## Linting
Check for linting errors with
```
yarn lint
```

Fix linting errors (& format code with prettier-standard) with
```
yarn lint-fix
```


## Styled-components

I've included react-app-rewire-styled-components which basically allows nicer experience debugging CSS styles created by Styled-components while preserving create-react-app functionality otherwise.
