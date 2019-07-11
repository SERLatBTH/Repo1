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

#### Introduction
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

#### Different type of VIVE Wave SDK

1. Wave Native SDK

VIVE Wave™ provides the native SDK for the native VR app development or third-party engine integration. The key features include VR device tracking and input, and VR stereo rendering.

2. Wave Unity SDK

VIVE Wave™ provides the Unity SDK which fully integrated with VIVE Wave™ native runtime for Unity developers. Unity developers don’t need to take care the detailed VR affairs and can concentrate on VR content development.

3. Wave Unreal SDK
VIVE Wave™ provides the Unreal SDK which fully integrated with Wave native runtime for Unreal development. Unreal developers don’t need to take care the detailed VR affairs and can concentrate on VR content development.

4. Wave PluginKit SDK

The PluginKit SDK is provided to help developers design a VR DeviceService. It encapsulates the communication between a VIVE Wave™ Server and a VR DeviceService. It also provides mechanisms for defining data transmission.
 * The PluginKit has defined several interfaces to make it easier to develop drivers.
 * A VR DeviceService can currently send three types of data (pose, button, and analog) to VR apps.
 * When developing a VR DeviceService, you should define what role your device will play and what data type your device will send.
 * You can decide how to use the tracker. For example, you can use the Android™ sensor manager (sensor.TYPE_GAME_ROTATION_VECTOR) as tracking data, and send the data to the VR App so the tracker will move with the smartphone. Or you can use a different path for the tracker. For example, the path could be a circle or a line.
 * VRCameraInterface provides an interface to let developer customized their own camera device. Currently, we only support customized camera features on HMD.

5. Wave OEM SDK
The VROEMservice SDK is provided to help developers design a VROEMService. It encapsulates the communication between a VIVE Wave™ Server and a VROEMService. It also provides mechanisms for defining data transmission and making VIVE Wave™ Server to act.
 * The VROEMservice defines several interfaces to make it easier to customize your own features.
 * A VROEMService can get information from VIVE Wave™ Server.
 * When developing a VROEMservice, you should implement the interface of IVROEMService and the interface of IVROEMService_api1.
 * You can design your own behaviors according the information that is transmitted from VIVE Wave™ Server.

