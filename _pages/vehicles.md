---
title: "Umanned Vehicles Showcase"
layout: single
classes: wide
permalink: /vehicles/
author_profile: true
show_title: false
intro: 
  - excerpt: 'This page introduces the autonomous vehicles that I have been involved in designing, building, or debugging.'

#* 特征行
feature_row:
    #* 图片路径
  - image_path: assets/test/unsplash-gallery-image-1-th.jpg
    #* 图片标题
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    #* 图片替换文字
    alt: "placeholder image 1"
    #* 图片标题
    title: "Placeholder 1"
    #* 图片描述
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    #* 按钮的链接
    url: /blog/post-chat
    #* 按钮的文字
    btn_label: "Chat"
    #* 按钮的样式，更多样式见https://mmistakes.github.io/minimal-mistakes/docs/utility-classes/#buttons
    btn_class: "btn--primary"
feature_6t:
  - image_path: /assets/images/6t.png
    alt: "6t"
    title: "The Heavy Tracked Unmanned Ground Vehicle (HTUGV)"
    excerpt: 'HTUGV is a dual-sided independently driven series-parallel hybrid tracked platform. It has the capability for autonomous driving and remote control in unstructured environments.'
    url: "#test-link"
    btn_label: "More Info"
    btn_class: "btn--primary"
feature_DF:
  - image_path: /assets/images/DF.png
    alt: "ADF"
    title: "The Pure Electric Autonomous Wheeled Vehicle (ADF)"
    excerpt: 'ADF is an autonomous vehicle modified based on a commercially available electric vehicle. It is capable of autonomous navigation in both structured and unstructured scenarios.'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_TANG:
  - image_path: /assets/images/Tang.png
    alt: "tang"
    title: "The Hybrid Power Data Collection SUV (TANG)"
    excerpt: 'TANG is a data collection vehicle modified based on a commercially available SUV. It is capable of performing data collection tasks in both structured and unstructured scenarios.'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_SV:
  - image_path: /assets/images/SV.png
    alt: "sv"
    title: "The Mini Ackermann-steered Autonomous Vehicle (MWV)"
    excerpt: 'MWV is a mini pure electric Ackermann-steered rear-wheel-drive autonomous wheeled vehicle. It is utilized for performance testing of autonomous algorithms.'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

<!-- *添加特征行 -->
<!-- id：特征行的名称 -->
<!-- type：特征行的排版，“left”, “center”, “right -->

<!-- *如果特征行可以只有文字描述 -->
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .container {
            display: inline-block; /* 让容器只占用实际内容的宽度 */
            text-align: center; /* 内容左对齐 */
            margin: 0 100px; /* 左右设置间隙 */
        }
    </style>
    <title>Centered Text with Margin</title>
</head>

  <div class="container">
      <p>This page introduces the autonomous vehicles that I have been involved in designing, building, or debugging.</p>
  </div>
---

{% include feature_row id="feature_6t" type="left" %}

{% include feature_row id="feature_DF" type="right" %}

{% include feature_row id="feature_TANG" type="left" %}

{% include feature_row id="feature_SV" type="right" %}