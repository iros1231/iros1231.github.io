---
title: Publications
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

Compilation of all our members' published works.

{% include section.html %}

## Highlighted

{% include citation.html lookup="10.1109/ACCESS.2022.3141200" style="rich" %}
{% include citation.html lookup="10.1186/s40537-020-00374-x" style="rich" %}
{% include citation.html lookup="10.1109/ACCESS.2020.2969021" style="rich" %}
{% include citation.html lookup="10.1016/j.media.2020.101712" style="rich" %}

{% include section.html %}

## All

{% include search-box.html %}

{% include search-info.html %}

{% capture content %}
{% include list.html data="citations" component="citation" %}
{% endcapture %}
{% include grid.html content=content %}
