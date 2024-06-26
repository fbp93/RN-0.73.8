# audio-manager

## Getting started

`$ npm install audio-manager --save`

### Mostly automatic installation

`$ react-native link audio-manager`

### Manual installation

#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `audio-manager` and add `AudioManager.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libAudioManager.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainApplication.java`

- Add `import com.reactlibrary.AudioManagerPackage;` to the imports at the top of the file
- Add `new AudioManagerPackage()` to the list returned by the `getPackages()` method

2. Append the following lines to `android/settings.gradle`:
   ```
   include ':audio-manager'
   project(':audio-manager').projectDir = new File(rootProject.projectDir, 	'../node_modules/audio-manager/android')
   ```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
   ```
     compile project(':audio-manager')
   ```

## Usage

```javascript
import AudioManager from 'audio-manager';

// TODO: What to do with the module?
AudioManager;
```
