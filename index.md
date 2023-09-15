---
slug: Index
---

# {{ page.slug }}

# [About](/about.md)

# Table of Contents
<ul>
  {% assign sorted_collections = site.collections | sort: 'order' %}
  {% for collection in sorted_collections %}
    {% unless collection.label == "posts" %}
      <li>{{ collection.label }}
        <ul>
          {% assign sorted_items = collection.docs | sort: 'order' %}
          {% for document in sorted_items %}
            <li><a href="{{ document.url | relative_url }}">{{ document.slug }}</a></li>
          {% endfor %}
        </ul>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
