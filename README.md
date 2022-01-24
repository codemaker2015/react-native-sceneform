# react native sceneform

<img src="demo/screenshot.png" />

# Requirements

This package requires your app to target Android SDK 24 at least and react-native 0.66+

Also, this package does not handle permissions, be sure to request:

- CAMERA: for AR view.
- WRITE_EXTERNAL_STORAGE: for screenshots.
- RECORD_AUDIO: for recording video.
- ACCESS_FINE_LOCATION/ACCESS_COARSE_LOCATION: for location-based AR.

# Installation

- Install from npm running `npm install --save @sceneview/react-native-sceneform`
- Add the following to your AndroidManifest.xml inside the Application node.
```xml
<meta-data  android:name="com.google.ar.core"  android:value="required"  />
```
- In your app/build.gradle, set your minSdkVersion to 24.

If you are going to use Cloud Anchors, be sure to add your API Key to the AndroidManifest or to sign your application in the Google Cloud Platform console (keyless auth)

# Loading the library

`import { SceneformView, AugmentedFacesView } from 'react-native-sceneform';`

# Components and Definitions

### » [SceneformView](./docs/SCENEFORMVIEW.md)
### » [AugmentedFacesView](./docs/AUGMENTED_FACES.md)
### » [Type Definitions](./docs/TYPES.md)

# To do

- Augmented images
- No-AR view (3D model viewer)
- Runtime renderable creation
- Custom lights
- Animation manipulation (currently animations are played automatically)
- Depth toggling
