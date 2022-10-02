---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an associate researcher with the Image & Video Analysis group (IVA) at Institute of Automation, Chinese Academy of Sciences. I received my PhD degree in Computer Application Technology from the National Laboratory of Pattern Recognition (NLPR), Institute of Automation, Chinese Academy of Sciences, under the supervision of [Prof. Jian Cheng](http://www.nlpr.ia.ac.cn/jcheng/), in 2018. My research interests include large-scale multi-model pretraining, efficient neural network computing, distributed optimization, etc. I have published papers on IEEE T-PAMI, T-NNLS, ICML, CVPR, ICCV, etc. I won the Nvidia scholarship in 2018, the first prize of MicroNet Challenge in NeurIPS 2019,  been elected for the 2021 StarTrack Program of Microsoft Research Asia.

If you are interested in my work, feel free to contact me peisong.wang@nlpr.ia.ac.cn

Selected Publications
======
<table style="font-size:18px;width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

  {% for post in site.publications reversed%}
  <tr>
    <td style="border: none; padding:2.5%;width:25%;vertical-align:middle;max-width:100px;max-height:100px">
      <img src="/{{post.image}}" alt="project image" style="width:auto; height:auto; max-width:100%;" />
    </td>
    <td style="border: none; padding:2.5%;width:75%;vertical-align:middle">
      <h3>{{post.title}}</h3>
      {{post.authors}}
      <em>{{post.venue}}</em>, {{ post.date | date: "%Y" }}
      <br>
        {% if post.paperurl %}
          <a href="{{post.paperurl}}">paper</a> /
        {% endif %}
        {% if post.page %}
          <a href="{{post.page}}">website</a> /
        {% endif %}
        {% if post.video %}
          <a href="{{post.video}}">video</a> /
        {% endif %}
        {% if post.code %}
          <a href="{{post.code}}">code</a> /
        {% endif %}
        {% if post.poster %}
          <a href="{{post.poster}}">poster</a> /
        {% endif %}
        {% if post.slides %}
          <a href="{{post.slides}}">slides</a> /
        {% endif %}
        {% if post.dataset %}
          <a href="{{post.dataset}}">dataset</a> /
        {% endif %}
      <p></p>
      {{ post.excerpt }}
    </td>
  </tr>
  {% endfor %}
</table>