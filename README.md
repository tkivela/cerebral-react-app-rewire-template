# React template with Cerebral state management

Small React app template with everything you need.

**What's inside?**

* `react`
* `cerebral`
* `styled-components`

Setup is based on create-react-app but uses react-app-rewire for customization options.

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

Fix linting errors with
```
yarn lint-fix
```


## Styled-components

I've included react-app-rewire-styled-components which basically allows nicer experience debugging CSS styles created by Styled-components while preserving create-react-app functionality otherwise.
