---
title: Affiliated Clubs
layout: page
---

{% assign socials = "LinkTree,Instagram,Discord,Facebook,LinkedIn,TikTok,YouTube,Twitter,Website,Email" | split: "," %}

{% for club in site.data.clubs.clubs %}
<div class="box">
  <p>
    <b class="vp-academic-text">{{ club["Club Name"] }}</b><br>
  </p>

  {% if club["Club Description"] %}
    <p>{{ club["Club Description"] }}</p>
  {% endif %}

  <div class="buttons are-small mt-2">
    {% for social in socials %}
      {% assign value = club[social] %}
      {% if value %}
        {% assign lower = social | downcase %}
        {% capture url %}
{% if value contains "http" %}{{ value }}
{% elsif lower == "website" %}https://{{ value | strip }}
{% elsif lower == "linktree" %}https://linktr.ee/{{ value | remove: "@" | strip }}
{% elsif lower == "email" %}mailto:{{ value | strip }}
{% elsif lower == "instagram" %}https://www.instagram.com/{{ value | remove: "@" | strip }}/
{% elsif lower == "discord" %}https://discord.gg/{{ value | strip }}
{% elsif lower == "facebook" %}https://www.facebook.com/{{ value | strip }}
{% elsif lower == "linkedin" %}https://www.linkedin.com/company/{{ value | strip }}
{% elsif lower == "youtube" %}https://www.youtube.com/{{ value | strip }}
{% elsif lower == "twitter" %}https://twitter.com/{{ value | remove: "@" | strip }}
{% elsif lower == "tiktok" %}https://www.tiktok.com/@{{ value | remove: "@" | strip }}
{% else %}{{ value }}
{% endif %}
        {% endcapture %}
        <a class="button is-small vp-academic" href="{{ url | strip }}" target="_blank" rel="noopener">
          {{ social }}
        </a>
      {% endif %}
    {% endfor %}
  </div>
</div>
{% endfor %}
