# Crop Yield Prediction App

This is a Flutter-based mobile application that predicts crop yield using machine learning. The app uses a Flask API (deployed on PythonAnywhere) to handle ML model processing and also includes a chatbot feature.

## Features
- **Crop Yield Prediction** using a trained ML model.
- **Flask API Integration** for backend processing (hosted on PythonAnywhere).
- **Chatbot for User Assistance** as an additional feature.
- **User-friendly UI** for farmers and agricultural professionals.
- **Cross-platform Support** (Android & iOS).

## Prerequisites
Before running the project, ensure you have the following installed:
- Flutter SDK: [Install Flutter](https://flutter.dev/docs/get-started/install)
- Dart SDK (comes with Flutter)
- Android Studio / Visual Studio Code
- Emulator or a physical device
- Python (for local API testing)

## Setup and Installation
Follow these steps to set up the project:

### Flutter App Setup
1. **Clone the repository:**
   ```sh
   git clone https://github.com/Divyanand-L/Project-PayirseAI.git
   cd Project-PayirseAI
   ```
2. **Get dependencies:**
   ```sh
   flutter pub get
   ```
3. **Run the app:**
   ```sh
   flutter run
   ```

### Flask API Setup (Local Testing)
1. Navigate to the `backend` directory (if provided in the repository).
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the Flask API:
   ```sh
   python app.py
   ```
4. The API will be accessible at `http://127.0.0.1:5000`.

### PythonAnywhere Deployment (API Hosted Online)
- The Flask API is deployed on PythonAnywhere. Update the `baseUrl` in `lib/constants.dart` to match the hosted endpoint:
  ```dart
  const String baseUrl = "https://your-pythonanywhere-username.pythonanywhere.com";
  ```

## Dependencies
Ensure the following dependencies are added in `pubspec.yaml`:
```yaml
dependencies:
  flutter:
    sdk: flutter
  provider: ^6.0.5
  http: ^0.13.5
  flutter_bloc: ^8.1.2
```

Run the following command after modifying dependencies:
```sh
flutter pub get
```

## Machine Learning Model Integration
- The ML model is hosted on the Flask API, and predictions are retrieved via API requests.
- Modify the `baseUrl` in `lib/constants.dart` to point to the correct API endpoint.

## Chatbot Integration
- The chatbot is implemented in `lib/presentation/choose_module/pages/chat_bot/chat_bot.dart`.
- It interacts with predefined responses and may use API calls for dynamic responses.

## Running Tests
To run unit tests:
```sh
flutter test
```

## 📢 Featured on LinkedIn!
Check out our latest post about this project on LinkedIn:  
👉 [Read the post here](https://www.linkedin.com/posts/example-post-link)

## Contribution Guidelines
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`
3. Commit changes: `git commit -m 'Add new feature'`
4. Push to GitHub: `git push origin feature-branch`
5. Open a Pull Request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
**Developed by Divyanand L & Team** 🚀
