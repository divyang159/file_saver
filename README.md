# file_saver

A Flutter package that allows you to download image/file from url.

## Preview

https://github.com/divyang159/file_saver/assets/55906611/0e63da7c-a9af-4575-b163-d1f10cc1a920

## Installing

1.  Add dependency to `pubspec.yaml`

```dart
dependencies:
  file_saver: <latest-version>
```

2.  Import the package
```dart
import 'package:file_saver/file_saver.dart';
```


3Adding an onPressed of button.
```dart
try {
FileSaver()
    .urlFileSaver(url: controller.text,
fileName: "cat-sample_1313.jpg");
} catch(e) {
print(e);
}
```



## Platform specific configuration

### For image Picker
#### iOS
* Add the following keys to your _Info.plist_ file, located in `<project root>/ios/Runner/Info.plist`:

```
    <key>NSCameraUsageDescription</key>
    <string>Used to demonstrate image picker plugin</string>
    <key>NSMicrophoneUsageDescription</key>
    <string>Used to capture audio for image picker plugin</string>
    <key>NSPhotoLibraryUsageDescription</key>
    <string>Used to demonstrate image picker plugin</string>
```

### For voice messages

#### Android
* Change the minimum Android sdk version to 21 (or higher) in your android/app/build.gradle file.
```
    minSdkVersion 21
```

* Add RECORD_AUDIO permission in `AndroidManifest.xml`
```
    <uses-permission android:name="android.permission.RECORD_AUDIO"/>
    <uses-permission android:name="android.permission.RECORD_AUDIO"/>
    <uses-permission android:name="android.permission.RECORD_AUDIO"/>
```

## License

```text
MIT License
Copyright (c) 2024 Divyang Parmar
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
