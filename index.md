---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Required labs files may be [DOWNLOADED HERE](https://github.com/CloudKlass/Azure-Admin/edit/main/archive/AzureAdministrator-AllFiles.zip)

Hyperlinks to each of the lab exercises are listed below.

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Module | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}


