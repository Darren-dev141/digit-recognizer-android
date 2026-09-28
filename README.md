# Digit Recognizer (Android)

An Android app that recognizes handwritten digits. Draw a digit on the canvas and the app classifies it on-device with a TensorFlow Lite model.

## How it works

- `MainActivity.java` captures the drawing from a `FingerPaintView`, downscales it to 28×28, and feeds it into a bundled `digit.tflite` model (MNIST-style, 10 output classes).
- The predicted digit is shown as text; a clear button resets the canvas.

## Build

Open in Android Studio (or run `./gradlew assembleDebug`). The model file lives in `app/src/main/assets/digit.tflite`.

## Stack

Java, Android SDK, TensorFlow Lite, FingerPaintView
