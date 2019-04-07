
# react-native-native-ios

## Getting started

`$ npm install react-native-native-ios --save`

### Mostly automatic installation

`$ react-native link react-native-native-ios`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-native-ios` and add `RNNativeIos.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNNativeIos.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNNativeIosPackage;` to the imports at the top of the file
  - Add `new RNNativeIosPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-native-ios'
  	project(':react-native-native-ios').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-native-ios/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-native-ios')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNNativeIos.sln` in `node_modules/react-native-native-ios/windows/RNNativeIos.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Native.Ios.RNNativeIos;` to the usings at the top of the file
  - Add `new RNNativeIosPackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNNativeIos from 'react-native-native-ios';

// TODO: What to do with the module?
RNNativeIos;
```
  