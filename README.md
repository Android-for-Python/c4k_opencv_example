Camera4Kivy OpenCV Example
==========================

*OpenCV Image Analysis using Camera4Kivy.*

# Overview

Uses OpenCV to edge detect the image stream, and replaces the usual Preview image with the detection result.

Available on the [usual platforms](https://github.com/Android-for-Python/Camera4Kivy/#tested-platforms).

# Install

A prerequisite is a working camera installed and seen as device '0'. Test this with the platform's camera app before proceeding.

This example depends on Camera4Kivy. **[Read about Camera4Kivy](https://github.com/Android-for-Python/Camera4Kivy#camera4kivy)** because, depending on the platform you may need to install a [camera provider](https://github.com/Android-for-Python/Camera4Kivy#dependencies). 

Assuming you have installed a camera provider (if necessary):

## Windows, MacOS

`pip3 install opencv-python camera4kivy`

## Linux

`sudo apt-get install libatlas-base-dev`

`pip3 install opencv-python camera4kivy`

## Android

Camera4Kivy depends on the 'master' version of Buildozer. Currently `1.2.0.dev0`

`pip3 install git+https://github.com/kivy/buildozer.git`

The example includes a camera provider and a buildozer.spec

For any other project, follow the [camerax_provider install instructions](https://github.com/Android-for-Python/Camera4Kivy#candroid-camerax_provider)

And the following **must** be in the buildozer.spec:

`requirements= python3,kivy, opencv, camera4kivy`

`android.permissions = CAMERA`

`android.api = 30`  or greater (min 29)

`p4a.local_recipes = ./camerax_provider/recipes`

`p4a.hook = ./camerax_provider/gradle_options.py`   

# Other Stuff

On a desktop the example assumes a builtin camera facing the user, so the Preview is mirrored. If you want to point a freely mounted camera you may want to set the [Camera4Kivy mirror option False]((https://github.com/Android-for-Python/Camera4Kivy/#mirror)). 

The example demonstrates basic usage of the image analysis api. Analyzing image frames, annotating the results to the Preview (including when mirrored), and interacting with the annotation.

