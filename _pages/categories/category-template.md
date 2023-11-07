<!-- title      : 해당 페이지에 진입했을때 보이는 페이지에 제목 -->
<!-- permalink  : 해당 페이지의 url, nav_list_main.html에 해당 페이지를 추가할때 맞춰줘야함-->
---
title: "제목"
layout: archive
permalink: categories/foo
author_profile: true
sidebar_main: true
---

***
<!-- site.categories.foo  : foo는 이 페이지에서 수집해서 보여줄 카테고리의 이름-->
{% assign posts = site.categories.foo %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}