# husky commitzen lab

A repo built for trying workflows using husky and commitzen

## 🦾 Install commitlint

```cmd
yarn add --dev @commitlint/cli @commitlint/config-angular cz-conventional-changelog
```

## 📃 Add commitlint.config.js
```js
module.exports = {
    extends: ['@commitlint/config-angular']
};
```

## 🐶 Install husky

```cmd
yarn add --dev husky
yarn husky init
```

## ⚡️ package.json

```json
"scripts": {
    "commit": "git-cz",
    "prepare": "husky install",
    "test": "commitlint --edit"
  },
```

## ⚙️ husky config
> .husky/pre-commit
```bash
yarn test
```
