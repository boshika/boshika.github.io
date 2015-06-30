---
layout: default
---

<article class="post">

  <h1>{{ page.title }}Test Page</h1>

  <div class="entry">
    {{ content }}
  </div>

  <div class="date">
    Written on {{ page.date | date: "%B %e, %Y" }}
  </div>

  <div class="comments">
    {% include disqus.html disqus_identifier=page.disqus_identifier %}
  </div>
</article>
