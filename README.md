# HostelFinder

HostelFinder is an Android app that helps students discover and book student accommodation, while giving hostel owners tools to manage listings and booking requests.

## Features

### For students
- Create an account, sign in, and recover a password.
- Browse and search hostels by district, area, and nearby university.
- Sort listings by price, rating, and availability.
- View hostel details and submit a booking request.
- Save hostels, view bookings, and access messages, reviews, and notifications.

### For hostel owners
- Register and access an owner dashboard.
- Add and manage hostel listings.
- Review booking requests.
- Access owner messages, notifications, profile, settings, and analytics screens.

## Technology

- Native Android application
- Java and Kotlin
- Android Gradle Plugin with Kotlin Gradle DSL
- AndroidX, Material Components, and ConstraintLayout
- Firebase Authentication
- Google Credential Manager and Google ID sign-in libraries

## Requirements

- Android Studio with Android SDK Platform 37 installed
- JDK 11 or a compatible JDK supported by the installed Android Gradle Plugin
- A Firebase project configured for the app

The application ID is `com.example.hostelfinder` and the minimum Android version is API 24 (Android 7.0).

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/ssemwangaerick01-png/hostelfind.git
   cd hostelfind
   ```

2. Open the project in Android Studio and allow Gradle to sync.

3. Configure Firebase for the Android application:
   - Create or select a Firebase project.
   - Add an Android app with package name `com.example.hostelfinder`.
   - Enable the authentication providers used by your configuration.
   - Download `google-services.json` and place it in the `app/` directory.

   Do not commit private credentials or production configuration files to a public repository.

4. Select an emulator or connect an Android device, then run the `app` configuration from Android Studio.

## Build from the command line

On macOS or Linux:

```bash
./gradlew assembleDebug
```

On Windows:

```bat
gradlew.bat assembleDebug
```

The debug APK is written to `app/build/outputs/apk/debug/app-debug.apk`.

## Project structure

```
app/
  src/main/
    java/com/example/hostelfinder/  # Android activities and app logic
    res/                            # Layouts, drawables, and other resources
    AndroidManifest.xml
gradle/
  libs.versions.toml                # Dependency versions
build.gradle.kts
settings.gradle.kts
```

## Current implementation notes

This repository is an early-stage app. Some screens use sample hostel data or temporary in-memory interactions; booking submission and other flows may not yet persist data to a backend. Firebase Authentication is included as a dependency, but a valid local Firebase configuration is required to build and use Firebase-backed features.

## Contributing

1. Fork the repository.
2. Create a branch for your change.
3. Make and verify your changes in Android Studio.
4. Open a pull request with a clear description.

## License

No license file is currently included. Contact the repository owner before redistributing or reusing this project.
