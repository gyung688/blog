---
layout: postlist
categories : TipsForCode
---

{% for post in site.categories.TipsForCode %}
  <div class="postlist">
    <p class="postlist__date">{{ post.date | date_to_string }}</p>
    <h2 class="postlist__title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <div class="postlist__excerpt">{{ post.excerpt }}</div>
  </div>
{% endfor %}
    -- 개인 공부를 하고 적는 것이므로 다소 부족할 수 있습니다.

