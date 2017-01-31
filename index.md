## AdBOOST.sk - platform manual


Welcome to AdBOOST platform manual. Feel free to browse features displayed in the right sidebar or if you know exactly what you are looking for, use search bar on top of the page to quickly navigate towards most accurate results and quickly fulfill your needs.

### Most recent topics

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


