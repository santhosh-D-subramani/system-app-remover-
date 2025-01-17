# System App Remover

**System App Remover** is a Flutter application designed to help Android users delete unwanted system apps (bloatware) from their devices. This app leverages the ADB (Android Debug Bridge) commands and organizes system apps into various categories, providing a more convenient and efficient way to manage system bloatware.

## Download

[Play Store Link](https://play.google.com/store/apps/details?id=com.santhoshDsubramani.systemappremover)

## TODO
<br>

| Task                   | Status   |
|------------------------|----------|
| create a [new flugin plugin for Shizuku Api](https://pub.dev/packages/shizuku_api)     | ✅ Done  |
| add ADB inBuilt to app, without relying on a-Shell  |  ✅ Done |

<br>
## Features

- **System App Categorization**: The app filters system apps into the following categories:
  - `recommendedApps`
  - `advancedApps`
  - `expertApps`
  - `unsafeApps`
  - `others`

- **App Selection & Copy**: Users can select apps from these categories and copy their package names. These can then be pasted directly into **AShell**, an app that uses the Shizuku API to run ADB commands directly on the Android device.

- **History & Analysis**: 
  - **Copied Apps History**: The history page maintains a list of copied app package names along with the commands applied to them:
    - `pm uninstall --user 0`
    - `pm uninstall -k --user 0`
    - `pm disable-user --user 0`
  - The command prefix (selected in the settings screen) is applied to each copied app.
  - **App Analysis**: The analysis page scans the copied list and checks whether the apps have been deleted. It also provides the option to try a different command prefix if the uninstallation was unsuccessful.

- **Language Support**: The app supports multiple languages:
  - English (`en_US`)
  - German (`de_DE`)
  - French (`fr_FR`)
  - Hindi (`hi_IN`)
  - Tamil (`ta_IN`)
  - Chinese (`zh_CN`)
  - Japanese (`ja_JP`)
  - Spanish (`es_ES`)
  - Portuguese (`pt_PT`)
  - Russian (`ru_RU`)

- **Theme Switching**:
  - Users can switch between light and dark themes.

