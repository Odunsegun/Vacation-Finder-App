# Vacation Finder App 🏖️

A cross-platform destination-discovery application built with Flutter and Dart. Vacation Finder combines interactive mapping, location search, saved places, community posts, and English/French localization.

> This was developed collaboratively as a university mobile-development project. My contributions focused on Firestore-backed post and location management, post update integration, and English/French localization.

## Features

- Search for destinations using Google Places
- Explore locations on an interactive OpenStreetMap-based map
- Access the device’s current location
- Display routes between the user and selected destinations
- Save and revisit places through Cloud Firestore
- Create and browse location-based community posts
- Store profile contact information locally using SQLite
- Switch between English and French

## Technology Stack

- Flutter and Dart
- Firebase Core
- Cloud Firestore
- Firebase Authentication
- `flutter_map` with OpenStreetMap tiles
- Google Places, Directions and Geocoding APIs
- Geolocator
- SQLite
- SharedPreferences


## Getting Started

### Prerequisites

- Flutter SDK
- Dart SDK
- Android Studio or Visual Studio Code
- An Android emulator or physical device
- Firebase CLI
- A Firebase project
- A restricted Google Maps Platform API key

### Clone the repository

```bash
git clone https://github.com/Odunsegun/Vacation-Finder-App.git
cd Vacation-Finder-App
```

### Install dependencies

```bash
flutter pub get
```

### Configure Firebase

```bash
firebase login
dart pub global activate flutterfire_cli
flutterfire configure
```

Select your Firebase project and desired platforms. Enable Cloud Firestore and Email/Password Authentication in the Firebase Console.

### Configure the Maps API key

Provide a restricted Google Maps Platform key at build time:

```bash
flutter run --dart-define=GOOGLE_MAPS_API_KEY=YOUR_RESTRICTED_KEY
```

Do not commit unrestricted API keys or service-account credentials.

### Validate the project

```bash
flutter analyze
flutter test
```

## My Contributions

- Implemented Firestore-backed post and location-management functionality
- Integrated post creation and update workflows
- Added and refined English/French localization
- Fixed integration issues across post, database and location components

The repository’s Git history preserves all team contributions.

## Current Limitations

- A configured Firebase project and Maps API key are required
- Map and place-search features require an internet connection
- Automated test coverage is limited
