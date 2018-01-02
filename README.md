# React Native Document

## Javascript와 React를 활용하여 Native Mobile 어플리케이션을 만들어보세요.

React Native는 Javascript만을 이용하여 모바일 앱을 만들수 있게 해줍니다. React와 동일한 구조로 되어있으며, 정의된 컴포넌트를 활용하여 모바일 UI를 만들 수 있습니다.

```js
import React, { Component } from 'react';
import { Text, View } from 'react-native';

class WhyReactNativeIsSoGreat extends Component {
  render() {
    return (
      <View>
        <Text>
          If you like React on the web, you'll like React Native.
        </Text>
        <Text>
          You just use native components like 'View' and 'Text',
          instead of web components like 'div' and 'span'.
        </Text>
      </View>
    );
  }
}
```

## React Native 앱은 실제 모바일앱입니다.

React Native를 사용하면 "모바일웹 앱", "HTML5 앱", "Hybrid 앱"을 만들 필요가 없습니다. Objective-C나 Java를 사용하여 만든 앱과 구분할 수 없는 실제 모바일 앱을 만들게 됩니다. React Native에서는 일반적인 iOS나 안드로이드 앱과 같은 동일한 UI 개발구조를 사용하고 있습니다. Javascript와 React를 사용하여 이러한 개발구조을 추가할 수 있습니다.

```js
import React, { Component } from 'react';
import { Image, ScrollView, Text } from 'react-native';

class AwkwardScrollingImageWithText extends Component {
  render() {
    return (
      <ScrollView>
        <Image
          source={{uri: 'https://i.chzbgr.com/full/7345954048/h7E2C65F9/'}}
          style={{width: 320, height:180}}
        />
        <Text>
          On iOS, a React Native ScrollView uses a native UIScrollView.
          On Android, it uses a native ScrollView.

          On iOS, a React Native Image uses a native UIImageView.
          On Android, it uses a native ImageView.

          React Native wraps the fundamental native components, giving you
          the performance of a native app, plus the clean design of React.
        </Text>
      </ScrollView>
    );
  }
}
```

## 재컴파일로 시간을 낭비할 필요가 없습니다.

React Native는 앱을 더 빠르게 만들 수 있게 합니다. 재컴파일과정이 필요없이 즉시 앱을 재기동할 수 있습니다. [Hot Reloading](http://facebook.github.io/react-native/blog/2016/03/24/introducing-hot-reloading.html)을 사용하면 어플리케이션 상태를 유지하면서 새로운 코드를 반영할 수 있습니다.

![](https://media.giphy.com/media/13WZniThXy0hSE/giphy.gif)

## 필요하면 Native 코드를 사용할 수 있습니다.

React Native는 Objective-C나 Java, Swift로 작성된 컴포넌트와 부드럽게 조합할 수 있습니다. 어플리케이션의 일부 기능에 대한 최적화가 필요하여 Native 코드로 작성된 컴포넌트를 쉽게 추가할 수 있습니다. Facebook 앱이 실제로 하는 것 처럼, 앱에 대한 일부는 React Native로 작성하고 일부는 Native 코드를 직접 사용하여 구성할 수 있습니다.

```js
import React, { Component } from 'react';
import { Text, View } from 'react-native';
import { TheGreatestComponentInTheWorld } from './your-native-code';

class SomethingFast extends Component {
  render() {
    return (
      <View>
        <TheGreatestComponentInTheWorld />
        <Text>
          TheGreatestComponentInTheWorld could use native Objective-C,
          Java, or Swift - the product development process is the same.
        </Text>
      </View>
    );
  }
}
```