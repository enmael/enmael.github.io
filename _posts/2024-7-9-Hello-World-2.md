---
layout: post
title: 깃허브 블로그 작성용 탬플릿
date : 2024-10-04
author : "enmael"
categories: blog
tags: []
---

```csharp
//c# 코드 작성 
```

<span style="font-size: 15px;">
 글자 입력
</span>

![이미지 이름]({{ site.baseurl }}/images/이미지경로와입력)


<span style="font-size: 15px;">
 태그 작성법
</span>

{% for tag in page.tags %}
  <a href="/tags/{{ tag }}">{{ tag }}</a>
{% endfor %}

