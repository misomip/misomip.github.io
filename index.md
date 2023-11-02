---
layout: default
---

<div>
<img src="{{site.url}}img/baniere.png" width="100%" height="100%"/>
</div>

<br>

## The Marine Ice Sheet Intercomparison Project
Global sea-level rise is one of the most discussed potential consequences of global warming. The most uncertain aspect of such future sea-level change has to do with the marine based ice sheets. Despite its potential importance, current generation global climate models are unable to simulate sea-level change arising from ice sheet-ocean interaction. As a step towards remediating this situation, we are bringing together the international modeling community through workshops and model intercomparison projects. Such moddelling research will lay the groundwork for including ice sheet-ocean interaction in global scale, IPCC class models.

## News
{% for post in site.posts %}
   - {{ post.date | date_to_string }} » [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
