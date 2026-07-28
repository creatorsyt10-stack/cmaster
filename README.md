# CMaster

CMaster is a Kotlin + Jetpack Compose MVP for learning C programming from basic to intermediate concepts. The app opens directly in guest mode, stores progress locally, includes chapter lessons, practice tasks, quizzes, search, settings, and a built-in beginner-focused C lab.

## Tech Stack

- Kotlin
- Jetpack Compose
- Material Design 3
- MVVM
- Local `SharedPreferences` progress storage
- Dark theme by default

## Open In Android Studio

1. Open the `CMaster` folder in Android Studio.
2. Install Android SDK 36 or adjust `compileSdk` and `targetSdk` in `app/build.gradle.kts` to an installed SDK.
3. Use JDK 17 or newer.
4. Let Android Studio sync the project. If it asks to create Gradle wrapper files, accept the prompt.
5. Run the `app` configuration.

## MVP Note

The compiler screen uses a pluggable `CCompilerEngine` abstraction. Version 1.0 ships with `TeachingCCompilerEngine`, which runs common beginner examples locally, including simple declarations, `scanf`, and `printf` formatting. Replace that engine later with a native TinyCC/Clang backend, WASM sandbox, or a cloud compiler without changing the UI.
