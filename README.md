#  Basic React-Native Boiler Plate
[![React Native](https://img.shields.io/badge/React%20Native-v0.57.8-blue.svg)](https://facebook.github.io/react-native/)
[![React Navigation V3](https://img.shields.io/badge/React%20Navigation-v3.0.9-blue.svg)](https://reactnavigation.org/)
[![js-eslint-style](https://img.shields.io/badge/lint%20compliance-eslint-brightgreen.svg?style=flat)](http://eslint.org/)

* This is a very basic boilerplate of react-native. It will be very helpful to kick-start your project, because it provides some common tools you may need. They are as following:
  * ES6 based project architecture
  * [react-navigation](https://reactnavigation.org/): A very helpful and easily customizable navigation libray.
  * [react-native-extended-stylesheet](https://github.com/vitalets/react-native-extended-stylesheet): Every mobile application should be responsive even if we don't use flex-layout for all the styling in the application. Instead of using the StyleSheet provided by react-native, we recommend using the stylesheet provided by this library.
  * [native-base](https://nativebase.io/): A very rich UI library which is also customizable. By using it, you don't have to create some basic UI components in your application. Further more it also provides [react-native-vector-icons](https://github.com/oblador/react-native-vector-icons) out of the box.
  * "eslint:recommended" linting guide: Writing good and error free code is a must. eslint will help you to write good code and not to make common mistakes.
  * There are pre-commit hooks implemented to prevent bad commits. So if you don't lint your code before commititng it, you won't be able to commit it.

## :arrow_up: How to Setup

**Step 1:** git clone this repo.

**Step 2:** cd to the cloned repo.

**Step 3:** Rename the project bundleId, package name and application name.

**Step 4:** Install the npm modules required for the project with `npm i`


## :arrow_forward: How to Run App

1. cd to the repo
2. Run Build for either OS
  * for iOS
    * run `npm run ios`
  * for Android
    * run `npm run android`

## <div style="display: flex;align-items: center;"><img src="https://eslint.org/img/logo.svg" width="35" title="eslint" style="vertical-align: middle;"> Eslint Compliant</div>

This project adheres to "eslint:recommended" style guide. We have setup and enabled eslint for this project. We suggest that you keep following it.

**To Lint**

This is implemented using [eslint](https://eslint.org). Just run `npm run lint`

**To Fix Lint Errors**

run `npm run fixcode`

**Bypass Lint And Run Project**

If you have to bypass lint and just run the project for special case.
  * for iOS
    * run `react-native run-ios`
  * for Android
    * run `react-native run-android`

**Understanding Linting Errors**

The linting rules are from eslint and React-Standard.  [Regular JS errors can be found with descriptions here](http://eslint.org/docs/rules/), while [React errors and descriptions can be found here](https://github.com/yannickcr/eslint-plugin-react).
We have customised the linting as per our requirements. You can check the .eslintrc of the project and modify it as per your requirements.

## :closed_lock_with_key: Secrets

This project uses [react-native-config](https://github.com/luggit/react-native-config) to expose config variables to your javascript code in React Native. You can store API keys
and other sensitive information in a `.env` file:

```
API_URL=https://myapi.com
GOOGLE_MAPS_API_KEY=abcdefgh
```

and access them from React Native like so:

```
import Secrets from 'react-native-config'

Secrets.API_URL  // 'https://myapi.com'
Secrets.GOOGLE_MAPS_API_KEY  // 'abcdefgh'
```

The `.env` file is ignored by git keeping those secrets out of your repo.

### Get started with react-native-config:
1. Copy .env.example to .env
2. Add your config variables
3. Follow instructions at [https://github.com/luggit/react-native-config#setup](https://github.com/luggit/react-native-config#setup)
4. Done!
