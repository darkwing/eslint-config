# `@metamask/eslint-config-typescript`

MetaMask's [TypeScript](https://www.typescriptlang.org) ESLint configuration.

## Usage

```bash
yarn add --dev \
    eslint@^7.7.0 \
    eslint-plugin-import@^2.22.0 \
    @typescript-eslint/eslint-plugin@^3.9.1 \
    @typescript-eslint/parser@^3.9.1 \
    @metamask/eslint-config@^5.0.0 \
    @metamask/eslint-config-typescript@^5.0.0
```

```js
module.exports = {
  root: true,

  extends: [
    '@metamask/eslint-config',
  ],

  overrides: [
    // The TypeScript config disables certain rules that you want to keep for
    // .js files, so it should be added in an override.
    {
      files: ['*.ts'],
      extends: [
        '@metamask/eslint-config-typescript',
      ],
    },
  ],
};
```
