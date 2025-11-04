---
title: Affiliated Clubs
layout: page
---

{% assign socials = "Website,LinkTree,Email,Instagram,Discord,Facebook,LinkedIn,TikTok,YouTube,Twitter" | split: "," %}
{% assign categories = "Arts and Music|Athletics|Social Change and Advocacy|Community Service and Outreach|Cultural, Faith, or Identity-Based Community Group|Design/Competition Team|Hobby/Special Interest|Education and Professional Development|Discipline-Specific Club" | split: "|" %}


<h2 class="vp-academic-text mb-3" style="font-size: 1.25rem;">Filter by Category</h2>
<div id="category-filters" class="buttons are-small mb-5">
  {% for category in categories %}
    <button class="button is-light category-button" data-category="{{ category | strip }}">{{ category }}</button>
  {% endfor %}
</div>

<div id="clubs-container">
  {% assign sorted_clubs = site.data.clubs.clubs | sort: "Club Name" %}
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

<script>
document.addEventListener("DOMContentLoaded", function() {
  const buttons = document.querySelectorAll(".category-button");
  const clubs = document.querySelectorAll(".club-box");
  let selectedCategories = [];

  buttons.forEach(button => {
    button.addEventListener("click", () => {
      const category = button.dataset.category;
      button.classList.toggle("is-vp-academic");

      if (selectedCategories.includes(category)) {
        selectedCategories = selectedCategories.filter(c => c !== category);
      } else {
        selectedCategories.push(category);
      }

      clubs.forEach(club => {
        const clubCategory = club.dataset.category?.trim();
        if (selectedCategories.length === 0 || selectedCategories.includes(clubCategory)) {
          club.style.display = "";
        } else {
          club.style.display = "none";
        }
      });
    });
  });
});
</script>

<style>
.category-button.is-vp-academic {
  background-color: var(--vp-academic-color, #003366);
  color: white;
}
</style>
