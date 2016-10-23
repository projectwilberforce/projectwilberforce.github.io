---
title:  "Volumetric Ambient Occlusion Unity Plugin v1.3 has been released"
date:   2016-10-21 18:36:42
categories: unity plugin
excerpt: "New version includes luminance sensitivity option and new random samples sets for better visual quality."
tags: [vao, new releases, ssao, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

## {{page.title}}

New version of our VAO has been released! We have both added new features and optimized the existing ones.

VAO is our answer to ambient occlusion problem. It has better performance and visual quality than other SSAO solutions. 

![]({{site.baseurl}}/images/social-vao-heading.jpg)

## What's new in v1.3  

 * Luminance sensitivity
 * Better visual quality (for all quality settings)

## About VAO

VAO works by approximating amount of light that can reach given pixel taking volume of surrounding geometry into account. We have developed fast approximation algorithm and use fine-tuned random samples sets to calculate it in real time. Ambient occlusion will add depth and realism to your scenes.

Our algorithm works in screen space (using only normals and depth values readily available in G-Buffer). Therefore, there is no performance hit when using more complicated meshes (more polygons) and it makes use of bump textures automatically. It is also fully dynamic - there is no need for pre-calculating specific scenes and it works with both static and moving objects.

In the newest version, we also provide option to gradually reduce VAO on bright surfaces such as windows, TV screens, lamps etc. making it easy to setup VAO in wide variety of scenes.

You can get VAO at [Unity Asset Store](http://u3d.as/xzs).

See [documentation here](https://projectwilberforce.github.io/vaomanual/) and [forum here](https://forum.unity3d.com/threads/volumetric-ambient-occlusion-image-effect.428426/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>

## Screenshots

<div>Try moving the sliders to see the difference:</div>
<iframe frameborder="0" class="juxtapose" width="100%" height="380" src="{{site.baseurl}}/sliders/slider1.html"></iframe>
<iframe frameborder="0" class="juxtapose" width="100%" height="380" src="{{site.baseurl}}/sliders/slider2.html"></iframe>

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

{% if page.comments %}
<div id="disqus_thread"></div>
<script>
var disqus_config = function () {
this.page.url = "{{site.url}}{{ page.url }}"; // <--- use canonical URL
this.page.identifier = "{{ page.id }}";
};
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = '//vaounityplugin.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>

<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
</div>

{% endif %}