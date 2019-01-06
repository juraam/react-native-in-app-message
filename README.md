React Native in-app platform-specific notifications. 


<img src="https://user-images.githubusercontent.com/17552441/50739935-cae35080-11f7-11e9-96f9-a87579e405dd.gif" width="250" height="400" /><img src="https://user-images.githubusercontent.com/17552441/50739938-db93c680-11f7-11e9-84e3-a7a07feba7b9.gif" width="200" height="400" /><img src="https://user-images.githubusercontent.com/17552441/50739945-e9e1e280-11f7-11e9-9d0b-4d15db0e1c3d.gif" width="200" height="400" />


- The package uses react-native-blur and gesture-handler to implement native-like appearance
- Compatible with iPhone X, XR, XS, XS Max.
- Allows you to use your own components.

## Installation

- Run `npm install react-native-in-app-message`
- Run `npm install react-native-gesture-handler` and follow the <a href="https://kmagiera.github.io/react-native-gesture-handler/docs/getting-started.html#installation">linking guide</a>
- Run `npm install react-native-blur` and follow the <a href="https://github.com/react-native-community/react-native-blur#installation">linking guide</a>

## Usage

```
import {Notification} from "react-native-in-app-message";

...

render() {
    return (
      <View>
        <AppNavigator screenProps={{showNotification: this.showMessage}} />
        <Notification 
            text={'Hello world'}
            onPress={this.hideMessage} 
            ref={node => this.notification = node} 
            textColor={'#000'} />
      </View>
    )
  }

```

## 