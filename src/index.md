---
layout: base
eleventyNavigation:
  key: "Forum Home"
  order: 10
---

The **2015 DLF Forum** was held in Vancouver, BC, October 26–28, at the [Pinnacle Hotel Vancouver Harbourfront](https://www.pinnacleharbourfronthotel.com/). We greatly enjoyed our first Forum outside of the United States, and thank everyone who made it so memorable! Look here for archived video recordings and other Forum outcomes soon. You can keep up to date on future **DLF Forum news** by subscribing to our [mailing list](http://eepurl.com/baReNX), [listserv](https://lists.clir.org/cgi-bin/wa?SUBED1=DLF-ANNOUNCE&A=1), or following us on [Twitter](https://www.twitter.com/clirdlf).

<h3 class="mt-5 pb-4 mb-4 border-bottom">2015 Blog Posts</h3>

{% for post in collections.posts %}
<article class="blog-post border-bottom">
    <h2 class="blog-post-title"><a href="{{ post.data.url }}">{{ post.data.title }}</a></h2>
    <p class="blog-post-meta">{{ post.data.date | readableDate }} in <a href="https://www.diglib.org/category/forum/">Forum</a></p>
    <p>{{ post.data.blurb }}...</p>
    <p>
        <a href="{{ post.data.url }}" class="btn btn-outline-primary">Read More</a>
    </p>
</article>
{% endfor %}

<div class="my-5 py-5">
<a target="_blank" href="https://www.diglib.org/category/forum/" class="btn btn-primary">Read More Forum Posts</a>
</div>