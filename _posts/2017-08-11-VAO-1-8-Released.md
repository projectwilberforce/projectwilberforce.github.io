---
title:  "Volumetric Ambient Occlusion v1.8 released"
date:   2017-11-08 17:36:42
categories: unity plugin
excerpt: "Fixed aliasing problem (jaggy edges) in single pass stereo mode"
tags: [vao, new releases, ssao, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

# {{page.title}}

![]({{site.baseurl}}/images/vao18/fixed-jaggy-edges.jpg)

We've managed to fix aliasing artifact that occured in newest Unity versions when using single pass stereo mode (VR).

Problem occured when running post processing effects via command buffers due to incorrect information about actual screen texture size passed from Unity. It did not take into account extra texture width needed to render two eyes simultaneously. Result was that effect was rendered in only half the resolution in horizontal dimension and then stretched which created jaggy edges in one direction only. 

To try it, just [download free demo](https://projectwilberforce.github.io/vaodemo/) with watermark, or get full version at [Unity Asset Store](http://u3d.as/xzs)


## Additional information

See [documentation here](https://projectwilberforce.github.io/vaomanual/) and [forum here](https://forum.unity3d.com/threads/volumetric-ambient-occlusion-image-effect.428426/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>
