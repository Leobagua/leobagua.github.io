# Welcome, nil
```ruby 
# Hi, my name is Leonardo da Rosa.
# Welcome to my blog.
# Here, we're gonna talk about some cool things

# You can find me over the internet as @leobagua
```

## Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
