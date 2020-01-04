---
title: Welcome to my Blog
layout: blog
---

<main>
{% for post in site.posts %}
      <a href="{{site.baseurl}}{{post.url}}" style="text-decoration: none;">
        <div class="article">
          <p class="a-title">
            {{post.title}}
          </p>
          <p class="a-date">{{post.date | date_to_string}}</p>
        </div>
      </a>
{%endfor%}
</main>