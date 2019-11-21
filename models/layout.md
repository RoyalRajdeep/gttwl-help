### Tags used in your Layouts and internal templates

#### Agency
{{agency}}
{{agency.name}}
{{agency.cname}}
etc...

#### To Include Content:
-------------------
{{content_for_layout}}

#### Meta Information
----------------
{{meta_title}}
{{meta_description}}
{{meta_keywords}}

#### Custom HTMl Header Info
-----------------------
{{html_header}}

#### Miscellenous:
-------------
{{year}} * eg: "2013"
{{csrf}} * Include this in all forms with a POST method
{{ip_address}} -- IP Address of thte visitor
{{params}} -- any params in the URL. eg: http://yoursite.com?greeting=hello would be {{params.greeting}}

#### Env Variables
-------------
{{env.server_software}}
{{env.server_name}}
{{env.request_method}}
{{env.request_path}}
{{env.path_info}}
{{env.request_uri}}
{{env.http_version}}
{{env.http_host}}
{{env.http_connection}}
{{env.http_cache_control}}
{{env.http_accept}}
{{env.http_if_none_match}}
{{env.http_user_agent}}
{{env.http_referer}}
{{env.http_accept_encoding}}
{{env.http_accept_language}}
{{env.http_cookie}}
{{env.gateway_interface}}
{{env.server_port}}
{{env.query_string}}
{{env.server_protocol}}
{{env.script_name}}
{{env.remote_addr}}
{{env.original_fullpath}}
{{env.current_url}}

#### Menu System
-----------
{{menu}} - A simple menu system like this:
It's an array of arrays, eg:
<ul>
{% for m in menu %}
  <li><a href="{{m.url}}">{{m.title}}</a>
   <ul>
   {% for submenu in m.menu %}
     <li><a href="{{submenu.url}}">{{submenu.title}}</a></li>
   {% endfor %}
   </ul>
  </li>
{% endfor %}
</ul>

#### Currently Logged In User
------------------------
{{current_user}}
{{current_user.name}}
{{current_user.link}} -- link for user profile page
(rest is same is {{author}} tags)

