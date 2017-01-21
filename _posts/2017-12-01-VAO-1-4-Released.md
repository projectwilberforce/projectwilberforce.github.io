---
title:  "Volumetric Ambient Occlusion Unity Plugin v1.4 has been released + DEMO"
date:   2016-01-21 18:36:42
categories: unity plugin
excerpt: "New version includes color bleed and various speed optimizations."
tags: [vao, new releases, ssao, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

## {{page.title}}

Another new version of our VAO has been released! We have both added new features and optimized the existing ones.

VAO is our answer to ambient occlusion problem. It has better performance and visual quality than other SSAO solutions. 

Download [free demo](https://projectwilberforce.github.io/vaodemo) and buy at [Unity Asset Store](http://u3d.as/xzs)

![]({{site.baseurl}}/images/social-vao-heading.jpg)

## What's new in v1.4  

 * [Downloadable demo here](https://projectwilberforce.github.io/vaodemo)
 * *Color bleed* mode
 * *Presence* option to make effect more pronounced without increasing radius (which means no additional performance hit)
 * *Speed Boost* experimental optimization feature
 * More *Quality* options

## About VAO

VAO works by approximating amount of light that can reach given pixel taking volume of surrounding geometry into account. We have developed fast approximation algorithm and use fine-tuned random samples sets to calculate it in real time. Ambient occlusion will add depth and realism to your scenes.

Our algorithm works in screen space (using only normals and depth values readily available in G-Buffer). Therefore, there is no performance hit when using more complicated meshes (more polygons) and it makes use of bump textures automatically. It is also fully dynamic - there is no need for pre-calculating specific scenes and it works with both static and moving objects.

In the newest version, we added color bleed option. This means that on top of shadows the surfaces now cast their color onto their surroundings. We also 

See [documentation here](https://projectwilberforce.github.io/vaomanual/) and [forum here](https://forum.unity3d.com/threads/volumetric-ambient-occlusion-image-effect.428426/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>

## Performance tips

- Judge the quality by the final image, not AO only.
- For the best results set *Radius* so the shadow created by the effect is around 10-20cm (4-8in).
- To make AO effect more pronounced increase *Presence* and *Power* settings before increasing *Radius*.
- Use appropriate number of samples (*Quality* setting) - high enough to hide aliasing.
- Consider using *Downsampling* at high screen resoltions.
- Use *Speed Boost* feature (currently experimental.)