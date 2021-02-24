# Welcome, nil
```ruby 
# Hi, my name is Leonardo da Rosa.
# Welcome to my blog.
# Here, we're gonna talk about some cool things

# You can find me over the internet as @leobagua
```

## Posts
<ul>
  {% for post in paginator.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% for post in paginator.posts %}
<h2>
  <a href="{{ post.url }}">{{ post.title }}</a>
</h2>
<p class="author">
  <span class="date">{{ post.date }}</span>
</p>
<div class="content">
  {{ post.content }}
</div>
<div class="excerpt">
  {{ post.excerpt }}
</div>
{% endfor %}

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="previous">
      Previous
    </a>
  {% else %}
    <span class="previous">Previous</span>
  {% endif %}
  <span class="page_number ">
    Page: {{ paginator.page }} of {{ paginator.total_pages }}
  </span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% else %}
    <span class="next ">Next</span>
  {% endif %}
</div>
