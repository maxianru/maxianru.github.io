---
permalink: /
title: ""
excerpt: ""
author_profile: true
layout: default
redirect_from: 
  - /about/
  - /about.html
---
<span class='anchor' id='个人简介'></span>
{% include_relative includes/intro.md %}

<span class='anchor' id='教育经历'></span>
{% include_relative includes/edu.md %}

<span class='anchor' id='研究方向'></span>
{% include_relative includes/research_interests.md %}

<span class='anchor' id='论文著作'></span>
{% include_relative includes/pub.md %}

<span class='anchor' id='科研项目'></span>
{% include_relative includes/projects.md %}

<span class='anchor' id='主讲课程'></span>
{% include_relative includes/courses.md %}

<span class='anchor' id='荣誉奖励'></span>
{% include_relative includes/honers.md %}

<span class='anchor' id='社会活动'></span>
{% include_relative includes/activities.md %}

<span class='anchor' id='news'></span>
{% include_relative includes/news.md %}


document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            window.scrollTo({
                top: target.offsetTop,
                behavior: 'smooth'
            });
        }
    });
});
