---
title: Design Teams
layout: page
---

{% assign socials = "Website,LinkTree,Email,Instagram,Discord,Facebook,LinkedIn,TikTok,YouTube,Twitter" | split: "," %}

See the most up-to-date list of design teams and clubs on [the Affiliated Clubs page.](https://skule.ca/get-involved/affiliated_clubs.html)

{% assign socials = "Website,LinkTree,Email,Instagram,Discord,Facebook,LinkedIn,TikTok,YouTube,Twitter" | split: "," %}


<div id="clubs-container">
  {% assign design_clubs = site.data.clubs.clubs | where: "Category", "Design/Competition Team" %}
  {% assign sorted_clubs = design_clubs | sort: "Club Name" %}
  {% for club in sorted_clubs %}
  <div class="box club-box" data-category="{{ club.Category }}">
    <p>
      <b class="vp-academic-text">
        {{ club["Club Name"] }}{% if club["Club Name Abbreviation"] and club["Club Name Abbreviation"] != "" %} ({{ club["Club Name Abbreviation"] }}){% endif %}
      </b><br>
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
</div>