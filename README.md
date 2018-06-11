# GearVR GDNative plugin for Godot

*WIP* This is an unfinished work in progress repository, it requires a few unsubmitted changes in the core of Godot. Check back here soon when we're a little further along!

This repository contains the source code for the GearVR plugin for Godot.
See demo project as an example for how to use the plugin

This is an Android only plugin that only works on suitable GearVR capable phones!
Currently only the HMD is handled!

License
-------
Please check the GearVR SDK for license information in relation to the GearVR SDK used in this project.
The rest of this project is released under a MIT license.

Compiling
---------
In order to compile this plugin you first need to download the GearVR SDK from the Oculus developer website.
You will also need the Android NDK(Make sure it's in your PATH variable) and JDK.

After cloning this repository make sure to initialise the submodules with `git submodule init`
When you've pulled a newer version make sure to run `git submodule update`

Next, modify the jni/Android.mk by adding the respective paths. Alternatively, you can add them to path and call using $(Var_Name).

Then run `ndk-build NDK_LIBS_OUT=./demo/addons/godot_gearvr/bin`
