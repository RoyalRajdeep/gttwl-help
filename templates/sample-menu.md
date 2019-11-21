```
<ul class="nav" id="main-menu-left">
    {% for m in menu %}
    <li {% if m.menu.size > 0 %} class="dropdown" {% endif %}>
      {% if m.menu.size > 0 %}
      <a href="{{m.url}}" class="dropdown-toggle" data-toggle="dropdown">{{m.title}}  <b class="caret"></b></a>
      <ul class="dropdown-menu" id="swatch-menu">
        {% for s in m.menu %}
          <li><a href="{{s.url}}">{{s.title}}</a></li>
        {% endfor %}
      </ul>
      {% else %}
      <a href="{{m.url}}">{{m.title}}</a>
      {% endif %}
    </li>
    {% endfor %}
</ul>
```
