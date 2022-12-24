# ReVanced Extended Magisk Module
[![Build Modules](https://github.com/MatadorProBr/revanced-extended-magisk-module/actions/workflows/build.yml/badge.svg)](https://github.com/MatadorProBr/revanced-extended-magisk-module/actions/workflows/build.yml)
[![CI](https://github.com/MatadorProBr/revanced-extended-magisk-module/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/MatadorProBr/revanced-extended-magisk-module/actions/workflows/ci.yml)

You can get the [latest CI release from here](https://github.com/MatadorProBr/revanced-extended-magisk-module/releases).

[**mindetach module**](https://github.com/j-hc/mindetach-magisk) in the releases section detaches YouTube and YouTube Music from Play Store and blocks it from updating them.

## Features
 * Can build Magisk modules or non-root APKs
 * Updated every hour with the latest versions of apps and patches in accordance with your configuration
 * Cleans APKs from unneeded libs to make them smaller
 * Fully open-source, every binary or APK is compiled without human intervention
 * Modules
     * recompile invalidated odex for YouTube and Music apps for faster usage
     * receive updates from Magisk app
     * do not break safetynet or trigger root detections used by certain apps
     * handle installation of the correct version of the stock app and all that
     * mount the patched app immediately without needing to reboot

#### **Note that the [CI workflow](../../actions/workflows/ci.yml) is scheduled to build the modules and APKs every hour if there is a change. You may want to disable it.**

## To include/exclude patches
[**See the list of patches**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-patches)

 * Star the repo :eyes:
 * [Fork the repo](https://github.com/MatadorProBr/revanced-extended-magisk-module/fork) or use it as a template
 * Edit the patcher args in [`build.conf`](./build.conf)
 * Run the [workflow](../../actions/workflows/build.yml)
 * Grab your modules from [releases](../../releases)

To be able to use non-root variants of YT and YT Music you will need to install [Vanced Extended MicroG](https://github.com/inotia00/VancedMicroG/releases) (recommended) or [Vanced MicroG](https://github.com/TeamVanced/VancedMicroG/releases).

# Building Locally
Make sure you have JDK 17 installed. Then run:

```console
$ git clone --recurse-submodules https://github.com/MatadorProBr/revanced-extended-magisk-module
$ cd revanced-extended-magisk-module
$ ./build.sh build
```
