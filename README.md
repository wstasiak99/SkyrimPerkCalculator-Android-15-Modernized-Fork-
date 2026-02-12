# Skyrim Perk Calculator (Android 15 Modernized Fork)

[![Android SDK](https://img.shields.io/badge/SDK-35%20%28Android%2015%29-green.svg)](https://developer.android.com/about/versions/15)
[![Java](https://img.shields.io/badge/Java-17-orange.svg)](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
[![Gradle](https://img.shields.io/badge/Gradle-8.14.4-blue.svg)](https://gradle.org/releases/)

This is a modernized fork of the original [SkyrimPerkCalculator](https://github.com/PawelS96/SkyrimPerkCalculator) by @PawelS96. The original project was no longer buildable on modern Android Studio versions due to deprecated plugins and old Gradle configurations.

**This version has been updated to run on Android 14 and 15 (target SDK 35).**

## Key Modernization Changes

To make this project buildable and stable in 2026, the following updates were implemented:

- **Build System:** Migrated to **Gradle 8.14.4** with **Android Gradle Plugin 8.5.2**.
- **Modern Java:** Project now requires **JDK 17** for compilation.
- **Android 15 Support:** Updated `compileSdk` and `targetSdk` to **35**.
- **Core Updates:**
    - Centralized repository management in `settings.gradle`.
    - Centralized plugin versions in root `build.gradle`.
    - Enabled `buildConfig` generation (required by the app logic).
    - Fixed Material Design resource paths (specifically `design_bottom_sheet` ID issues).
- **Minimum Requirements:** Bumped `minSdk` to **26** (Android 8.0) to support modern libraries.

## How to Build

1. Clone this repository.
2. Open the project in the latest **Android Studio (Ladybug or newer)**.
3. Ensure your **Gradle JDK** is set to **Java 17** (Settings -> Build, Execution, Deployment -> Build Tools -> Gradle).
4. Sync the project and run the `app` module.

## License
This project is licensed under the same terms as the original repository.
