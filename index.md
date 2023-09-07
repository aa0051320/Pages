---

---

# Navigation

<ul>
  {% for collection in site.collections %}
    {% unless collection.label == "posts" %}
      <li>{{ collection.label }}
        <ul>
          {% for document in collection.docs %}
            <li><a href="{{ document.url | relative_url }}">{{ document.title }} - {{ document.modified_time }}</a></li>
          {% endfor %}
        </ul>
      </li>
    {% endunless %}
  {% endfor %}
</ul>

# Index Content

