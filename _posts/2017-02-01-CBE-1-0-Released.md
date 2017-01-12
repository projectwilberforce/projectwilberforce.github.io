---
title:  "New Release - Colorblind Effect Unity Plugin"
date:   2017-01-02 12:30:00
categories: unity plugin
excerpt: "We have released a new image effect to help with designing a better user experience for colorblind people."
tags: [cbe, new releases, ux, unity plugin, unity3d]
layout: default
comments: true
permalink: /blog/:title
---

<time datetime="{{ page.date | date_to_xmlschema }}">
  <em>{{ page.date | date: "%b %-d, %Y" }}</em>
</time>

## {{page.title}}

We have released a new image effect to help with designing a better user experience for colorblind people.

## About CBE

Colorblind Effect (CBE) plugin simulates three most common types of colorblindness. This lets gamedesigners better identify potential problems with reduced color vision.

With this plugin it is easy to check if some part of the game relies too much on colors as a source of information (for example, people with most common colorblindness have trouble distinguishing between red and green). 
Typical problems are:

 - Color gradidents: healthbars, threat levels etc.
 - Only color-coded information: eg. green friendly and red enemy units on minimap
 - Overlaying colors that look similar to colorblind: GUI/HUD might be hard to see in certain areas, or something as simple as wrong combination of text and background color

![]({{site.baseurl}}/images/colorblind1.jpg)

## Additional information

You can get CBE at [Unity Asset Store](https://www.assetstore.unity3d.com/en/#!/content/76360).

See [documentation here](https://projectwilberforce.github.io/colorblind/) and [forum here](https://forum.unity3d.com/threads/released-colorblind-image-effect-check-how-colorblind-see-your-game.448971/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>

{% if page.comments %}
<!--<div id="disqus_thread"></div>
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
</div>-->

{% endif %}