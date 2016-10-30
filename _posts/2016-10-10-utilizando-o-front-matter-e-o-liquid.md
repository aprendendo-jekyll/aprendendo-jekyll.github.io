---
layout: post
title:  "Utilizando o Front Matter e o Liquid"
date:   2016-10-10 19:21:37 -0300
categories: jekyll curso
comments: true
hello_world: "Hello World com Liquid!"
itens:
 - "Item 1"
 - "Item 2"
 - "Item 3"
show_date: true
---
#### (Escopo de variáveis)
{{ page.hello_world }} (Escopo: page)  
{{ site.markdown }} (Escopo: site)  
 
#### (Loops)
{% for item in page.itens %}
{{ item }} 
{% endfor %}

#### (Condicionais)
{% if page.show_date %}
18/09/2016
{% endif %}
