# social_auth_buttons
[![Pub Version](https://img.shields.io/pub/v/auth_buttons?color=blue&logo=dart)](https://pub.dev/packages/auth_buttons)

Social Auth Buttons is a fork of auth_buttons flutter widget library. It includes buttons for authenticating with the most popular social networks and with email/password.

## Installation
1) Add this to your packages pubspec.yaml file:
```yaml
dependencies:
  auth_buttons: ^0.0.5
```
2) Install it 
You can install it from the command line:
```bash
$ flutter pub get
```
3) Import it 
Now in Dart code, you can use:
```dart
import 'package:auth_buttons/social_auth_buttons.dart';
```

## Recommendation

We recommend you to using `show` special when you want use some button.
`show` help you importing part of library.

```dart
import 'package:auth_buttons/social_auth_buttons.dart'
    show GoogleAuthButton, AuthButtonStyle;
```

## Overview

There are two style you can choose between them:
1. [Default](#default-style)
1. [Icon](#icon-style)

Note: all api is documented click `Ctrl + Q` to read the docs if you are using `Android Studio`
or `Intellij Idea` on `Visual Studio Code` just hover over.

![default-light](./doc/readme_assets/api-docs-example-1.png)

This is happen if you know you some property, other way click `Ctrl + space` then `Ctrl + Q`
double click and the result will be like so.
![default-light](./doc/readme_assets/api-docs-example-2.png)


## Using
 
You need to use just the following code: 

### Default style

```dart
GoogleAuthButton(
  onPressed: () {},
  darkMode: false,
),
```
![default-light](./doc/readme_assets/full-button-light.png)

```dart
GoogleAuthButton(
  onPressed: () {},
  darkMode: true,
),
```
![default-dark](./doc/readme_assets/full-button-dark.png)


### Icon Style
```dart
GoogleAuthButton(
  onPressed: () {},
  darkMode: false,
  style: AuthButtonStyle.icon,
),
```
![light-icon](./doc/readme_assets/icon-button-light.png)

```dart
GoogleAuthButton(
  onPressed: () {},
  darkMode: true,
  style: AuthButtonStyle.icon,
),
```
![dark-icon](./doc/readme_assets/icon-button-dark.png)


Do same think with the other buttons, when you want customize any button 
you can do it just passing a property which you want.

Full property you can passing:

```dart
GoogleAuthButton(
  onPressed: () {},
  buttonColor: Colors.white,
  splashColor: Colors.grey,
  elevation: 2.0,
  borderRadius: 8.0,
  padding: EdgeInsets.all(8.0),
  text: 'Sign in with Google',
  textStyle: TextStyle(),
  darkMode: false,
  borderColor: Colors.red,
  borderWidth: 1.0,
  style: AuthButtonStyle.icon,
  width: 280.0,
  height: 50.0,
  iconSize: 35.0,
  separator: 15.0,
),
```

[return up](#auth_buttons)
