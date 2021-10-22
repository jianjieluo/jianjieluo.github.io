---
layout: single
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<h2>News</h2>
<div id="news">
  {% for item in site.data.news.main %}
  <p><strong><font class="new">NEW! </font></strong>{{ item | markdownify | remove: '<p>' | remove: '</p>'}}</p>
  {% endfor %}
  <a href="#" onclick="hideBlock('news'); showBlock('allnews'); return false;" class="btn btn--inverse">More</a>
</div>
<div id="allnews" style="display: none;">
  {% for item in site.data.news.all %}
  <p><strong><font class="new">NEW! </font></strong>{{ item | markdownify | remove: '<p>' | remove: '</p>'}}</p>
  {% endfor %}
  <a href="#" onclick="hideBlock('allnews'); showBlock('news'); return false;" class="btn btn--inverse">Less</a>
</div>

<h2 style="clear: both;" id="publications">Publications <a href="https://scholar.google.com/citations?user=PMgCjQcAAAAJ" style="font-size: 0.85em; font-weight: normal;">[Google Scholar]</a></h2>

<h3>2021</h3>
{% for publication in site.data.publications.year2021 %}
  {% include publication-single.html %}
{% endfor %}
<div style="clear: both;"></div>

<h3>2020</h3>
{% for publication in site.data.publications.year2020 %}
  {% include publication-single.html %}
{% endfor %}
<div style="clear: both;"></div>

<h2 style="clear: both;" id="bio">Bio</h2>

I am currently a Ph.D student of [School of Computer Science and Engineering](https://cse.sysu.edu.cn/) in [Sun Yat-sen University(SYSU)](http://www.sysu.edu.cn/2012/en/index.htm), a member of a joint Ph.D. program between SYSU and [JD AI Research(JDAIR)](https://air.jd.com/#index). My advisors are [Dr. Ting Yao](http://tingyao.deepfun.club/), [Dr. Tao Mei](https://taomei.me/) and [Prof. Hongyang Chao](https://cse.sysu.edu.cn/content/2508).

<h2 style="clear: both;" >Research Interests</h2>

* Vision and Language
* Video Analytics
* Representation Learning

<h2 style="clear: both;">Education</h2>

* **08/2019 - 06/2024, Sun Yat-Sen University**
  * Ph.D. in Computer Science and Technology (Expected June 2024)
  * Joint Ph.D. Program with JD AI Research

* **08/2015 - 07/2019, Sun Yat-sen University (GPA:3.9, rank 8/120)**
  * B.S. in Software Engineering

<h2 style="clear: both;">Selected Awards</h2>

* **Outstanding Undergraduate**, SYSU 2019, **Top 5%** in SYSU
* **National Scholarship**, 2018, **Top 1%** in SYSU
* **Finalist Winner** of 2018 American College Students Mathematical Modeling Contest, **Top 0.38%** in 20638 teams

<h2 style="clear: both;">Experiences</h2>

* **08/2020 - Present**: Research Intern
  * Computer Vision and Multimedia Lab at JD AI Research, Beijing
  * Mentor: [Ting Yao](http://tingyao.deepfun.club/)

* **07/2018 - 04/2019**: Research Intern
  * Computer Vision and Multimedia Lab at JD AI Research, Beijing
  * Mentor: [Ting Yao](http://tingyao.deepfun.club/)

* **03/2018 - 06/2018**: Research Intern
  * [Pixtalks Technology](http://www.pixtalks.com/home), Guangzhou
  * Mentor: [Shengyong Ding](https://dblp.uni-trier.de/pers/hd/d/Ding:Shengyong)


