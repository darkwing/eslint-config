# `@metamask/eslint-config-nodejs`

MetaMask's [Node.js](https://nodejs.org) ESLint configuration.

## Usage

```bash
yarn add --dev \
    eslint@^7.7.0 \
    eslint-plugin-import@^2.22.0 \
    eslint-plugin-node@^11.1.0 \
    @metamask/eslint-config@^5.0.0 \
    @metamask/eslint-config-nodejs@^5.0.0
```

```js
module.exports = {
  extends: [
    '@metamask/eslint-config',
    '@metamask/eslint-config-nodejs',
  ],
}
```

To lint the `.eslintrc.js` file itself, you will **need** to add this config in addition to the base config.
