---
title: Busca
layout: page
permalink: "/busca"
comments: false
---

<p> Título, tag, descrição, conteúdo ou data de publicação (2020, 2016-02, 2016-07-21).
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="buscar..."> <a href="{{site.baseurl}}/en/search">en</a>
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<!-- anteriormente estava usando arquivo local .js (linha abaixo), porém, vi que o dev atualizou o repo e o colocou no unpkg, então mudei para lá. Além disso, não está mais dando um erro, quando se verificava o console debug (firefox), apesar de funcionar normal. -->
<!-- <script src="{{site.baseurl}}/assets/js/simple-jekyll-search.min.js" type="text/javascript"></script> -->
<script src="https://unpkg.com/simple-jekyll-search@latest/dest/simple-jekyll-search.min.js"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{site.baseurl}}/search.json'
})
</script> 
