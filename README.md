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