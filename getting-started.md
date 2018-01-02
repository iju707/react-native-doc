# 시작하기

이번 페이지에서는 React Native를 설치하고 첫번째 어플리케이션을 만들어보겠습니다. 만약 React Native가 설치되어있다면, [자습서](https://facebook.github.io/react-native/docs/tutorial.html)을 생략하셔도 됩니다.

## 빠르게 시작하기

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

### React Native 어플리케이션 실행

iOS나 Android 폰에 [Expo](https://expo.io/) 클라이언트 앱을 설치하고 컴퓨터와 동일한 네트워크에 접속을 합니다. Expo 앱을 이용하여 터미널에 표시되는 QR 코드를 스캔하시면 프로젝트가 실행됩니다.

#### 어플리케이션 수정하기

성공적으로 어플리케이션이 실행되면, 수정해보겠습니다. `App.js` 파일을 열고 일부 라인을 수정합니다. 수정사항을 저장하면 어플리케이션이 자동으로 재기동될 것 입니다.

#### 이것이 전부입니다!

축하합니다! 첫번째 React Native 어플리케이션에 대한 실행과 수정을 완료하였습니다.

![](https://facebook.github.io/react-native/docs/assets/GettingStartedCongratulations.png)