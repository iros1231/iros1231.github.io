---
---

# Welcome to the Intelligent Robots and Systems (IRoS) Lab 

Lab IRoS ini berfokus pada penelitian yang berkaitan dengan pengembangan sistem robotik cerdas. Area kajiannya mencakup sistem sensor multimodal, model-model representasi data dan analitika untuk pengembilan keputusan pada sistem robotika, serta sistem aktuator robotika dinamis.

{% include section.html %}

## Highlights

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="research"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/publication.jpg"
  link="research"
  title="Our Publications"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our research projects"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/project.jpg"
  link="projects"
  title="Our Research Projects"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Our team members are actively developing artificial intelligent systems for various purposes, especially robots, drones, embedded systems, computer vision, medicine, etc. Here are our key members of our lab.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/members/alumni-gathering.jpg"
  link="team"
  title="Our Team"
  text=text
%}
