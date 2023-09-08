---

---

# About
| Content Author | Crescent Chen                                                                |
| :------------: | :--------------------------------------------------------------------------- |
|     Email      | <mailto:aa0051320@gmail.com>                                                 |
|  X (Twitter)   | [@aa0051320](https://twitter.com/aa0051320){:target="_blank"}                |
|    YouTube     | <https://www.youtube.com/channel/UCGvANU1XJmT3FVQBt8Ixbog>{:target="_blank"} |

# Table of Content
<ul>
  {% for collection in site.collections %}
    {% unless collection.label == "posts" %}
      <li>{{ collection.label }}
        <ul>
          {% for document in collection.docs %}
            <li><a href="{{ document.url | relative_url }}">{{ document.title }}</a></li>
          {% endfor %}
        </ul>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
