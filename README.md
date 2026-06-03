# Velocity Messenger for Android

Velocity is a blazing fast and secure messaging application built for Android. Based on the robust architecture of the Telegram open-source project, Velocity provides an enhanced user experience with custom features like Premium integrations, AI styling tools, and advanced messaging capabilities.

## 🚀 Features

- **Speed & Security:** Lightning-fast message delivery with state-of-the-art MTProto encryption.
- **Velocity Premium:** Exclusive features, customizations, and capabilities for power users.
- **AI Editor Styles:** Advanced AI-powered styling, shared links, and custom limits.
- **Deep Customization:** Highly customizable UI with various themes and layouts.

## 🛠 Compilation Guide

### Prerequisites
- Android Studio 3.4 or higher
- Android NDK rev. 20
- Android SDK 8.1

### Build Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/techxsarwar/velocity.git
   ```
2. **Setup Keystore:**
   Copy your `release.keystore` into the `TMessagesProj/config` directory.
3. **Configure Gradle:**
   Fill out `RELEASE_KEY_PASSWORD`, `RELEASE_KEY_ALIAS`, and `RELEASE_STORE_PASSWORD` in `gradle.properties` to access your keystore.
4. **Setup Firebase:**
   - Navigate to the [Firebase Console](https://console.firebase.google.com/).
   - Create two Android apps with the application IDs `org.telegram.messenger` and `org.telegram.messenger.beta`.
   - Turn on Firebase Cloud Messaging and download `google-services.json`.
   - Place `google-services.json` in the same folder as `TMessagesProj`.
5. **Open Project:**
   Open the project in Android Studio (Make sure to select **Open**, not Import).
6. **Configure Environment:**
   Fill out the values in `TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java`. There are links provided for each variable explaining where and how to obtain the necessary data.
7. **Build:**
   You are now ready to compile and run Velocity!

## 🔐 Security & API

To interact with the core network, you must obtain your own `api_id` from the [API Development Tools](https://my.telegram.org/apps). 

Please carefully study the [security guidelines](https://core.telegram.org/mtproto/security_guidelines) and ensure that you are taking good care of users' privacy and data security.

## 🌍 Localization

Translations and localizations are managed collectively. If you wish to contribute to the translations, please visit the [Localization Platform](https://translations.telegram.org/en/android/).
