---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% for post in paginator.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}

<div class="pagination">
  <span class="previous">{{ paginator.previous_page }}</span>
  <span class="next">{{ paginator.next_page }}</span>
</div>
