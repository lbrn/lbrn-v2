---
layout: post
title: LBRN Workshops
featuredImageUrl: images/MicrosoftTeams-image.png
featuredImageUrlSquare: images/MicrosoftTeams-image.png
excerpt_separator: <!--more-->
desc: LBRN Cores host various one or two day workshops throughout the year where researchers, faculty, graduate and undergraduate students are invited to attend. Topics range from computational bioinformatics to protein purification, etc.
eventDate: Beginning June 8, 2020
---

<section class="news tne" id="newsContainer">
<!-- add limit: 2 to the 2nd tne post if needed -->
{% assign tne-post = site.posts | where: "tags", "workshop" %}
  {% for post in tne-post %}
    {% include news-full-list-item.html %}
  {% endfor %}

</section>
<aside id="newsSidebar" class="tne">
  <ul>
    {% for post in tne-post %}
      <a href="#{{post.date}}"><li>{{post.title}}</li></a>
    {% endfor %}
  </ul>
</aside>
