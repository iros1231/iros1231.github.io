---
title: Team
nav:
  order: 3
  tooltip: Meet our team members
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our team members are actively developing artificial intelligent systems for various purposes, especially robots, drones, embedded systems, medicine, etc. Here are our key members of our lab.

{% include section.html %}

# Head of Lab
{% include list.html data="members" component="portrait" filters="role: head" %}

{% include section.html %}

# Principal Investigators
{% include list.html data="members" component="portrait" filters="role: pi" %}

{% include section.html %}

# Researchers and Programmers
{% include list.html data="members" component="portrait" filters="role: researcher" %}
{% include list.html data="members" component="portrait" filters="role: programmer" %}

{% include section.html %}

# Graduate Students (Doctoral)
{% include list.html data="members" component="portrait" filters="role: phd" %}

{% include section.html %}

# Graduate Students (Magister)
{% include list.html data="members" component="portrait" filters="role: master" %}

{% include section.html %}

# Undergraduate Students
{% include list.html data="members" component="portrait" filters="role: undergrad" %}

{% include section.html %}

{% include site-search.html %}

<!--
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}
{% include section.html background="images/background.jpg" dark=true %} 
-->

<!--
{% include section.html background="images/background.jpg" dark=true %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
-->

<!--
{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
-->
