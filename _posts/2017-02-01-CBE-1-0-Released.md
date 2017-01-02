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

## {{page.title}}

We have released a new image effect to help with designing a better user experience for colorblind people.

Colorblind Effect (CBE) plugin simulates three most common types of colorblindness. This lets gamedesigners better identify potential problems with reduced color vision

![]({{site.baseurl}}/images/colorblind1.jpg)

## About CBE

You can get CBE at [Unity Asset Store](https://www.assetstore.unity3d.com/en/#!/content/76360).

See [documentation here](https://projectwilberforce.github.io/colorblind/) and [forum here](https://forum.unity3d.com/threads/released-colorblind-image-effect-check-how-colorblind-see-your-game.448971/).

Please rate, review and comment, we are looking forward to your feedback.

In case of questions or further issues, please contact us at <projectwilberforce@gmail.com>

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