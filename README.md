# idental

# Dental Diseases Detector
A Flutter app that detects a dental diseases given either an panoramic x-ray or normal images.
# DEMO
 https://drive.google.com/file/d/1Z4Q9t0MZT02TbLyZCGbBsSAxLZqTmor8/view?usp=sharing

## Requirements
- Any operating System (ie. MacOS X, Linux, Windows)
- Any IDE with latest Flutter SDK installed (ie. IntelliJ, Android Studio, VSCode etc)
- A little knowledge of Dart and Flutter.

## Additional Info
Packages used include: tflite, pytorch, image_picker, provider,flutter_local_notification, flutter bloc , firebase_core, firebase_messaging.
Model used and labels file are found in the <i>assets/model</i> folder. 

## Installation
A Flutter installation is required to run this project.
To install Flutter, visit the official installation [documentation](https://docs.flutter.dev/get-started/install).
Set up an editor of choice as specified [here](https://docs.flutter.dev/get-started/editor).


```

Run the below command inside the project directory to install necessary packages.
```bash
flutter pub get
```
To run the project in debug mode 
```bash
flutter run
```
To generate a release build
```bash
flutter build apk
```
Locate the `app-release.apk` file from the directory `build/app/outputs/flutter-apk/` and install in your Android smartphone or emulator to use.

## Usage

On launching the application, you will be able to select one dental disease from the available dental diseases, then take a photo , or select a photo from your gallery.

The application then runs the TFLITE model in the background to get the diagnosis result.


## Important to note
- The `periodontal tflite` model has been trained to detect panoramic x-ray images and label it as periodontal or non periodontal
- The `Oral cancer tflite` model has been trained to detect normal images and label it as cancer or non cancer
- The `Multi disease pytorch` model has been trained to detect panoramic x-ray images and label it as 
  - cavity
  - infected teeth
  - impacted teeth
  - filling
  - implant
    
