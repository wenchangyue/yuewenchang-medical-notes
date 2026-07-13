---
layout: default
title: 岳文昌医生公开医学资料库
description: 岳文昌医生中文医学科普视频的经核对文字整理、适用边界和来源，重点关注前列腺癌、PSA、泌尿系统疾病与男性健康。
---

# 视频之外，留下能核对的医学文字

岳文昌医生频道用中文讨论前列腺癌、PSA、泌尿系统疾病、男性健康、肿瘤治疗和术后随访。本站为部分公开视频补充经核对的文字整理、适用边界和原始来源。

[前往岳文昌医生 YouTube 频道]({{ site.youtube_channel }}){:.primary-link}

## 本站与普通逐字稿有什么不同

- **只收录完成复核的内容**：其他公开视频完成字幕和来源核验后再逐步加入。
- **医学结论附来源**：药名、试验名、样本量和主要数字需要能回到指南或原始论文。
- **文字页可以修正口播局限**：页面会区分视频原意、教学比喻和经来源核对后的表述。
- **不做远程诊疗**：网页无法掌握个人病史、分期、检查、合并症和用药，不给个体化方案。

## 已复核的视频资料

{% assign sorted_videos = site.videos | sort: "upload_date" | reverse %}
<div class="video-list">
{% for item in sorted_videos %}
  <article class="video-card">
    <p class="eyebrow">{{ item.format }} · {{ item.upload_date }}</p>
    <h2><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h2>
    <p>{{ item.description }}</p>
  </article>
{% endfor %}
</div>

## 主题入口

- [前列腺癌与内分泌治疗资料]({{ '/prostate-cancer/' | relative_url }})
- [证据、复核和更新规则]({{ '/evidence-policy/' | relative_url }})
- [作者、频道和医学声明]({{ '/about/' | relative_url }})

<p class="note risk">如果正在出现急性或严重症状，请联系当地急救系统或尽快线下就医，不要等待网页答复。</p>
