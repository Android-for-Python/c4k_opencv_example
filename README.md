Camera4Kivy OpenCV Example
==========================

*OpenCV Image Analysis using Camera4Kivy.*

# Overview

Uses OpenCV to edge detect the image stream, and replaces the usual Preview image with the detection result.

Available on most of the [usual platforms](https://github.com/Android-for-Python/Camera4Kivy/#tested-platforms).

On a desktop the example assumes a builtin camera facing the user, so the Preview is mirrored. If you want to point a freely mounted camera you may want to set the [Camera4Kivy mirror option False]((https://github.com/Android-for-Python/Camera4Kivy/#mirror)). 

The example demonstrates basic usage of the image analysis api. Analyzing image frames, annotating the results to the Preview (including when mirrored), and interacting with the annotation.

# Install

This example depends on Camera4Kivy. **[Read about Camera4Kivy](https://github.com/Android-for-Python/Camera4Kivy#camera4kivy)** because, depending on the platform you may need to install a [camera provider](https://github.com/Android-for-Python/Camera4Kivy#dependencies). 

## Windows, MacOS

`pip3 install opencv-python camera4kivy`

## Linux

`sudo apt-get install libatlas-base-dev`

`pip3 install opencv-python camera4kivy`

## Android

Camera4Kivy depends on the 'master' version of Buildozer. Currently `1.2.0.dev0`

`pip3 install git+https://github.com/kivy/buildozer.git`

The example includes a [camera provider](https://github.com/Android-for-Python/camera4kivy#android-camera-provider) and a [buildozer.spec](https://github.com/Android-for-Python/camera4kivy#buildozerspec).



