---
layout: article
title: "Video"
description: "Learn about the simplest ways to add video to your site and ensure users
              get the best possible experience on any device."
introduction: "Users like videos; they can be fun, informative.
               On mobile devices, videos can be an easier way to consume information.
               But videos take bandwidth;
               they don't always work the same across every platform.
               Users don't like waiting for videos to load,
               or when they press play and nothing happens.
               Read more to find the simplest way to add video to your site and
               ensure users get the best possible experience on any device."
article:
  written_on: 2014-04-16
  updated_on: 2014-04-29
  order: 2
collection: introduction-to-media
id: videos
key-takeaways:
  add-a-video:
    - Use the video element to load, decode, and play video on your site.
    - Produce video in multiple formats to cover a range of mobile platforms.
    - Size videos correctly; ensure they don't overflow their containers.
    - Accessibility matters; add the track element as a child of the video element.
remember:
  media-fragments:
    - The Media Fragments API is supported on most platforms, but not on iOS.
    - Make sure Range Requests are supported by your server. Range Requests are enabled by default on most servers, but some hosting services may turn them off.
  dont-overflow:
    - Don't force element sizing that results in an aspect ratio different from the original
      video. Squashed or stretched looks bad.
  accessibility-matters:
    - The track element is supported on Chrome for Android, iOS Safari, and all current browsers on desktop except Firefox (see <a href="//caniuse.com/track" title="Track element support status">caniuse.com/track</a>). There are several polyfills available too. We recommend <a href='//www.delphiki.com/html5/playr/' title='Playr track element polyfill'>Playr</a> or <a href='//captionatorjs.com/' title='Captionator track'>Captionator</a>.
  construct-video-streams:
    - MSE is supported by Chrome and Opera on Android, and in Internet Explorer 11 and Chrome for desktop, with support planned for <a href='//wiki.mozilla.org/Platform/MediaSourceExtensions' title='Firefox Media Source Extensions implementation timeline'>Firefox</a>.
  optimize:
    - <a href="../images/">Images</a>
    - <a href="../../performance/optimizing-content-efficiency/">Optimizing content efficiency</a>
---

{% wrap content%}

<style>

  img, video, object {
    max-width: 100%;
  }

  img.center {
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

</style>

{% for guide in page.articles.videos %}
1. [{{guide.title}}]({{site.baseurl}}{{guide.url | clean}}) &mdash;
{{guide.description}}
{% endfor %}

{% include modules/nextarticle.liquid %}

{% endwrap %}
