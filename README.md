# Android 11 Storage Permissions

A modern Android application demonstrating proper implementation of storage permissions for Android 11 (API level 30+) and beyond, with emphasis on scoped storage.

## 📱 Features

- Scoped Storage implementation for Android 11+
- Runtime permissions handling
- File access demonstrations
- Modern Android best practices
- Automated CI/CD builds

## 🛠️ Tech Stack

- **Language:** Java 11
- **Android SDK:** API 34 (Android 14)
- **Minimum SDK:** API 24 (Android 7.0)
- **Build System:** Gradle 8.1.0
- **Architecture Components:** AndroidX

## 📋 Requirements

- Android Studio Flamingo or later
- JDK 11 or higher
- Android SDK 34
- Gradle 8.1.0+

## 🚀 Getting Started

### Clone the Repository
```bash
git clone https://github.com/chandrahotha/Android-11-Storage-Permissions.git
cd Android-11-Storage-Permissions
```

### Build the Project
```bash
./gradlew clean build
```

### Build APK
```bash
./gradlew assembleDebug    # Debug APK
./gradlew assembleRelease  # Release APK
```

### Run Tests
```bash
./gradlew test
```

## 📦 Dependencies

- AndroidX AppCompat 1.7.0
- Material Design 1.12.0
- ConstraintLayout 2.1.4
- JUnit 4.13.2
- Espresso 3.5.1

## 🔄 Continuous Integration

This repository has automated CI/CD with GitHub Actions:

- **Android Build**: Triggers on push/PR to master, main, or develop branches
  - Builds debug and release APKs
  - Runs unit tests
  - Uploads artifacts (APKs, build reports)

- **Release Build**: Triggers on GitHub releases
  - Creates optimized release APK and AAB (Android App Bundle)
  - Automatically uploads to release assets
  - Generates build reports

### Build Status
[![Android Build](https://github.com/chandrahotha/Android-11-Storage-Permissions/actions/workflows/android-build.yml/badge.svg)](https://github.com/chandrahotha/Android-11-Storage-Permissions/actions)

## 📁 Project Structure

```
Android-11-Storage-Permissions/
├── app/                          # Main application module
│   ├── src/
│   │   ├── main/
│   │   │   ├── AndroidManifest.xml
│   │   │   ├── java/            # Application source code
│   │   │   └── res/             # Resources (layouts, strings, etc.)
│   │   ├── test/                # Unit tests
│   │   └── androidTest/         # Instrumented tests
│   └── build.gradle
├── .github/
│   └── workflows/               # GitHub Actions workflows
│       ├── android-build.yml
│       └── release.yml
├── gradle/                       # Gradle wrapper
├── build.gradle                  # Root build configuration
├── settings.gradle              # Project settings
├── gradle.properties            # Gradle properties
└── README.md
```

## 🔐 Permissions

Required permissions (as per Android 11+ storage access):

```xml
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
<uses-permission android:name="android.permission.MANAGE_EXTERNAL_STORAGE" />
```

## 📚 Resources

- [Android Storage Updates](https://developer.android.com/about/versions/11/privacy/storage)
- [Scoped Storage Documentation](https://developer.android.com/training/data-storage/shared/media)
- [Runtime Permissions](https://developer.android.com/training/permissions/requesting)

## 🐛 Known Issues

None currently. Please report any issues [here](https://github.com/chandrahotha/Android-11-Storage-Permissions/issues).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## 📄 License

This project is open source and available under the MIT License.

## ✨ Changelog

### Version 2.0
- Updated to Android SDK 34
- Modernized Gradle build system (8.1.0)
- Updated all dependencies to latest stable versions
- Added GitHub Actions CI/CD workflows
- Improved build performance with caching
- Enhanced security with ProGuard optimization

### Version 1.0
- Initial project setup
- Basic storage permissions implementation

## 👤 Author

[chandrahotha](https://github.com/chandrahotha)

## 📞 Support

For support, please open an issue on [GitHub Issues](https://github.com/chandrahotha/Android-11-Storage-Permissions/issues).

---

**Last Updated:** 2026-07-04
