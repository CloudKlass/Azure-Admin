---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Required **labs files** can be [DOWNLOADED HERE](https://github.com/MicrosoftLearning/AZ-104-MicrosoftAzureAdministrator/archive/master.zip)

Please use the Hyperlinks to each of the lab exercises listed below *(not from the LabFiles download above)*.

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Module | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}


