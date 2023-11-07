---
title: "Test1"
layout: archive
permalink: categories/test1
author_profile: true
sidebar_main: true
---

***
<!-- site.categories.Test1  : Test1는 이 페이지에서 수집해서 보여줄 카테고리의 이름을 의미한다. -->
{% assign posts = site.categories.Test1 %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}