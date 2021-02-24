# Welcome, nil
```ruby 
# Hi, my name is Leonardo da Rosa.
# Welcome to my blog.
# Here, we're gonna talk about some cool things

# You can find me over the internet as @leobagua
```

## Posts
{% for post in site.posts %}
<h3>
  <a href="{{ post.url }}">{{ post.title }}</a>
</h3>
<p class="author">
  <span class="date">{{ post.date }}</span>
</p>
<div class="highlight">
  {{ post.content }}
</div>
<div>
  {{ post.content }}
</div>
<div class="highlight">
  {{ post.excerpt }}
</div>
<div>
  {{ post.excerpt }}
</div>
{% endfor %}
