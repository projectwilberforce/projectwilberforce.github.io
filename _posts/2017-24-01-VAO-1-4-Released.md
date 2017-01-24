---
title:  "Volumetric Ambient Occlusion Unity Plugin v1.4 has been released + DEMO"
date:   2017-01-24 17:36:42
categories: unity plugin
excerpt: "New version includes color bleed and various speed optimizations, improved image quality and more controls."
tags: [vao, new releases, ssao, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

## {{page.title}}

Another new version of VAO (our SSAO plugin) has been released! We have both added new features and optimized the existing ones. New demo has also been released.

<a href="https://projectwilberforce.github.io/vaodemo/" class="downloadbtn">Download Free Demo</a>

Get full version at [Unity Asset Store](http://u3d.as/xzs)

![]({{site.baseurl}}/images/space_age.png)

## What's new in v1.4  

 * *Color bleed* mode
 * *Presence* option to make effect more pronounced without increasing radius (which means no additional performance hit)
 * *Speed Boost* experimental optimization feature
 * More *Quality* options
 
<iframe frameborder="0" class="juxtapose" width="100%" height="380" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=d1d18d1e-e259-11e6-8b75-0edaf8f81e27"></iframe>

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


<div>
<div class="img-thumb">
	<a href="{{site.baseurl}}/images/screenshots/e1.png" data-lightbox="vao"><img src="{{site.baseurl}}/images/screenshots/e1_thumb.png" /></a>
</div>
<div class="img-thumb">
	<a href="{{site.baseurl}}/images/screenshots/e2.png" data-lightbox="vao"><img src="{{site.baseurl}}/images/screenshots/e2_thumb.png" /></a>
</div>
<div class="img-thumb">
	<a href="{{site.baseurl}}/images/screenshots/e3.png" data-lightbox="vao"><img src="{{site.baseurl}}/images/screenshots/e3_thumb.png" /></a>
</div>
</div>
<div style="clear:both;">
<div class="img-thumb">
	<a href="{{site.baseurl}}/images/screenshots/e4.png" data-lightbox="vao"><img src="{{site.baseurl}}/images/screenshots/e4_thumb.png" /></a>
</div>
<div class="img-thumb">
	<a href="{{site.baseurl}}/images/screenshots/e5.png" data-lightbox="vao"><img src="{{site.baseurl}}/images/screenshots/e5_thumb.png" /></a>
</div>
</div>

<div style="clear: both; padding-top: 50px;">
