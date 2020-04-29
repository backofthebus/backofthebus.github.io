---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{% for recipe in site.recipes %}
  <div class="recipe">
    <a href="{{recipe.link}}" target="_blank">{{ recipe.title }}</a> | {{recipe.description}}
    <div>
        {% for tag in recipe.tags %}
            <span class="tag">{{ tag }}</span>
        {% endfor %}
    </div>
  </div>
{% endfor %}
