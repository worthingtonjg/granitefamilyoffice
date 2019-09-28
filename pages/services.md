---
layout: default
permalink: /services
---
{%- for post in site.section_services -%}
    {%- if forloop.index != 1 -%}
    <div id ="{{post.section-link}}" class="section-content" data-aos="fade" data-aos-duration="8000">
        <h2>{{post.heading}}</h2>
        {{post}}
    </div>
    {%- else -%} 
    <div id ="{{post.section-link}}" class="section-content">
        <h2>{{post.heading}}</h2>
        {{post}}
    </div>
    {%- endif -%} 
{%- endfor -%}