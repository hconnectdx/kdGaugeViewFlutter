# Invites 에서 사용하고 있는 그래프 라이브러리
이 라이브러리를 커스텀하여 인바이츠앱에 사용 (원형 그래프)

#### pubspec.yaml
```dart
  kdgaugeview:
    git:
      url: git@github.com:hconnectdx/kdGaugeViewFlutter.git
      ref: 1.0.9-custom #태그를 사용하여 버전관리 함
```
<image src=https://github.com/hconnectdx/kdGaugeViewFlutter/assets/107895890/95f273ad-86d2-4c6e-a118-41fca2bc16ad width=400/>
	
---


# KdGaugeViewFlutter
KDGaugeView is a simple and customizable gauge control for Android inspired by [KdGaugeView](https://github.com/Sorbh/kdgaugeView)

The source code is **100% Dart**.

[![pub package](https://img.shields.io/pub/v/kdgaugeview.svg?style=flat-square)](https://pub.dartlang.org/packages/kdgaugeview) ![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)


# Motivation

I need some clean Guage view for my Flutter application.

# Getting started

## Installing
Add this to your package's pubspec.yaml file:

This library is posted in pub.dev

#### pubspec.yaml
```dart
dependencies:  
	kdgaugeview: ^1.0.4
```

# Usage

After Importing this library, you can directly use this view in your Widget tree

```dart
import  'package:kdgaugeview/kdgaugeviewflutter.dart';
```

```
 GlobalKey<KdGaugeViewState> key = GlobalKey<KdGaugeViewState>();
```

```dart
KdGaugeView(
    key: key,
    minSpeed: 0,
    maxSpeed: 180,
    speed: 70,
    animate: true,
)
```
Update the speed of the Gauge View using this method

```
key.currentState.updateSpeed(120, animate: true,duration: Duration(milliseconds: 400));
```

# Customization
  Depending on your view you may want to tweak the UI. For now you can these custom attributes

  | Property | Type | Description |
  |----------|------|-------------|
  | 'speed' | double | Initial speed for the Gauge |
  | 'speedTextStyle' | TextStyle | Text Style for Speed Text |



# Screenshots
![alt text](https://github.com/sorbh/kdGaugeViewFlutter/blob/master/raw/demo.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![alt text](https://github.com/sorbh/kdGaugeViewFlutter/blob/master/raw/demo.gif)


 


# Author
  * **Saurabh K Sharma - [GIT](https://github.com/Sorbh)**
  
      I am very new to open source community. All suggestion and improvement are most welcomed. 
  
 
## Contributing

1. Fork it (<https://github.com/sorbh/kdgaugeViewflutter/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

