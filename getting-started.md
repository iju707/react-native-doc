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
