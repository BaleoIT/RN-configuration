# React Native configuration

##### Dépendances

* Babel
* Babel presets
* ESLint
* ESLint presets
* AirBnB config

```
# shell command
yarn add eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react eslint-watch babel-core babel-eslint babel-preset-airbnb babel-preset-react-native babel-preset-react-native-stage-0 -D
```

##### Scripts

```
# package.json
"lint": "esw src/**",
"lint-watch": "esw -w --changed src/**",
"start-ios": "react-native run-ios && npm run lint-watch",
"start-ios-device": "react-native run-ios --device && npm run lint-watch",
"start-android": "react-native run-android && npm run lint-watch",
```

Pour installer l'application sur un device iOS sans passer par Xcode, il est nécessaire d'installer `ios-deploy` en global sur la machine :

```
# shell command
npm i -g ios-deploy
```

##### Fichiers de configuration

* [.eslintrc.json](.eslintrc.json)
* [.prettierrc.json](.prettierrc.json)
* [.babelrc.json](.babelrc.json)

##### Préférences VSCode

```
# settings.json
"editor.formatOnSave": true,
"files.trimTrailingWhitespace": true,
"eslint.packageManager": "yarn"
```

##### Extensions VSCode

[React Native - Full Pack](https://marketplace.visualstudio.com/items?itemName=kelset.rn-full-pack)
