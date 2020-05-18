---
title: Busca
layout: page
permalink: "/en/search"
comments: false
---

<p> Title, tag, description, content or publication date (2020, 2016-02, 2016-07-21).
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="{{site.baseurl}}/assets/js/simple-jekyll-search.min.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{site.baseurl}}/search.json'
})
</script> 