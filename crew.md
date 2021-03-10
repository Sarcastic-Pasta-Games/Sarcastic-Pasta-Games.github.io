---
title: Crew
layout: default
--- 
 <h2>
    Our crew
  </h2>
  <article>

    <h3 class="blue-text">Leadership</h3>
    {% for staff_member in site.crew %}
      {% if staff_member.position == "Leadership" %}
        <h4>{{ staff_member.name }}</h4>
        <p>{{ staff_member.content | markdownify }}</p>
      {% endif %}
    {% endfor %}
 
    <h3 class="blue-text">Visuals</h3>
      {% for staff_member in site.crew %}
        {% if staff_member.position == "Visuals" %}
          <h4>{{ staff_member.name }}</h4>
          <p>{{ staff_member.content | markdownify }}</p>
        {% endif %}
    {% endfor %}

    <h3 class="blue-text">Music</h3>
      {% for staff_member in site.crew %}
        {% if staff_member.position == "Music" %}
          <h4>{{ staff_member.name }}</h4>
          <p>{{ staff_member.content | markdownify }}</p>
        {% endif %}
    {% endfor %}
  </article>