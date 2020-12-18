---
title: Jeff Eaton
tagline: Digital strategy, content architecture, CMS nerdery
subhead: I help organizations understand their content and improve the tools they use to create, manage, and publish it.
---

<ul class="list-unstyled">
{%- for project in site.data.projects.items -%}
  <li class="media">
    <img class="mr-3 rounded-circle project-logo" src="{{ project.logo | relative_url }}" alt="{{ project.title }}" />
    <div class="media-body">
    {{ project.description | markdownify }}
    </div>
  </li>
{% endfor -%}
</ul>

<div class="social-icons">
    <a class="social-icon" href="https://www.linkedin.com/in/jeffeaton"><i class="fab fa-linkedin-in"></i></a>
    <a class="social-icon" href="https://github.com/eaton"><i class="fab fa-github"></i></a>
    <a class="social-icon" href="https://twitter.com/eaton"><i class="fab fa-twitter"></i></a>
</div>
