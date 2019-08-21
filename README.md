## Create React Native App Typescript

### Steps

- configure enviroment
  - https://docs.rocketseat.dev/ambiente-react-native/android/windows
- `yarn global add react-native-cli (if not installed)`
- `react-native init coolName --template typescript`
- install essential depedencies
  - `yarn add eslint-config-airbnb eslint-config-prettier eslint-config-react-app eslint-config-react-native eslint-import-resolver-typescript eslint-plugin-flowtype eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-prettier eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-react-native @typescript-eslint/parser @typescript-eslint/eslint-plugin prettier -D`
- .eslintrc.js
  ```javascript
  module.exports = {
    env: {
      browser: true,
      es6: true,
      jest: true
    },
    root: true,
    extends: [
      "react-native",
      "airbnb",
      "plugin:@typescript-eslint/recommended",
      "prettier/@typescript-eslint"
    ],
    globals: {
      Atomics: "readonly",
      SharedArrayBuffer: "readonly"
    },
    parserOptions: {
      ecmaFeatures: {
        jsx: true
      },
      ecmaVersion: 2018,
      sourceType: "module"
    },
    plugins: ["react-native", "react", "import", "jsx-a11y"],
    rules: {
      "react/jsx-filename-extension": [
        "error",
        {
          extensions: [".tsx"]
        }
      ],
      "import/prefer-default-export": "off",
      "@typescript-eslint/explicit-function-return-type": "off",
      "@typescript-eslint/explicit-member-accessibility": "off",
      "@typescript-eslint/interface-name-prefix": 0,
      "react/destructuring-assignment": 0,
      "@typescript-eslint/no-non-null-assertion": 0,
      "@typescript-eslint/no-explicit-any": 0,
      "@typescript-eslint/no-empty-interface": 0,
      "no-underscore-dangle": 0,
      "react/no-access-state-in-setstate": 0,
      "spaced-comment": 0,
      "react-native/no-inline-styles": 0,
      "react-native/no-color-literals": 0,
      "no-console": 0,
      "object-curly-newline": 0,
      "max-len": 0
    },
    settings: {
      "import/parsers": {
        "@typescript-eslint/parser": [".ts", ".tsx"]
      },
      "import/resolver": {
        typescript: {}
      }
    }
  };
  ```
- install navigation depedencies
  - `yarn add react-navigation react-native-gesture-handler react-native-reanimated`
  - `yarn add @types/react-navigation -D`
  - if android update the manifest by following these steps https://kmagiera.github.io/react-native-gesture-handler/docs/getting-started.html
- install axios (if nescessary)
  - `yarn add axios`
  - `yarn add @types/axios`
- install socket.io-client (if nescessary)
  - `yarn add axios`
  - `yarn add @types/axios`
- install socket.io-client (if nescessary),
  - `yarn add socket.io-client`
  - `yarn add @types/socket.io-client`
- `react-native run-android`
- `yarn start`
