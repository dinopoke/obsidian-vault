---
title: Unreal VR Notes
tags:
  - unreal
  - vr
  - notes
created: 2026-11-24T00:14:00
---




[https\://docs.unrealengine.com/latest/INT/Platforms/VR/CheatSheet/index.html](https://docs.unrealengine.com/latest/INT/Platforms/VR/CheatSheet/index.html)

[https\://docs.unrealengine.com/latest/INT/Platforms/VR/ContentSetup/index.html](https://docs.unrealengine.com/latest/INT/Platforms/VR/ContentSetup/index.html)

* Set up Chaperone  
* Make new bindings  
* Extend from the interface  
* Allow CPU access for mesh

* Turn off post processing  
* Objects are best viewed when they are 0.75 \- 3.5 metres away  
  * In Unreal, 1 UU \= 1 cm  
* Three kinds of tests  
  * Fresh for motion sickness  
  * General players  
  * Developers \- Worst Test subjects because they are used to VR  
* Target 90 FPS Min, 120 FPS Ideal  
* Minimize 360 motion  
* Avoid Cinematic Cameras \- don’t take camera control away from player  
* Don’t override FOV  
* No Walking Bob  
* No Camera Shake  
* Close the **clipping plane**  
* Dim lights  
* Avoid Stairs and use lifts  
* Start moving at full speed. Constant rate of acceleration.   
* Don’t use DOF or Motion Blur  
* \-simulatestereo test as VR

Forward Rendering may be better than Deferred Renderer (default)

Numbers

* Character Size  
  * VR Height \- 176 cm  
  * VR Width \- 68 cm  
  * Character \!= Player Height  
* Movements Speed  
  * 24 m/s  
* Camera Location  
  * 160 cm  
  * 

Content

* SCALE  
* No Normal Maps  
  * Parallax Occlusion Mapping instead  
  * Tessellation  
* Be careful of removing faces  
* Use Static Lighting and Lightmaps  
  * Minimize dynamic lighting  
    * Never Touch one another  
* Some VFX like smoke and fire don’t work in VR  
* Transparency is expensive  
  * Use DitherTemporalAA  
* Fake everything  
* Use Reflection Probes instead of Screen Space Reflections

* Increase r.screenpercentage as much as you can  
* Stat\_unit \- profiling FPS

* Instant Stereo Rendering  \-renders both eyes in one pass  
* Flipbooks don’t work  
* Nick Whiting to Occulus \- VP Settings  
* Keep horizon Level  
* VR games are about the manipulation of objects