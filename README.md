# ClearCue — Understand Before You Act

**A Smart Document, Bill & Medicine Understanding Assistant**

ClearCue is an Android application built with Flutter that helps users understand everyday documents, public notices, bills, and medicine-related information through a simple, user-friendly interface.

The goal is to make complex information easier to understand by organizing extracted details into clear, useful information.

## ✨ Features

### 📄 Document & Notice Understanding
- Helps users review information from documents and public notices.
- Makes important details easier to identify and understand.

### 🧾 Bill Analysis
- Helps users examine bill information.
- Makes relevant details easier to review.

### 💊 Medicine Scanner
- Uses text recognition to extract text from medicine-related images.
- Helps users review the information printed on medicine packaging.

### 📚 Medicine Library
- Provides a dedicated section for medicine information.

### 🕘 Scan History
- Stores previous scan records locally.
- Allows users to revisit saved scan results.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Flutter | Android app UI and development |
| Dart | Application programming |
| SQLite | Local database storage |
| Google ML Kit Text Recognition | Text extraction from images |

## 🏗️ Architecture

ClearCue follows a layered architecture to separate the user interface, business logic, data access, and storage.

```text
          User
           |
           v
      Flutter Screens
           |
           v
        Analyzer
      (Business Logic)
           |
           v
       Repositories
           |
           v
      SQLite Database
        clearcue.db
```

### Database

The local SQLite database includes these tables:

- `medicines` — medicine-related records
- `scans` — scan history records
- `qa` — question-and-answer related records

## 📱 Application Screens

The application home screen is designed around five main sections:

1. Document / Notice
2. Bill Analysis
3. Medicine Scanner
4. Medicine Library
5. Scan History

## 🚀 Getting Started

### Prerequisites

Install the following tools on Windows:

- [Flutter SDK](https://docs.flutter.dev/get-started/install/windows)
- [Android Studio](https://developer.android.com/studio)
- Android SDK
- [Git](https://git-scm.com/)

### Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/pathilalitha889-jpg/ClearCue.git
   ```

2. Open the project folder:

   ```bash
   cd ClearCue
   ```

3. Download dependencies:

   ```bash
   flutter pub get
   ```

4. Run the application on a connected Android device or running emulator:

   ```bash
   flutter run
   ```

### Build the Android APK

Generate a release APK using:

```bash
flutter build apk --release
```

After a successful build, the APK will be available at:

```text
build/app/outputs/flutter-apk/app-release.apk
```

Transfer the APK to your Android phone and install it. If prompted, allow installation from that source.

**Note:** The APK is generated on your local computer; it is not automatically included in the GitHub repository.

## 🔒 Data Storage

ClearCue uses a local SQLite database for its stored records. Database contents remain on the device unless additional synchronization functionality is implemented.

## 🎯 Project Objective

The objective of ClearCue is to make everyday information easier to understand through a mobile application that combines text recognition, structured information processing, and local data storage.

## 🔮 Future Enhancements

- Improve extraction and organization of important document details.
- Add deadline and key-information identification.
- Improve medicine information presentation and safety notices.
- Add support for more document formats and languages.
- Improve error handling and user experience.

## 👩‍💻 Developer

**Pathi Lalitha**

GitHub: [@pathilalitha889-jpg](https://github.com/pathilalitha889-jpg)

---

*ClearCue — Understand information before you act.*