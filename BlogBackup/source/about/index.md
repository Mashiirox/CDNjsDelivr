---
title: about
date: 2019-11-22 23:22:46
keywords: 关于
description: 
comments: false
photos: https://cdn.jsdelivr.net/gh/MashiroRb/CDNjsDelivr@v1.8/img/banner/miku.jpg
---
{% raw %}
<!-- 因为vue和botui更新导至bug,现将对话移至js下的botui中配置 -->
<div class="entry-content">
  <div class="moe-mashiro" style="text-align:center; font-size: 50px; margin-bottom: 20px;">[さくら荘のねこ]</div>
  <div id="hello-mashiro" class="popcontainer" style="min-height: 300px; padding: 2px 6px 4px; background-color: rgba(242, 242, 242, 0.5); border-radius: 10px;">
    <center>
    <p>
    </p>
    <h4>
    与&nbsp;<ruby>
    Mashiro&nbsp;<rp>
    （</rp>
    <rt>
    真（ま）白（しろ）</rt>
    <rp>
    ）</rp>
    </ruby>
    对话中...</h4>
    <p>
    </p>
    </center>
    <bot-ui></botui>
  </div>
</div>
<script src="/js/botui.js"></script>
<script>
bot_ui_ini()
</script>
{% endraw %}
