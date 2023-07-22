---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 3
dropdown: true
children:
    - title: publications
      permalink: /publications/
    - title: category2
    - title: category3
      permalink:
---
<!-- _pages/publications.md -->
<div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} %}

</div>
