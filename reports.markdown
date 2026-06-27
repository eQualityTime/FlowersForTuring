---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Reports
layout: home
---

{% assign total = 0 %}
{% for entry in site.data.donations %}
  {% assign total = total | plus: entry.amount %}
{% endfor %}

{% assign rounded_total = total | divided_by: 1000 | round  %}

<img src="{{site.baseurl}}/assets/images/2019/1.png" alt="Alan Turing's Statue surrounded by flowers"  style="width:50%;display:block;margin-left:auto;margin-right:auto;" />

Alan Turing, the pioneering Computer Scientist and World War II codebreaker, has a statue in Sackville Gardens in Manchester. Each year on 23rd June, we honor his birthday by surrounding his statue with flowers. Since 2013, we've raised over £{{ rounded_total | append: ",000" }} for the [Open Voice Factory](https://theopenvoicefactory.org/) and the amazing [Special Effect](https://www.youtube.com/watch?v=kpYNG7MivHs&feature=emb_title). 

We've been running this event since 2013, here are the reports from previous years. Feel free to have a browse: they are a mix of heartwarming messages and much less heartwarming accounting details. 
