---

---

# Navigation

<ul>
  {% for collection in site.collections %}
    <li>{{ collection.label }}
      <ul>
        {% for document in collection.docs %}
          <li><a href="{{ document.url }}">{{ document.title }}</a></li>
        {% endfor %}
      </ul>
    </li>
  {% endfor %}
</ul>

# Index Content
