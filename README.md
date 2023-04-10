# vue-example

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### 解決eslint prettier 格式化衝突
npm install --save-dev eslint-config-0
npm install --save-dev eslint-plugin-prettier
in .eslintrc.js
```js
{
  ...
  extends: [
    ...
    "plugin:prettier/recommended",
  ],
}
```