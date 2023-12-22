---
title: "Splash Page"
layout: splash
#* 如果把permalink改为/就可以作为首页
permalink: /splash-page/
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/test/unsplash-image-1.jpg
  actions:
    - label: "Learn More"
      url: "/terms/"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'

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
  - image_path: /assets/test/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/test/unsplash-gallery-image-3-th.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row2:
  - image_path: /assets/test/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/test/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/test/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

<!-- *添加特征行 -->
<!-- id：特征行的名称 -->
<!-- type：特征行的排版，“left”, “center”, “right -->

需要配合头信息使用
<!-- *如果特征行可以只有文字描述 -->
{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}