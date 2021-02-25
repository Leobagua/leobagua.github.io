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
<div>
  {{ post.excerpt | strip_html }}
  <p>
    <small>
      {{ post.date | date_to_string }}
    </small>
  </p>
</div>
{% endfor %}
