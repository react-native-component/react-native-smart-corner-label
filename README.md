# react-native-smart-corner-label
A smart corner label for React Native app, written in JS for cross-platform support.
It works on iOS and Android.

This component is compatible with React Native 0.25 and newer.

## Preview

![react-native-smart-corner-label-preview-ios][1]
![react-native-smart-corner-label-preview-android][4]

## Installation

```
npm install react-native-smart-corner-label --save
```

or

```
npm install @react-native-component/react-native-smart-corner-label --save
```



## Usage

Install the button from npm with `npm install @react-native-component/react-native-smart-corner-label --save`.
Then, require it from your app's JavaScript files with `import Button from '@react-native-component/react-native-smart-corner-label'`.

```js
export default class CornerLabelDemo extends Component {

  render() {
    return (
      <View style={{flex: 1, justifyContent: 'center', alignItems: 'center', backgroundColor: '#fff',}}>
        <View style={{ overflow: 'hidden', //don't forget to set this
                       justifyContent: 'center', alignItems: 'center', height: 100, width: 100,
                       borderWidth: StyleSheet.hairlineWidth, borderColor: '#eee', margin: 5}}>
          <Image source={image_shopping} style={{width: 30, height: 30, marginHorizontal: 10, marginBottom: 10,}}/>
          <Text>shopping</Text>
          <CornerLabel
            cornerRadius={36}
            style={{backgroundColor: 'red', }}
            textStyle={{fontSize: 10, color: '#fff', }}>
            New
          </CornerLabel>
        </View>
        <View style={{ overflow: 'hidden', //don't forget to set this
                       justifyContent: 'center', alignItems: 'center', height: 100, width: 100,
                       borderWidth: StyleSheet.hairlineWidth, borderColor: '#eee', margin: 5}}>
          <Image source={image_shopping} style={{width: 30, height: 30, marginHorizontal: 10, marginBottom: 10,}}/>
          <Text>购物</Text>
          <CornerLabel
            cornerRadius={36}
            style={{backgroundColor: 'red', }}
            textStyle={{fontSize: 12, color: '#fff', transform: [{rotate: '-45deg'}],}}>
            新
          </CornerLabel>
        </View>
        <View style={{ overflow: 'hidden', //don't forget to set this
                       justifyContent: 'center', alignItems: 'center', height: 100, width: 100,
                       borderWidth: StyleSheet.hairlineWidth, borderColor: '#eee', margin: 5}}>
          <Image source={image_shopping} style={{width: 30, height: 30, marginHorizontal: 10, marginBottom: 10,}}/>
          <Text>shopping</Text>
          <CornerLabel
            cornerRadius={54}
            style={{backgroundColor: 'red', height: 24,}}
            textStyle={{color: '#fff', }}>
            30% off
          </CornerLabel>
        </View>
        <View style={{ overflow: 'hidden', //don't forget to set this
                       justifyContent: 'center', alignItems: 'center', height: 100, width: 100,
                       borderWidth: StyleSheet.hairlineWidth, borderColor: '#eee', margin: 5}}>
          <Image source={image_shopping} style={{width: 30, height: 30, marginHorizontal: 10, marginBottom: 10,}}/>
          <Text>购物</Text>
          <CornerLabel
            cornerRadius={54}
            style={{backgroundColor: 'red', height: 24,}}
            textStyle={{color: '#fff', fontSize: 12,}}>
            3折优惠
          </CornerLabel>
        </View>
      </View>
    )
  }
}
```

## Props

Prop                   | Type   | Optional | Default   | Description
---------------------- | ------ | -------- | --------- | -----------
cornerRadius           | number | No       |           | determines the value of the corner's radius.
style                  | style  | Yes      |           | see [react-native documents][2]
textStyle              | style  | Yes      |           | see [react-native documents][3]

[1]: http://cyqresig.github.io/img/react-native-smart-corner-label-preview-ios-v1.0.0.gif
[2]: https://facebook.github.io/react-native/docs/style.html
[3]: https://facebook.github.io/react-native/docs/text.html#style
[4]: http://cyqresig.github.io/img/react-native-smart-corner-label-preview-android-v1.0.0.gif
