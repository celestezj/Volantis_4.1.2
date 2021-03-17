---
layout: friends
cover: true
sidebar: []
top_meta: false
---
<p style="text-align:left;font-size:28px">🌻友情链接</p>
<hr>
<!-- more -->

<!-- <p style="text-align:left;font-size:20px">小伙伴们</p> -->
{% issues sites | api=https://api.github.com/repos/celestezj/ImageHosting/issues?sort=updated&state=open&page=1&per_page=100&labels=active %}

<br><br>

{% tabs tab-id %}

<!-- tab 友链申请流程 -->

{% timeline %}

{% timenode 步骤一：请先将本站添加到贵站 %}

- 名称：Muggledy's Blog
- 链接：https://muggledy.top/
- 头像：https://cdn.jsdelivr.net/gh/celestezj/ImageHosting@v0.1/img/20210207093620.ico
- 截图：https://cdn.jsdelivr.net/gh/celestezj/ImageHosting/img/20210318153848.png
- 描述：好好学习，天天向上

{% endtimenode %}

{% timenode 步骤二：前往GitHub，新建<a href="https://github.com/celestezj/ImageHosting/issues" target="_blank">Issue</a> %}

```json
{
    "title": "",  #网站标题
    "screenshot": "",  #网站截图
    "url": "",  #网站链接
    "avatar": "",  #网站头像
    "description": "",  #网站描述
}
```
建议先将图片压缩一下，以提高加载速度

{% endtimenode %}

{% timenode 步骤三：等待博主审核 %}

无需操作，也可在下方评论区留言（请填写正确的邮箱）

{% endtimenode %}

{% endtimeline %}

<!-- endtab -->

<!-- tab 友链申请须知 -->

1. 非博客类网站不接收，抱歉🙇
2. 能够添加本站我深感荣幸，谢谢🥰

<!-- endtab -->

{% endtabs %}