# EdgeDetectionApp
Real-time Android edge detection using CameraX + OpenCV


A real-time edge detection Android app using CameraX and OpenCV with native (JNI) support.

1. Features Implemented
2. Real-time camera preview using CameraX
3. Live edge detection using OpenCV (Canny)
4. Save processed image to gallery
5. Runtime permission handling (Camera, Storage)
6.OpenCV initialized in Java (can be expanded to C++)

#Setup Instructions

Prerequisites
Android Studio Hedgehog (or latest)
Android SDK 31+
NDK 23+
OpenCV Android SDK (4.5.5+

#Dependencies

implementation("androidx.camera:camera-camera2:1.3.0")
implementation("androidx.camera:camera-lifecycle:1.3.0")
implementation("androidx.camera:camera-view:1.3.0")
implementation("org.opencv:opencv-android:4.5.5")


Add OpenCV SDK

1.Download OpenCV Android SDK from opencv.org
2.Copy OpenCV-android-sdk/sdk/native/libs to your jniLibs/ folder
3.Load OpenCV using:
if (!OpenCVLoader.initDebug()) {
    Log.e("OpenCV", "Initialization failed");
} else {
    Log.d("OpenCV", "OpenCV loaded successfully");
}

NDK Setup
Install NDK from SDK Manager > SDK Tools > NDK
CMake version: >=3.22.1


