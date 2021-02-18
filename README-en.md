![social preview](social-dark.png)

<p align="center">
  <a href="https://pub.dev/packages/fair"><img src="https://img.shields.io/pub/v/fair.svg" alt="pub"></a>
  <a href="https://github.com/wuba/fair"><img src="https://img.shields.io/badge/platform-flutter-blue.svg" alt="github"></a>
  <a href="https://fair.58.com/"><img src="https://img.shields.io/badge/doc-fair.58.com-green.svg" alt="doc"></a>
  <a href="https://github.com/wuba/fair/LICENSE"><img src="https://img.shields.io/badge/license-BSD-green.svg" alt="license"></a>
  <a href="https://github.com/wuba/fair/actions"><img src="https://github.com/wuba/fair/workflows/build/badge.svg" alt="build"></a>
  <a href="https://gitter.im/flutter_fair/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img src="https://badges.gitter.im/flutter_fair/community.svg" alt="Gitter"></a>
</p>

[简体中文](README.md)|[English](README-en.md)

---

Fair is a lightweight package for Flutter, which can be used to update widget tree dynamically. This package is still at an early stage.

We create Fair so we can dispatch UI changes to users as bundle(s), the way similar to React Native. With Flutter Fair integrated, you can publish your UI pages without waiting for the next release date of your App. Fair provides standard widget, it can be used as a new dynamic page or as part of existing Flutter page.

![what-is-fair](https://github.com/wuba/fair/blob/main/fair/what-is-fair-en.png?raw=true)

## Quick Start
Use Flutter Fair require few steps. Add dependency inside `pubspec.yaml`.
```yaml
dependencies:
  fair: ^0.2.0
```

Wrap your app with FairApp Widget.
```dart
void main() {
  runApp(
    FairApp(
      child: MaterialApp(home: App())
    ),
  );
}
```

Import a dynamic widget as FairWidget
```dart
FairWidget(
  type: 'hello_world',
  path: 'assets/bundle/hello_world.json',
)
```

## Documentation
For more details, please refer to [https://fair.58.com](https://fair.58.com)