---
layout: docs
seo_title: 关于
cover: false
bottom_meta: false
sidebar: [blogger]
valine:
  placeholder: 有什么想对我说的呢？
---
{% image https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210212182801.jpg %}

<!-- 滚动字体特效（纯JS）：你可以在任意页面使用该特效，但是不要忘记调用相应的scrollfont滚动字效函数哦 -->
<div style="text-align:center;" id="aboutsubtitle">———— 孤筏重洋</div>

<!-- {% link 个人简历, https://muggledy.github.io, https://cdn.jsdelivr.net/gh/muggledy/best-resume-ever/resume/id.jpg %} -->

<script>
var aboutsubtitle = document.getElementById('aboutsubtitle');
scrollfont(aboutsubtitle,[aboutsubtitle.textContent]);
</script>