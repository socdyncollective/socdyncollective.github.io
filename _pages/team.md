---
title: "Social Dynamics Collective - Members"
layout: gridlay
excerpt: "Social Dynamics Collective - Members"
sitemap: false
permalink: /team/
---

# Faculty

{% assign number_printed = 0 %}
{% for member in site.data.faculty %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left"/>
<h4>{{ member.name }}</h4>
<i>{{ member.info }} <br> 
email: {{ member.email }} <br> 
{{ member.web }}
</i>

<ul style="overflow: hidden">
{% if member.number_educ == 1 %}
<li> {{ member.education1 }} </li>
{% endif %}

{% if member.number_educ == 2 %}
<li> {{ member.education1 }} </li>
<li> {{ member.education2 }} </li>
{% endif %}

{% if member.number_educ == 3 %}
<li> {{ member.education1 }} </li>
<li> {{ member.education2 }} </li>
<li> {{ member.education3 }} </li>
{% endif %}

</ul>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

# Ph.D. Students

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left"/>
<h4>{{ member.name }}</h4>
<i>{{ member.info }} <br> 
email: {{ member.email }}
</i>

<ul style="overflow: hidden">
{% if member.number_educ == 1 %}
<li> {{ member.education1 }} </li>
{% endif %}

{% if member.number_educ == 2 %}
<li> {{ member.education1 }} </li>
<li> {{ member.education2 }} </li>
{% endif %}

{% if member.number_educ == 3 %}
<li> {{ member.education1 }} </li>
<li> {{ member.education2 }} </li>
<li> {{ member.education3 }} </li>
{% endif %}

</ul>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

# MSc. Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left"/>
<h4>{{ member.name }}</h4>
<i>thesis: "{{ member.topic }}" <br></i>
<i>supervised by {{ member.supervisors }} <br></i>
<i>{{ member.mprogram }} <br></i>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

# Friends
{% assign number_printed = 0 %}
{% for member in site.data.friends %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}
<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left"/>
<h4>{{ member.name }}</h4>
<i>{{ member.position }} <br></i>
<i>{{ member.affiliation }} <br></i>
<i>{{ member.website }} </i>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}