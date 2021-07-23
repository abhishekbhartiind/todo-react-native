### React Native Learning

```
npm install -g expo-cli

# generate a new app
expo init project_name

# make sure to navigate inside the project directory
cd project_name

yarn add react-navigation react-navigation-stack react-native-paper @react-native-community/masked-view

expo install react-navigation react-native-gesture-handler react-native-reanimated react-native-screens react-navigation-stack

```

Components are the visual elements that you see on the screen in a React Native app.
1. View
2. Text
3. StyleSheet


A View component is the basic building block in a React Native component file. 
It maps to fundamental native iOS (UIView) and Android (View) components, hence its name.
It puts a container element that supports layout styling with flexbox and other styles using a JavaScript object called StyleSheet.

`react-navigation-stack`
- provides a built-in function that returns a react component
- createStackNavigator: takes a route configuration object and an options object

`react-navigation`
- provides a function called createAppContainer that also returns a React component.

`react-native-paper`
- PaperProvider component is going to wrap the navigator and provides the theme to all the components in the framework 
- provides cross-platform components to add to the app.

a mode property for the stack navigator. The value of this property is used to define a specific way to render styles and transitions. The default value of this property is card for screen transitions in iOS and Android. In the above snippet, add the property with a value of modal

A modal is like a popup that displays the content but temporarily blocks the interaction from the primary screen.

```
import { Text, FAB } from 'react-native-paper'

```
Using navigation.navigate as the value of the button press prop onPress, 
the app will navigate to the screen with its name passed as the second parameter

`
yarn add react-native-gesture-handler
`

FlatList
- It is an efficient way to create scrolling data lists in a React Native app.
- data: an array of data used to create a list. Generally, this array is built from multiple objects.
- renderItem: a function that takes an individual element from the data array and renders it on the UI.
- keyExtractor: tells the list of data to use the unique identifiers or ID for an individual element.

