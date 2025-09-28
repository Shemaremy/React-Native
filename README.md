# REACT NATIVE WRAPPER
---------------------------------------------------------------------------------------------------------------

1. New elements not in jsx
2. Changes compared to jsx
3. Environment setup
4. Stylesheets api / inline styles
5. Expo
6. Testing with Expo, web or emulators


---------------------------------------------------------------------------------------------------------------


<!------------------------------- Optionals to install ------------------------------------------
    - Install 'React Native tools' vscode extension for debugging
    - Install 'React-Native/React/Redux snippets for es6/es7' vscode extension for shortcut snippets
------------------------------------------------------------------------------------------------->





## 1. New elements based on jsx
------------------------------

- div → View
- h1, h2, h3, p, span etc. → Text
- img → Image
- button → Button

- ul, ol, li → Custom Views/Text for lists or FlatList/SectionList for dynamic lists
- input (text field) → TextInput
- textarea → TextInput (with multiline={true})

- form → Managed through state and functions
- a (anchor link) → Linking API or custom navigation logic
- select (dropdown) → Picker or custom dropdown components




## 2. Changes made based on jsx
--------------------------------

- No separate css file, styles are done directly in the main file (inline styles or stylesheet api)
- Navigation is handled with libraries like React Navigation, not React Router.

- Animations rely on Animated API, not CSS transitions.
- React Native apps run in a native environment, not a browser.

- Deployment involves App Store and Google Play, not just hosting files on a server.
- Must consider hardware features like cameras, GPS, and sensors.

- We use Expo CLI or React Native CLI, same way we used Vite or CRA in react js
- Expo is like a toolkit for building and testing React Native apps easily.




## 3. Environmental setup  (We're using Expo)
---------------------------------------------

- npm i -g expo-cli
- expo init Flacko
(select blank)

- cd Flacko
- npm start

(You'll then see local host opening from your browser)
(With metro bundler menu indicating on how you want to run your app)



## 4. Run your app on android simulator
---------------------------------------

- Download, run & install android studio app on pc from (https://developer.android.com/studio)
- Once setting up is finished, and see your android on pc screen,
- Go to localhost window from browser and click 'Run on android device'



## 5. Run your app on iOS simulator
-----------------------------------



## 6. Run your app on mobile
-----------------------------
(Make sure pc & phone are connected to same wireless network)

- Download expo app on your phone
- Go to metro bundler and find the qr code
- Open your expo/camera app and scan the code



## 7. Debug app errors in browser
----------------------------------

- Open developer menu on physical/virtual device
- Click 'Debug Remote Js'
- Now go to dev tools on browser as default 

(Make sure to stop remote debugging after you finish doing tasks. It slows down the app)



## 8. Publishing app - for test/dev not production (We will use expo in this case)
----------------------------------------------------------------------------------

- Click publish project in metro bundler
- Follow steps and publish to generate url
- To run, click url and you'll see a qr code
- It will be used to run the app but phone has to have expo app always



## 9. Some elements & events we saw
-----------------------------------
(You first import elements before using them)

- View, SafeAreaView
- Text, Image
- Touchable
- Button

- onPress, onLongpress

- alerts (customizing alerts)



## 8. Stylesheet
----------------

- Used for defining styles

ex:
const styles = StyleSheet.create({
    container: {
        backgroundColor: "red",
        flex: 1
    },
})

