---
title: Oční ordinace a optika
subtitle: Praha-Radotín/Řevnice
layout: page
show_sidebar: true
hide_hero: true
top_blocks: home_blocks
---
{% assign blocks = site.data[page.top_blocks] %}
<div class="container">
    <div class="columns is-multiline is-centered">
        {% for block in blocks.items %}
            <div class="column is-6">
                <p class="title is-5 has-text-centered">{{ block.title }}</p>
                {% for part in block.parts %}
                  <p class="subtitle is-5 has-text-centered">{{ part.subtitle }}</p>
                  <div class="content">
                      <p>{{ part.description | markdownify }}</p>
                  </div>
                {% endfor %}
            </div>
        {% endfor %}
    </div>
</div>
