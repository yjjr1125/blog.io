---
layout: default
---

{
    "code" : 0 ,
    "data" : [
    {% for post in site.posts %}
    {
    	"title" : " - {% for tag in post.tags %}{% if forloop.rindex != 1 %}{% else %}{% endif %}{% endfor %}",
    	"url" : ""
    }
	{% if forloop.rindex != 1  %}
	,
	{% endif %}
     {% endfor %}
	]
 }
