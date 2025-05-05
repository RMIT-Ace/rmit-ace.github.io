---
layout: post
title: "Porting Unity Apps to Vision Pro"
---

| Unity App Running On VisionPro | Unity Windowed App Vs Native visionOS App |
| --- | --- |
| [![Unity App on Vision Pro in Windowed Mode](https://img.youtube.com/vi/ZqEk3z4zkpg/default.jpg)](https://youtu.be/ZqEk3z4zkpg) | [![Unity App on Vision Pro in Windowed Mode](https://img.youtube.com/vi/gFS8nQsvod0/default.jpg)](https://youtu.be/gFS8nQsvod0) |
| Feature Unity app running on Vision Pro in 2D mode | In comparision, the above video shows native visionOS app utilising all 3 modes: Window, Volume, and Immersive space |

I have successfully porting Unity projects to Vision Pro. In this first-round attempt, it was a 1-to-1 porting usig Unity provided Build Profiles, with no modification to the source code. Here are some of my observation:

- with the provided Build Profiles (visionOS, iOS, macOS), Unity project is ported to run in Vision Pro in "Windowed" mode. The ported app runs in "flat" 2D views on Vision Pro

- The gameplay works with external bluetooth keyboard wirelessly connected to Vision Pro. With no modification to the source code, Unity app cannot interact with visionOS's gesture controls (eye or hands gestures)

- The generated source codes are C++ - not Swift/SwiftUI. Modifying the generated source code directly from Xcode is NOT convenient and not recommended as they will be overwritten the next time the project is ported again.

<!--more-->

# R&D Plan

![](https://github.com/RMIT-Ace/VisionPro-Research/blob/main/res/vision-arch.png)

1) Research into Unity' Poly Spatial technology and create 3D volume and immersive features
2) Research how to access Vision Pro's gesture control from Unity app