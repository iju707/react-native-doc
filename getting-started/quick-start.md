# 빠르게 시작하기

[Create React Native App](https://github.com/react-community/create-react-native-app)은 새로운 React Native 어플리케이션을 쉽고 빠르게 만들 수 있게 합니다. 별도로 Native 코드의 빌드를 위한 Xcode, Android Studio나 다른 툴의 설치/설정 필요없이 프로젝트를 시작할 수 있게 합니다.([주의사항](#caveats) 참조)

만약 [Node](https://nodejs.org/en/download/)가 설치되어있다면, npm을 활용하면 `create-react-native-app`을 다음 명령으로 설치할 수 있습니다.

```bash
npm install -g create-react-native-app
```

설치한 다음 다음 명령으로 "AwesomeProject"라는 새로운 React Native 프로젝트를 만들 수 있습니다.

```bash
create-react-native-app AwesomeProject

cd AwesomeProject
npm start
```

개발서버를 시작하게 되며 터미널에 QR코드를 출력하게 될 것 입니다.

## React Native 어플리케이션 실행

iOS나 Android 폰에 [Expo](https://expo.io/) 클라이언트 앱을 설치하고 컴퓨터와 동일한 네트워크에 접속을 합니다. Expo 앱을 이용하여 터미널에 표시되는 QR 코드를 스캔하시면 프로젝트가 실행됩니다.

### 어플리케이션 수정하기

성공적으로 어플리케이션이 실행되면, 수정해보겠습니다. `App.js` 파일을 열고 일부 라인을 수정합니다. 수정사항을 저장하면 어플리케이션이 자동으로 재기동될 것 입니다.

### 이것이 전부입니다!

축하합니다! 첫번째 React Native 어플리케이션에 대한 실행과 수정을 완료하였습니다.

![](https://facebook.github.io/react-native/docs/assets/GettingStartedCongratulations.png)

## 이제 뭘할까요?

Create React Native App에 대하여 궁금한 점이 있는 경우에는 [사용자 가이드](https://github.com/react-community/create-react-native-app/blob/master/react-native-scripts/template/README.md)를 참고하시면 됩니다.

만약 원하는 대로 동작하지 않으면, Create React Native App의 README 중 [Troubleshooting](https://github.com/react-community/create-react-native-app/blob/master/react-native-scripts/template/README.md#troubleshooting) 섹션을 보시면 됩니다.

React Native에 대하여 좀더 배우고 싶으면, [튜토리얼](https://facebook.github.io/react-native/docs/tutorial.html)을 계속 진행하시면 됩니다.

## 어플리케이션을 시뮬레이터나 가상장치에 실행하기

Create React Native App은 별도의 개발환경 설정하지 않고도 물리적 장치에 React Native 앱을 쉽게 실행할 수 있게 해줍니다. 만약 iOS 시뮬레이터나 Android 시뮬레이터를 이용하여 앱을 실행하고 싶으면 Xcode나 Android 개발 환경을 설정하여 Native 코드와 함께 빌드하는 방법을 참고하시면 됩니다.

이러한 설정이 끝나면 Android 가상장치는 `npm run android` 명령으로, iOS 시뮬레이터는(macOS 전용) `npm run ios` 명령으로 앱을 실행할 수 있습니다.

# 주의사항

Because you don't build any native code when using Create React Native App to create a project, it's not possible to include custom native modules beyond the React Native APIs and components that are available in the Expo client app.

If you know that you'll eventually need to include your own native code, Create React Native App is still a good way to get started. In that case you'll just need to "eject" eventually to create your own native builds. If you do eject, the "Building Projects with Native Code" instructions will be required to continue working on your project.

Create React Native App configures your project to use the most recent React Native version that is supported by the Expo client app. The Expo client app usually gains support for a given React Native version about a week after the React Native version is released as stable. You can check this document to find out what versions are supported.

If you're integrating React Native into an existing project, you'll want to skip Create React Native App and go directly to setting up the native build environment. Select "Building Projects with Native Code" above for instructions on configuring a native build environment for React Native.