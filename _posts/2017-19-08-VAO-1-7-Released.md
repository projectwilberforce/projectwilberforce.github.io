---
title:  "We're releaseing Volumetric Ambient Occlusion Unity Plugin v1.7"
date:   2017-08-19 17:36:42
categories: unity plugin
excerpt: "Improved occlusion in great distances (suitable for exterior scenes), controls to limit radius near camera, fade occlusion in the distance and bugfixes in Unity integration"
tags: [vao, new releases, ssao, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

# {{page.title}}

![]({{site.baseurl}}/images/vao17/vao_1_7.jpg)

In this release we focused on improving visual quality and adding new controls. Based on the feedback from our users we have added:

- **Controls to limit AO radius** near camera to certain size wrt. the screen. This is to prevent performance loss when radius grows very large after perspective projection to the screen for nearby objects.
- Controls to gradually **fade occlusion** in the distance
- **"Same color suppresion"** for color bleeding - this is supposed to prevent bleeding colors of same hue to each other (as it oversaturates colors and looks unrealistic)

We have also fixed some issues from previous versions:

- **Far plane source control** - this will take information about far plane setting either from "ProjectionParams" variable provided by Unity or directly from camera object. As we had flickering issues with Temporal Antialiasing in Unity's Post Processing Stuck we had to change our implementation to support also second setting - from camera.
- We've **improved precision** of our algorithm so it now creates detailed occlusion also far away from camera in great distances  
- **Intermediate Texture Format** - used by command buffer implementation to decide what texture format to use to mix VAO with the scene. Auto setting is recommended but you can choose any format if you run into issues, especially with HDR rendering.
- Fixed **flipping image upside down** in new Unity versions - this happens every other Unity release and we keep fixing it constantly

To try it, just [download free demo](https://projectwilberforce.github.io/vaodemo/) with watermark, or get full version at [Unity Asset Store](http://u3d.as/xzs)

![]({{site.baseurl}}/images/vao17/vao-1-7-fix.jpg)


## Additional information

See [documentation here](https://projectwilberforce.github.io/vaomanual/) and [forum here](https://forum.unity3d.com/threads/volumetric-ambient-occlusion-image-effect.428426/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>
