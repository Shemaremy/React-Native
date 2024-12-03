# REACT NATIVE WRAPPER
---------------------------------------------------------------------------------------------------------------

1. New elements based on jsx
2. Changes made based on jsx
3. Environment setup
4. Stylesheets api / inline styles
5. Expo

6. Testing with Expo, web or emulators
7. 


---------------------------------------------------------------------------------------------------------------


<!------------------------------- Optionals to install ------------------------------------------
    - Install 'React Native tools' vscode extension for debugging
    - Install 'React-Native/React/Redux snippets for es6/es7' vscode extension for shortcut snippets
    - Install 'Prettier' for formatting our code
    - Install 'Material Icon theme' for project directory icons
------------------------------------------------------------------------------------------------->







## 1. New elements based on jsx
------------------------------

- div → View
- h1, h2, h3, etc. → Text
- p, span → Text
- img → Image
- button → TouchableOpacity, Button, or Pressable

- ul, ol, li → Custom Views/Text for lists or FlatList/SectionList for dynamic lists
- input (text field) → TextInput
- textarea → TextInput (with multiline={true})
- form → Managed through state and functions
- a (anchor link) → Linking API or custom navigation logic

- select (dropdown) → Picker or custom dropdown components
- video → Use a library like react-native-video
- audio → Use libraries like react-native-sound
- hr (horizontal rule) → Custom View with styles for a line
- table, tr, td → Use View and Text with Flexbox styling














## 2. Changes made based on jsx
--------------------------------

- No separate css file for styles, styles are done directly in the main file (inline styles or stylesheet api)
- No DOM in React Native, it uses native components.
- Navigation is handled with libraries like React Navigation, not React Router.
- No traditional HTML events; instead, use Touchables (e.g., TouchableOpacity, TouchableWithoutFeedback).
- Animations rely on Animated API, not CSS transitions.

- Use Flexbox exclusively for layout (no Grid, float, or inline-block).
- Platform-specific code is possible with .ios.js and .android.js files.
- No browser-based APIs (e.g., document, window).
- React Native apps run in a native environment, not a browser.
- Libraries for features like video, audio, and WebView need to be installed separately.

- Debugging is done with tools like React Native Debugger or Flipper, not just browser DevTools.
- React Native has native modules for bridging to platform-specific functionality.
- Use the Expo framework for easier app development and deployment (optional).
- Deployment involves App Store and Google Play, not just hosting files on a server.
- React Native requires Metro Bundler, not Webpack.

- Testing involves emulators/simulators, not browsers.
- Native app performance tuning is often needed for heavy tasks.
- No HTML semantics, so accessibility is handled differently.
- Must consider hardware features like cameras, GPS, and sensors.
- We use Expo CLI or React Native CLI, same way we used Vite or CRA in react js
- Expo is like a toolkit for building and testing React Native apps easily.






















## 3. Environmental setup  (We're using Expo)
---------------------------------------------

- Install 'Expo client' app on your mobile phone
- Install Expo CLI (same way we start with installing Vite in react js): npx create-expo-app Flacko --template blank
- Go to project directory: cd Flacko
- Start the app: npx expo start
- Then scan the qr code in terminal, click the link then it will redirect on expo app

- To run on machine, install: npx expo install react-dom react-native-web @expo/metro-runtime
- Them npx expo start, and after click 'w'
- But there is no ios simulators on windows pc


We dont need the npm i like reactjs cause by installing Expo CLI, it automatically installs dependencies












