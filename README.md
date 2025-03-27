# Fundamental Firebase

Firebase is a powerful backend-as-a-service (BaaS) platform developed by Google, designed to help developers build, improve, and grow their applications. When combined with Flutter, Google's UI toolkit for building natively compiled applications for mobile, web, and desktop from a single codebase, Firebase becomes an indispensable tool for creating modern, scalable, and feature-rich apps.

Caption: **Unlock the Power of Real-Time Data and Backend Services with Firebase and Flutter!**

# Tech Stack **👩‍💻**

- Flutter (Framework)
- Dart (Language)
- Firebase (Cloud Database)

# Package 📦

- firebase_core
- cloud_firestore
- uuid
- firebase_storage

# Step 📦

Install Firebase Tools global in our device using terminal

```
npm install -g firebase-tools
```

Login our Firebase.

```
firebase login
```

Install FlutterFire CLI.

```
dart pub global activate flutterfire_cli
```

Go to project folder and configure FlutterFire. Every single project has different name.

```
flutterfire configure --project=fir-tutorial-7cd0a
```

To initialize Firebase, call `Firebase.initializeApp` from the `firebase_core` package with the configuration from your new `firebase_options.dart` file:

```dart
import 'package:firebase_core/firebase_core.dart';
import 'firebase_options.dart';

// ...

await Firebase.initializeApp(
    options: DefaultFirebaseOptions.currentPlatform,
);
```
