---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Research Publications

My research focuses on **perception, representation, and planning for robot manipulation**. I work at the intersection of computer vision, machine learning, and robotics to develop systems that can better understand and interact with their environment.

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Research Areas

- **Robot Manipulation**: Developing algorithms for precise and robust robotic manipulation tasks
- **Computer Vision**: Novel approaches for visual perception and scene understanding
- **Representation Learning**: Learning effective representations for robotic tasks
- **Machine Learning**: Applying deep learning and reinforcement learning to robotics
- **Motion Planning**: Algorithms for safe and efficient robot motion
