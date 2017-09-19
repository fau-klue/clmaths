---
layout: default
---

A lot of people struggle with maths and getting into it can be scary, [but that's not your fault](https://www.youtube.com/watch?v=7snnRaC4t5c). If my 7th grade maths teacher would have told me that Linear Algebra is at the heart of many machine learning algorithms, that would have been great. Anyhow, you're here and ready to take a step towards a deeper understanding of computational theories. Don't worry, you can do it!

The topics in this course are aimed at Computational Linguists. That means, we're going to use linguistic examples to make topics directly relatable. It will give you a basic understanding of everything you need to get started in your studies. The topics are not in any specific order, so feel free to begin where and skip whatever you like.

## Topics

{% for topic in site.pages %}
    {% if topic.url contains 'topic' %}

[{{ topic.title }}]({{ site.baseurl }}{{ topic.url }})
<br/>
<em> {{topic.description}} </em>

{% endif %}
{% endfor %}

