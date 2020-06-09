---
title: I write about stuff.
nav: Writing
order: 3
---
I write semi-regularly on [Medium](https://medium.com/@eaton), contribute to the [Lullabot blog](https://www.lullabot.com/topics/content-strategy), and host a [mothballed personal site](http://angrylittletree.com) that serves as a record of embarrassing things I said in the 90s. There are, thankfully, a few standout pieces I think stand the test of time.

{% assign pieces = site.writing | sort: 'order'  %}
{%- for piece in pieces -%}
<h5 class="mt-0 mb-1"><a href="{{ piece.link }}">{{ piece.title }}</a><small class="muted"> — {{ piece.published_by }}</small></h5>
{{ piece.content }}
{% endfor -%}