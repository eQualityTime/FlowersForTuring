---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Donate
layout: page
---
{% assign total = 0 %}
{% for entry in site.data.donations %}
  {% assign total = total | plus: entry.amount %}
{% endfor %}

{% assign rounded_total = total | divided_by: 1000 | round  %}

<img src="{{site.baseurl}}/assets/images/2017/1.jpg" alt="Long distance photo of statue" width=250px />


Alan Turing, the pioneering Computer Scientist and World War II codebreaker, has a statue in Sackville park in Manchester. On 23rd June each year, we surround it with flowers in their memory. 

Since 2013 we've raised £{{rounded_total | append: ",000"}} doing this, and we'd like {{ site.time | date: "%Y" }} to be our biggest year ever. Anyone who wants to get involved is welcome. Donations are made up of £3.50 to cover the cost of the flowers, a £13 charity contribution to [Special Effect](https://www.specialeffect.org.uk/), and a £3 charity contribution to the server costs of [The Open Voice Factory](https://theopenvoicefactory.org/) for a total of £18.50.   

<!-- Please use the button below to donate (it will allow you to make a bigger donation if you want). 

Thank you so much! 

<form action="https://www.paypal.com/donate" method="post" target="_top">
<input type="hidden" name="hosted_button_id" value="Q5NVFKKUZWA96" />
<input type="image" src="https://www.paypalobjects.com/en_US/GB/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
<img alt="" border="0" src="https://www.paypal.com/en_GB/i/scr/pixel.gif" width="1" height="1" />
</form>
--> 

