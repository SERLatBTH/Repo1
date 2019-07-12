# Vive Port VR

This doument has instructions about how to assemble, operate, and use the Vive Port VR.
Vive Port is a VR device that can be connect to the pc and acts like a controller with monitor where you can use it in VR apps.


## Content

* [Where To Find](#where-to-find)
* [In The Box](#in-the-box)
* [How To Make It Works](#how-to-make-it-works)
  * [Assembly](#assembly)
  * [Charging The Batteries](#charging-the-batteries)
  * [Powering Up](#powering-up)
* [Device's Functionalities and Features](#devices-functionalities-and-features)
* [Safety Guidelines](#safety-guidelines)
  * [Environmental Consideration](#environmental-consideration)
  * [Operation](#operation)
  * [Pre-Flight Checklist](pre-flight-checklist)
* [SDK](#sdk)
* [Accessories](#accessories)
  * [DJI Goggles](DJIGoggles)
* [Putting The Device Back](#putting-the-device-back)
* [More Documentations](more-documentations)


## Where To Find
Lab - shelf lef1

## In The box
The box contains all the equipments which related to Vive Port VR. It has the box based on the steps. Step 1 is one big paper which introduces how to download and set up. Step 2-5 all is linked to different boxes. Below is the content list of the Vive-pro box.
1. Headset with headset cable
2. Controller (with lanyard) x2
3. Power adaper x2
4. Micro-USB cable x2
5. Earphone hole cap x2
6. Link box mounting pad
7. Cleaning cloth
8. Screws x4
9. Documentations (SteamVR tracking 2.0 Base Stations mounting guide with different languages*2)
![alt text](/images/Box.jpg)
![alt text](/images/orderOfContent.jpg)
![alt text](/images/ContentDetails.jpg)

## How To Make It Works

### Assembly

1. The initial setup for the device is already done
2. Take the VR main unit and connect it to the PC in the lab, with the compatible VIVE port.
3. Adjust the VR to the size of your head using the wheel on the back.

### Charging The Batteries

1. Use the micro USB cable  with the adapter to charge the controller.
2. No charging needed for the main unit.

### Powering Up

1. Power on the VR main unit using the power button on the left side, press and hold.
2. Power on the controllers using the system button (the small last button), press and hold.
3. Open the VR app or game and start navigating using the controllers.
4. You can adjust the volume using the buttons on the left side speaker.
5. To power off the controllers use the system button (the small last button)

## SDK

* The information regarding the SDK and the developer tool can be found on the [developer website](https://developer.vive.com/us/) for VIVE PRO.
* Supported platforms: PC, android and iOS.


### Become A Developer
1. To get started you need to first create an account on VIVE website using this [link](https://developer.viveport.com/console?__woopraid=hMlphcsTYmDy&_ga=2.12836916.248110000.1562852303-399269017.1562852303)
2. After creating an account and signing in go to the same [link](https://developer.viveport.com/console?__woopraid=hMlphcsTYmDy&_ga=2.12836916.248110000.1562852303-399269017.1562852303) and click become a developer.

### Getting Application Key
1. When signed in as developer you will find a menu on top with link "My Titles", click on it.
2. Create new submission by clicking on the target platform for the desired content home/arcade or education.
3. Type a name for the project and click next after agreeing on the terms.
4. Fill in the form with the required information

### VIVE Wave SDK

VIVE Wave™, an open platform and toolset that will enable easy Android™ Mobile VR content development and high-performance device optimization for third party partners. The VIVE Wave™ SDK offers an open interface enabling interoperability between numerous mobile VR headsets and accessories, supporting mainstream game engines.

Download the VIVE Wave SDK from [here](https://developer.vive.com/resources/knowledgebase/wave-sdk/).

The documentation you can find [here](https://hub.vive.com/en-US/profile/documents).

#### The key feature of VIVE Wave SDK
Key Features of VIVE Wave™

1. Cross Platform

   VIVE Wave™ runtime is a set of installable apk files supported on the platform with Android 7.1 or above. Users just need to install VIVE Wave™ apks on the VR devices and then can start to enjoy the VR world.

2. Less Customization

   VIVE Wave™ runtime exists on Android application layer and has no any proprietary customization in Android framework and BSP.

3. High Performance Mode

   VR devices just need to configure the specific CPU/GPU clock rate for Android VR mode and then VR devices just can get the high performance mode for VR rendering.

4. Standardized SDK interface

   VIVE Wave™ provides easy-use and practical SDK APIs for VR contents development. Developers just need to spend minimal effort to be able to easily port contents to VIVE Wave™.

5. Versatile VR Features Optimized for Mobile VR 

   * <20ms motion to photon latency
   * 3/6 DoF head and controller tracking
   * Stereo rendering with Asynchronous TimeWarp
   * Single buffer rendering with V-Sync scheduling
   * Columns or Rows strip rendering
   * Lens distortion correction and chromatic aberration correction
   * Tracking prediction
   * System 2D Overlay
   * Unity and Unreal Plugin support
   * Safety virtual wall
  
6. Various HMD Types Supported

   * Smartphone slot-in HMD
   * Smartphone tethered HMD
   * Standalone HMD
  
7. Open Interface for Device Plugin

   The vendors of VR accessory can easily develop their device service(driver) and plug in into VIVE Wave™ via apk installation. Per this way, VIVE Wave™ device can widely be expanded to fulfill the various demands of end users, such as: 3/6 DoF controller, Eye tracking, Hand tracking, and etc.

8. Qualcomm Snapdragon VR Embedded

   VIVE Wave™ is fully integrated with Qualcomm SVR to leverage the hardware optimization of powerful Snapdragon SoC for mobile VR.


#### Wave Native SDK

   VIVE Wave™ provides the native SDK for the native VR app development or third-party engine integration. The key features include VR device tracking and input, and VR stereo rendering.

#### Wave Unity SDK

   VIVE Wave™ provides the Unity SDK which fully integrated with VIVE Wave™ native runtime for Unity developers. Unity developers don’t need to take care the detailed VR affairs and can concentrate on VR content development.

#### Wave Unreal SDK

   VIVE Wave™ provides the Unreal SDK which fully integrated with Wave native runtime for Unreal development. Unreal developers don’t need to take care the detailed VR affairs and can concentrate on VR content development.

#### Wave PluginKit SDK

   The PluginKit SDK is provided to help developers design a VR DeviceService. It encapsulates the communication between a VIVE Wave™ Server and a VR DeviceService. It also provides mechanisms for defining data transmission.
   
   * The PluginKit has defined several interfaces to make it easier to develop drivers.
   * A VR DeviceService can currently send three types of data (pose, button, and analog) to VR apps.
   * When developing a VR DeviceService, you should define what role your device will play and what data type your device will send.
   * You can decide how to use the tracker. For example, you can use the Android™ sensor manager (sensor.TYPE_GAME_ROTATION_VECTOR) as tracking data, and send the data to the VR App so the tracker will move with the smartphone. Or you can use a different path for the tracker. For example, the path could be a circle or a line.
   * VRCameraInterface provides an interface to let developer customized their own camera device. Currently, we only support customized camera features on HMD.

#### Wave OEM SDK

   The VROEMservice SDK is provided to help developers design a VROEMService. It encapsulates the communication between a VIVE Wave™ Server and a VROEMService. It also provides mechanisms for defining data transmission and making VIVE Wave™ Server to act.
   
   * The VROEMservice defines several interfaces to make it easier to customize your own features.
   * A VROEMService can get information from VIVE Wave™ Server.
   * When developing a VROEMservice, you should implement the interface of IVROEMService and the interface of IVROEMService_api1.
   * You can design your own behaviors according the information that is transmitted from VIVE Wave™ Server.


### VIVE Sense SDK
This SDK is used to build applications for pc, it consists of multiple sub SDK that can be downloaded and used.

#### SRanipal SDK
  The SRanipal SDK allows developers to track and integrate users’ eye and lip movements, empowering developers to read intention and model facial expression. The SRanipal SDK includes the required runtime which runs in the notification tray to show the current eye tracking status for VIVE Pro Eye. Plugins for Unreal and Unity are included in the SRanipal SDK along with sample code for native C development. You can find more details [here](https://community.viveport.com/t5/Developer-Blog/Attention-Developers-VIVE-Pro-Eye-Has-Arrived/ba-p/31090?_ga=2.21629240.248110000.1562852303-399269017.1562852303)

  SRanipal SDK can be download from [here](https://developer.vive.com/resources/knowledgebase/vive-sranipal-sdk/)

#### VIVE Hand Tracking SDK
  A cross platform tool to track hand position and recognize gestures using the front camera(s) of the VIVE, VIVE Pro and the VIVE Focus (Wave Platform). Finger tracking (21 points) is available for the Vive and Vive Pro.

  VIVE hand tracking SDK can be downloaded from [here](https://developer.vive.com/resources/knowledgebase/vive-hand-tracking/)

  Detailed documentations and code samples can be found [here](https://developer.viveport.com/documents/sdk/en/vivehandtracking_index.html?_ga=2.8634422.248110000.1562852303-399269017.1562852303)

#### [SRWorks SDK](https://developer.vive.com/resources/knowledgebase/intro-vive-srworks-sdk/)
  SRWorks SDK With the launch of VIVE Pro, developers will now have access to the stereo front facing cameras to create new experiences that can mix the see-through stereo camera view and their virtual worlds. This will enable developers to perform 3D perception and depth sensing with the stereo RGB sensors, opening new worlds for more creative, interactive experiences.

  In addition to the updated OpenVR camera APIs that can now handle more than the mono camera of the original VIVE, the VIVE Software team is also providing developers with early access to the SRWorks SDK.

  SRWorks SDK can be downloaded from [here](https://developer.vive.com/resources/knowledgebase/intro-vive-srworks-sdk/)

#### [VIVE 3DSP SDK](https://developer.vive.com/resources/knowledgebase/about-vive-pro-sdks/)
  The VIVE 3D Sound Perception SDK provides a Unity compatible, audio spatialization plugin with the following features:

  * Higher Order Ambisonics
  * HRTFs based on refined real-world modeling (horizontally and vertically)
  * Support for Hi-Res audio source files and playback.
  * Acoustic distance effect with real-world modeling.

  The VIVE 3DSP plugin supports room effect, room reverberation and reflection, and acoustic occlusion that is tuned for the VIVE Pro. However the original VIVE and other HMDs and headphones are also supported.

  VIVE 3DSP SDK can be download from [here](https://developer.vive.com/resources/knowledgebase/vive-3dsp-sdk-2/)

  Detailed documentations and code samples can be found [here](https://developer.vive.com/resources/knowledgebase/about-vive-pro-sdks)
  

### VIVEPORT SDK

   Viveport is the official VR App Store, available in 60+ markets. VIVEPORT is compatible with a range of devices from HTC, other SteamVR devices, as well as devices from partner companies based on the WAVE runtime for all-in-one VR headsets.
   
   Download the VIVEPORT SDK from [here](https://developer.vive.com/resources/knowledgebase/viveport-sdk-download-2/).
   
   Dowenload the VIVEPORT Scene SDK from [here](https://developer.vive.com/resources/knowledgebase/download-viveport-scene-sdk/).

#### VIVEPORT SDK

Integrate your content with the VIVEPORT platform and utilize the store features.

When you publish your content to VIVEPORT, you can use the following features in your content if you integrate the VIVEPORT SDK into your content:

 1. Top Level
 2. DRM (Digitial Rights Management)
 3. Session Token
 4. User Profile
 5. In-App Purchase (IAP)
 6. Downloadable Content (DLC)
 7. Stats & Achievements
 8. Leaderboard
 9. Sessions (Per-round) for VIVEPORT Arcade (For Windows)

The VIVEPORT SDK consists of the components below:

 1. Client-side SDK
 2. VIVEPORT Desktop (For Windows) / VIVEPORT M (For Android)
 3. VIVEPORT cloud services
 4. ViVEPORT Switch Tool (For Windows Arcade development)
  
##### Introduction

* How Does the Client-Side SDK Work

  1. Users need to log in VIVEPORT Desktop by using their HTC Account (the account has owned this content) before launching the content.
  2. With the VIVEPORT SDK, the launched content can send a request to the VIVEPORT cloud services via VIVEPORT Desktop or Viveport App to check the user’s profile and licenses.
  3. The VIVEPORT cloud services return the user’s profile and licenses to client-side SDK for processing or verifying.
  4. The launched content may interact with the user through the user’s profile in VIVEPORT, or just check whether the user owns the content.

* VIVEPORT ID and VIVEPORT Key

  The VIVEPORT SDK uses VIVEPORT ID and VIVEPORT Key to communicate with the VIVEPORT platform.VIVEPORT ID and VIVEPORT Key is on the VIVEPORT Listing page.

  1. Before content can be published to VIVEPORT, the content must have a unique VIVEPORT ID and VIVEPORT Key.
  2. The VIVEPORT ID and VIVEPORT Key can be requested from the VIVEPORT developer portal at [here](https://developer.viveport.com/console).
  3. The VIVEPORT ID and VIVEPORT Key must be included in the authentication script before attempting to publish the content on VIVEPORT.

* System Requirements

  * Software Requirements
   1. Unity 5.x for Windows (32/64-bit)
   2. Unreal Engine 4.x for Windows (64-bit, Visual Studio 2013)
   3. VIVEPORT Desktop - You can download whole Vive Software since it includes VIVEPORT Desktop.
   4. VIVEPORT M - You can download whole Vive App from your Android.

  * Runtime Environment
   1. For Windows, standalone applications for Windows 7/8/10 (32/64-bit) are supported.
   2. For Android, standalone app from Android version 4.1 with Gyroscope (minimum) to Android version 6 or later with 4G RAM and 1440p resolution (high standard) are supported.

* SDK Usage Outline

  Before publishing your content to VIVEPORT, you can (and should) check if the DRM license generated from VIVEPORT cloud services is valid, and then test whether other SDK functions work. The steps below outline the process of integrating the VIVEPORT SDK.

  For Unity user:

   1. Create or import your content into Unity
   2. Download and install the VIVEPORT SDK
   3. Integrate the VIVEPORT SDK into your content in Unity

  For Unreal user:

   1. Create or import your content into Unreal
   2. Download and install the VIVEPORT SDK
   3. Integrate the VIVEPORT SDK into your content in Unreal

  For C# user:

   1. Create an empty C# project in your visual studio 2015
   2. Copy settings into your project
   3. Reload your project and rebuild

* API

 It has 9 different type of APIs. They are [Top Level API](https://developer.viveport.com/documents/sdk/en/api_top.html), [DRM API](https://developer.viveport.com/documents/sdk/en/api_drm.html), [Session Token API](https://developer.viveport.com/documents/sdk/en/api_token.html), [User Profile API](https://developer.viveport.com/documents/sdk/en/api_userprofile.html), [In-App Purchase (IAP) API](https://developer.viveport.com/documents/sdk/en/api_iap.html), [Deeplink API](https://developer.viveport.com/documents/sdk/en/api_deeplink.html), [Downloadable Content (DLC) API](https://developer.viveport.com/documents/sdk/en/api_dlc.html), [Stats & Achievements API](https://developer.viveport.com/documents/sdk/en/api_stats.html) and [Leaderboards API](https://developer.viveport.com/documents/sdk/en/api_leaderboard.html). The details of how to use them and the examples can be found by click the name.

* Integration 

 Here is the guideline of how to integrate your content with the VIVEPORT platform.
  1. Integration with [Unity](https://developer.viveport.com/documents/sdk/en/unity.html).
  2. Integration with [Unreal Engine](https://developer.viveport.com/documents/sdk/en/unrealengine.html).
  3. Integration with [C#](https://developer.viveport.com/documents/sdk/en/csharp.html).
  4. Integration with [C++](https://developer.viveport.com/documents/sdk/en/cplus.html).

#### VIVEPORT ARCADE SDK

* ViveportSwitch tool

 For developers who want to develop for the Arcade program, you can use this tool to simulate Arcade mode in your computer, and integrate VIVEPORT SDK in the Arcade mode.

  1. When you upload your title, opt-in to the VIVEPORT Arcade Program by checking one of the options in the VIVEPORT Arcade Program section.

  2. Download and install the VIVEPORT SDK from the [Download page](https://developer.viveport.com/documents/sdk/en/download.html#down-latest-viveport-sdk).

  3. Unzip the package and find the ViveportSwitch.exe tool.

  4. Open the ViveportSwitch.exe tool and select VIVEPORT Arcade, then click the Switch button.

  5. After switching to VIVEPORT mode, the VIVEPORT service will be restarted. You must re-launch VIVEPORT on your desktop before continuing development.

 The details of its API and integration, you can found [here](https://developer.viveport.com/documents/sdk/en/viveportarcadesdk.html).

#### VIVEPORT Scene SDK  

 Help you create immersive VR Previews that will be showcased in VIVEPORT.

 Required files:

  You will need to go to [https://developer.vive.com/](https://developer.vive.com/) to register or sign in if you have an existing account.

  Download the vr preview scene sdk [here](https://developer.viveport.com/documents/sdk/en/download_scenesdk.html)

 Required Hardware:

  A Vive and Vive controllers setup and working.

 The detailed tutorial can be found [here](https://developer.viveport.com/documents/sdk/en/scenesdk_tutorial.html).

#### VIVE HAND TRACKING SDK

 * Introduction

   Vive Hand Tracking SDK is aimed to provide:

    * First-person view hand recognition in VR/AR/Phones
    * Provide accurate, low-latency, deep learning-based solution.
    * Support different hardware & operation systems.
    * Use existing camera modules, no extra hardware needed.
    * Recognises static gestures, instead of gesture sequences.

 * Supported Operation Systems & Hardware

  Vive Hand Tracking SDK tries our best to support all VR/AR devices with camera on-board. A list of currently supported devices is listed below:

 | Operation Sytem  | Aarchitecture | Hardware |
 | --- | --- | --- |
 | Windows 7 or newer  | x86-64 | HTC Vive, HTC Vive Pro |
 |  Android N or newer |  ARMv7, ARMv8 | Android Phone with optional VR headset|
 | Android (WaveVR) | ARMv7	| HTC Vive Focus, HTC Vive Focus Plus |

 For detailed requirements for each OS/hardware, please see [Supported Hardware](https://developer.viveport.com/documents/sdk/en/overview/hardware.html).

 * Supported Features

   Vive Hand Tracking SDK supports:

    * Left/Right hand detection
    * Pre-defined gesture classification
    * Different modes for hand position result (restricted by OS/hardware capability)
   For detailed feature for each OS/hardware, please see [Available Features](https://developer.viveport.com/documents/sdk/en/overview/feature.html).

 * Available Plugins

 | Plugin Type | Supported Platforms |	Requirements |
 | ---- | --- | --- |
 | [Unity](https://developer.viveport.com/documents/sdk/en/unity/index.html) |	All	| Unity 5.4 or newer (Android armv8 requires 2017.4+) |
 | [Unreal](https://developer.viveport.com/documents/sdk/en/unreal/index.html) |	All |	Unreal 4.20 or newer |
 | [Android Library](https://developer.viveport.com/documents/sdk/en/android/index.html) |	Android, WaveVR |	Java 8 or newer |
 | [C/C++](https://developer.viveport.com/documents/sdk/en/capi/index.html) |	All |	c/c++ compiler (MSVC or Android NDK) |

 The details guide you can find [here](https://developer.viveport.com/documents/sdk/en/vivehandtracking_index.html).

#### VIVEPORT AirSig SDK

 This document will help you to integrate your content with the VIVEPORT AirSig gesture and signature recognition.

 * Usage Cases
 
  VIVEPORT AirSig Manager provides 4 major functions:

  * Player’s Signatures:

   Identify player’s identity by verifying against Player’s Signatures with adjustable signature strength.

  * Developer-defined Gestures:

   Identify input gestures against Developer-defined Gestures. The feature is:

   * Developers customize and define gestures. Players don’t have to train.
   * With high generality. Even different players with different drawing habit(e.g. different size, shape), system can recongnize it.
   * In order to use this feature, gestures sample must be collected first and then generate a gesture profile in AirSig Developer Portal , or developers can use the gesture profile generated by others.

  * Player-defined Gestures:

   Learn and identify Player-defined Gestures. The feature is:

   * Players can create their own gestures in application real-time.
   * The training progress is needed. Players have to repeat the same gesture for about 5 times.
   * This kind of gesture focus on the drawing feature of individual. Less likely to be shareable between players.

  * Smart Gesture:

   Smart Gesture algorithm that combines the result of Developer-defined Gestures and Player-defined Gestures (2 and 3). The feature is:

   * Developers define the gesture and design a “Tutorial phase” in application. Players have to repeat the gesture and system learns the drawing habit in the same time. The accuracy is further improved.
   * In “Tutorial phase”, if the players’ drawing habit is very different from the gestures defined by developers, system will not learn it. That can avoid the wrong gesture affects the recognition result.
   * We suggest developers use this mode in most scenario. Players usually don’t familiar with using gestures. The “Tutorial phase” helps players practice it and system can learn the drawing habit in the same time.

* System Requirements

  * Software Requirements

   * .Net Framework 4.6.1 - for Windows.
   * Microsoft Visual C++ 2017 Redistributable (x64) for Windows (64-bit)
   * Unity v5.6 or above version.
   * HTC Wave SDK for Android.

 * Runtime Environment

   * For Windows, standalone applications for Windows 7/8/10 (32/64-bit) are supported.
   * For Android, standalone app from Android version 4.1 with Gyroscope (minimum) to Android version 6 or later with 4G RAM and 1440p resolution (high standard) are supported.

 * Installation

 VIVEPORT AirSig supports Vive and Wave. Please refer to [AirSig](http://www.airsig.com/vr/) for installation.

 * API and Integration
 
 It has two APIs which are [Method](https://developer.viveport.com/documents/sdk/en/viveport_airsig_api_method.html) and [Event Delegates](https://developer.viveport.com/documents/sdk/en/viveport_airsig_api_eventdelegates.html). The way of integration with Unity can be found [here](https://developer.viveport.com/documents/sdk/en/viveport_airsig_unity.html).
