## Create React Native App Typescript

### Steps

- configure enviroment
  - https://docs.rocketseat.dev/ambiente-react-native/android/windows
- yarn global add react-native-cli (if not installed)
- react-native init coolName --template typescript
- install essential depedencies
  - yarn add eslint-config-airbnb eslint-config-prettier eslint-config-react-app eslint-config-react-native eslint-import-resolver-typescript eslint-plugin-flowtype eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-prettier eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-react-native @typescript-eslint/parser @typescript-eslint/eslint-plugin prettier -D
- install navigation depedencies
  - yarn add react-navigation react-native-gesture-handler react-native-reanimated
  - yarn add @types/react-navigation -D
  - if android update the manifest by following these steps https://kmagiera.github.io/react-native-gesture-handler/docs/getting-started.html
- install axios (if nescessary)
  - yarn add axios
  - yarb add @types/axios
- install socket.io-client (if nescessary)
  - yarn add axios
  - yarn add @types/axios
- install socket.io-client (if nescessary)
- react-native run-android
- yarn start
