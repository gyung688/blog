---
layout: postlist
categories : TIL
---

<pre>
  TIL을 시작한다.  
  깃허브 블로그가 까다로워서 원노트에 공부했던 것들을 정리했는데, 공부한 것들이 쌓이다 보니  
  블로그에 정리하는 것이 더 좋아보여서 블로그를 다시 시작하려고 한다.  
  최근에 TIL이란 것을 알게됐다. 나도 TIL을 하면서 블로그를 쌓아가야겠다.  
</pre>

{% for post in site.categories.TIL %}
  <div class="postlist">
    <p class="postlist__date">{{ post.date | date_to_string }}</p>
    <h2 class="postlist__title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <div class="postlist__excerpt">{{ post.excerpt }}</div>
  </div>
{% endfor %}

