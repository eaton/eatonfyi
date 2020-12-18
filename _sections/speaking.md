---
title: I talk about stuff.
nav: Speaking
order: 2
---
I'm a frequent speaker at web tech, content strategy, and design events including [The IA Conference](https://www.confabevents.com), [Confab](https://www.confabevents.com), [DrupalCon](https://events.drupal.org), [SXSW](https://www.sxsw.com), and [Design/Content](https://content.design). I'm a contributor to UIE's [All-You-Can-Learn library](https://aycl.uie.com/experts/jeff_eaton), the occasional host of a [content-centric podcast](http://insertcontenthere.com), and I've spent the last several years running content modeling workshops for individuals and teams.

<ul class="list-unstyled">
{% assign talks = site.speaking | sort: 'order'  %}
{%- for talk in talks -%}
  <li class="media">
    <a class="d-none d-sm-block" href="{{ talk.video_url }}"><img src="{{ talk.video_thumb }}" class="mr-3 talk-thumb"></a>
    <div class="media-body">
      <h5 class="mt-0 mb-1"><a href="{{ talk.video_url }}">{{ talk.title }}</a><small class="muted"> — <a href="{{ talk.event_url }}">{{ talk.event }}</a></small></h5>
      {{ talk.summary | markdownify }}
    </div>
  </li>
{% endfor -%}
</ul>

If you think the themes I talk about would be a valuable addition to your event, or your organization needs a crash course in advanced content architecture, [drop me a line](#contact).