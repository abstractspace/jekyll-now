---
layout: post
title: Initial Impressions
comments: true
usemathjax: true
---
It was difficult for me, but I finally got math working!  $$x=\frac{1}{2}$$

I found the best instructions on how to do this here: https://alan97.github.io/random/mathjax/

Basically I had to just add one snippet of code to my _layouts/default .html document. 


{% if page.comments %}
<div id="disqus_thread"></div>
<script>
var disqus_config = function () {
this.page.url = page.url;  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = page.id; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://https-abstractspace-github-io.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
{% endif %}