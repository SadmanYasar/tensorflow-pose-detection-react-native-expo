# Overview

A modified version of [TFJS Pose Detection][posedetection] model
([MoveNet.SinglePose.Ligntning][tfhub]) using
[TFJS React Native][tfjs-react-native] in an Expo project. It supports both
portrait and landscape mode with front and back camera. Only the keypoints are
rendered in the demo.

# Note

This project uses Expo SDK 49 and jsc instead of Hermes. FPS is very low on my phone, around 3-4 FPS.

I updated Camera.Constants.Type to CameraType.front/back.

Added 3 additional props to TensorCamera according to [this](https://js.tensorflow.org/api_react_native/0.2.1/#Media-Camera) documentation.

Also updated tsconfig.json to use settings for Expo SDK 49.

Update 9/23/2023: Stopping development on this project for now. Will experiment with Flutter and Firebase MLkit.

# Installation

To run it locally:

```
$ yarn
$ yarn start
```

Then scan the QR code to open it in the `Expo Go` app.

If the app crashes on startup, see [here][readme] for more info.

<img src="screenshot_portrait.jpg" width="250">
<img src="screenshot_landscape.jpg" width="500">

[posedetection]: https://github.com/tensorflow/tfjs-models/tree/master/pose-detection
[tfhub]: https://tfhub.dev/google/tfjs-model/movenet/singlepose/lightning/4
[tfjs-react-native]: https://github.com/tensorflow/tfjs/tree/master/tfjs-react-native
[screenshots]: https://photos.app.goo.gl/U972ww4HpaKPK6jEA
[readme]: https://github.com/tensorflow/tfjs-examples/blob/master/react-native/README.md
