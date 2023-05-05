
Papers by day
=======

<ul>
{% for post in site.posts %}
<li><article> 
      <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> --       
      <a href="{{ post.url }}"> {{ post.title }} </a>
</article></li>
{% endfor %}
</ul>
