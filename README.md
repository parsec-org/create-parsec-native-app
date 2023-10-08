# create_parsec_app_native

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.



## 使用代码生成库序列化 JSON 数据

### 一次性代码生成

```shell
flutter pub run build_runner build --delete-conflicting-outputs
```

通过在项目根目录运行命令` flutter pub run build_runner build --delete-conflicting-outputs `
，你可以在任何需要的时候为你的模型生成 JSON 序列化数据代码。这会触发一次构建，遍历源文件，选择相关的文件，然后为它们生成必须的序列化数据代码。

虽然这样很方便，但是如果你不需要在每次修改了你的模型类后都要手动构建那将会很棒。

### 持续生成代码

```shell
flutter pub run build_runner watch
```
**监听器** 让我们的源代码生成过程更加方便。它会监听我们项目中的文件变化，并且会在需要的时候自动构建必要的文件。你可以在项目根目录运行` flutter pub run build_runner watch `启动监听。

启动监听并让它留在后台运行是安全的。


了解更多信息，请查阅[传送门](https://flutter.cn/docs/data-and-backend/serialization/json)。