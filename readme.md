```
╔═╗╦  ╦ ╦╔╦╗╔╦╗╔═╗╦═╗  ╔═╗╔╦╗╔═╗╦═╗╔╦╗╔═╗╦═╗
╠╣ ║  ║ ║ ║  ║ ║╣ ╠╦╝  ╚═╗ ║ ╠═╣╠╦╝ ║ ║╣ ╠╦╝
╚  ╩═╝╚═╝ ╩  ╩ ╚═╝╩╚═  ╚═╝ ╩ ╩ ╩╩╚═ ╩ ╚═╝╩╚═
```                                                         

Use this template to start up a new flutter project

**Note that these are just guidelines**

### Setup

- Clone the repo with `git clone git@github.com:cpuccino/flutter_starter.git`
- Remove .git and reset the version in pubspec
- [Rename](https://pub.dev/packages/rename) the project and update it's bundle id using
  ```
  pub global activate rename
  pub global run rename --bundleId "com.cpuccino.appname"
  pub global run rename --appname "App Name"
  ```
- Do a global search for any remaining instance of "com.example.flutter_starter" and replace it with the proper value
- Replace `android/app/src/main/kotlin/com/example/flutter_starter` with `android/app/src/main/kotlin/com/cpuccino/appname`

### Project structure

```
lib
  │
  ├── configurations
  |   ├── application_configuration.dart // Application specific configuration & metadata ex:  application name, version info
  |   ├── colors_configuration.dart // Define colors used within the app 
  |   ├── fonts_configuration.dart // Define fonts used within the app (styles and size)
  |   ├── gutters_configuration.dart // Defines margin and padding used within the app
  |   └── media_configuration.dart // Defines screensizes to be used within the app ex: xxs: 350, xs: 500, s: 750, m: 1000, l: 1300, xl: 1500, xxl: 2000
  |
  ├── controllers // state management (controllers, providers, blocs)
  |   ├── authentication_controller.dart
  |   ├── authorization_controller.dart
  |   └── etc...
  |
  ├── domain // app specific logic
  |   ├── auth
  |   |   ├── src
  |   |   |   ├── authentication.dart
  |   |   |   ├── authorization.dart
  |   |   |   └── etc...
  |   |   └── auth.dart // exports everything in the auth src
  |   └── etc...
  |
  ├── components // follows atomic design https://atomicdesign.bradfrost.com
  |   ├── atom
  |   ├── molecule
  |   └── organism
  |
  └── screens
      ├── home_screen.dart
      └── etc...
```

