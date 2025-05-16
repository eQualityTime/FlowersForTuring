---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

{% assign total = 0 %}
{% for entry in site.data.donations %}
  {% assign total = total | plus: entry.amount %}
{% endfor %}

{% assign rounded_total = total | divided_by: 1000 | round  %}

<img src="{{site.baseurl}}/assets/images/2019/1.jpg" alt="Alan Turing's Statue surrounded by flowers">  
Alan Turing, the pioneering Computer Scientist and World War II codebreaker, has a statue in Sackville Gardens in Manchester. Each year on 23rd June, we honor his birthday by surrounding his statue with flowers. Since 2013, we've raised over £{{ rounded_total | append: ",000" }} for the [Open Voice Factory](https://theopenvoicefactory.org/) and the amazing [Special Effect](https://www.youtube.com/watch?v=kpYNG7MivHs&feature=emb_title). Based in the UK, they use video games and technology to enhance the quality of life of people with disabilities.

By joining us in this heartfelt tradition, you can help celebrate Alan Turing's legacy and support an amazing cause. If you are curious about the event, check out our [FAQ](faq.html), or one of our [reports](reports.html). 

<img src="{{site.baseurl}}/assets/images/specialeffect.jpg" alt="One of the children helped by special effect">  

<!-- 
Amounts raised
2014,   436
2015,   650
2016,  2050
2017,   976
2018,  1530
2019,  1918
2021,  2459
2022,  2708
2023, 4875 + 4300 + 2,432.16 = 11607.16   
----
22,000 
---> 
