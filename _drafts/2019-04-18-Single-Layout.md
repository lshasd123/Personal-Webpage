---
#! ------------------基础信息-------------------
title: "Single Layout"
date: 2023-04-18T15:34:30-04:00
#* single版式
layout: single
#* 博客简介
excerpt: "A unique line of text to describe this post that will display in an archive listing and meta description with SEO benefits. You'll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated."

#! ------------------目录设置-------------------
#* 使用宽体版式
classes: # wide 此模式下会默认标题置顶
#* 显示目录
toc: true
#* 目录的名称
toc_label: "Directory"
#* 目录的图标
toc_icon: "far fa-book"
#* 目录始终显示在右侧
toc_sticky: true

#! ------------------博客头-------------------
#* 给博客添加位于最上方的图片
header:
  #* 单纯的添加一张图片
  # image: /assets/test/unsplash-image-3.jpg
  #* 添加一张图片，在图片上写title 和 excerpt
  overlay_image: /assets/test/unsplash-image-3.jpg
  #* 设置图片的不透明度，数字为放上黑色不透明版，也可以使用rgba(255, 0, 0, 0.5)设置不透明版颜色或使用linear-gradient(rgba(255, 0, 0, 0.5), rgba(0, 255, 255, 0.5))实现渐变色
  overlay_filter: 0.5
  #* 添加一个纯色图片，在图片上写title 和 excerpt
  # overlay_color: "#333"
  #* 图片描述
  image_description: "A description of the image"
  #* 图片标题，先是在右下角
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  #* 给图片增加一个More Info按钮
  actions:
    - label: "PDF"
      url: "https://unsplash.com"
#* 将博客头设置为视频
# header:
#   video:
#     id: playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB # 视频网址后缀
#     provider: youtube # 视频提供商，youtube, vimeo, google-drive, or bilibili

#! ------------------侧边栏设置-------------------
#* 是否显示作者信息
author_profile: true
#* 自定义侧边栏
sidebar:
  #* 侧边栏题目
  - title: "Title"
    #* 侧边栏图片
    image: /assets/test/unsplash-image-6.jpg
    #* 侧边栏图片的替代文字
    image_alt: "image"
    #* 题目下方的文字
    text: "Some text here."
  #* 侧边栏的另一个题目
  - title: "Another Title"
    #* 题目下方的文字
    text: "More text here."

#! ------------------底部设置-------------------
#* 设置分享链接
share: true

#! ------------------分别类和标签-------------------
categories:
  - blog
tags:
  - Jekyll
  - update

#! ------------------画廊-------------------
gallery:
    #* 图片的位置
  - url: /assets/test/unsplash-gallery-image-1.jpg
    #* 图片可到达的链接
    image_path: /assets/test/unsplash-gallery-image-1-th.jpg
    #* 图片替换文字
    alt: "placeholder image 1"
    #* 图片的标题
    title: "Image 1 title caption"
  - url: /blog/post-chat
    image_path: /assets/test/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: /assets/test/unsplash-gallery-image-3.jpg
    image_path: /assets/test/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"

gallery2:
  - url: https://flic.kr/p/8a6Ven
    image_path: https://farm2.staticflickr.com/1272/4697500467_8294dac099_q.jpg
    alt: "Black and grays with a hint of green"
  - url: https://flic.kr/p/8a738X
    image_path: https://farm5.staticflickr.com/4029/4697523701_249e93ba23_q.jpg
    alt: "Made for open text placement"
  - url: https://flic.kr/p/8a6VXP
    image_path: https://farm5.staticflickr.com/4046/4697502929_72c612c636_q.jpg
    alt: "Fog in the trees"

intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'

#! ------------------特征行-------------------
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
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
---

# 文档美化
## 图片的显示
### 使用include
<!-- * 使用include来添加图片 -->
<!-- image_path：图片路径 -->
<!-- alt：图片替代文字 -->
<!-- caption：图片标题 -->
{% include figure 
    image_path="/assets/test/unsplash-gallery-image-2.jpg" 
    alt="this is a placeholder image" 
    caption="This is a figure caption." %}

### 使用img
普通的添加图片形式不能使用markdown中的原本的形式
```markdown
![image-center](../assets/images/Li.jpg)
```
需要加上\{\{ site.url \}\}和\{\{ site.baseurl \}\}作为前缀

<!-- *使用img添加可以缩放的图片 -->
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/Li.jpg" alt="image-center" style="zoom:25%;" />

## 图片的对齐
<!-- *使用{: .align-center}、{: .align-left} {: .align-right}可以设置图片格式 -->
<!-- 设置{: .align-left} {: .align-right}时，文字部分为环绕 -->
<img src="{{ site.url }}{{ site.baseurl }}/assets/images/Li.jpg" alt="image-center" style="zoom:25%;" />{: .align-center}
无文字环绕

\\

\\

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/Li.jpg" alt="image-center" style="zoom:25%;" />{: .align-left}
文字环绕

\\

\\

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/Li.jpg" alt="image-center" style="zoom:25%;" />{: .align-right}
文字环绕

\\

\\


## 画廊的显示
需要配合头信息一起使用

<!-- * 使用include来添加画廊 -->
<!-- id：画廊的id,当存在多个画廊时，使用头文信息设置画廊的id -->
<!-- caption：画廊的标题 -->
<!-- layout：画廊的排版， “half”：两个图一行，“third”：三个图一行 “”：一个图一行-->
<!-- class："full"图片占满页面-->

{% include gallery caption="This is a sample gallery with Markdown support." %}
{% include gallery id="gallery2" layout="half" caption="This is a second gallery example with images hosted externally." %}

## 特征行的显示
<!-- *添加特征行 -->
<!-- id：特征行的名称 -->
<!-- type：特征行的排版，“left”, “center”, “right -->

需要配合头信息使用
<!-- *特征行可以只有文字描述 -->
{% include feature_row id="feature_row3" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row2" type="right" %}

{% include feature_row id="feature_row2" type="center" %}
详细见[splash-page.md](/Personal-Webpage/splash-page/)

You'll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

# 添加视频
<!-- *添加视频 -->
<!-- provider：视频提供商，youtube, vimeo, google-drive, or bilibili -->
<!-- id：视频网址的后缀 -->
{% include video id="playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB" provider="youtube" %}

<!-- 如果是bilibili，则添加/video/后的第一部分内容作为id -->
<!-- danmaku="1"表示打开弹幕 -->
<!-- https://www.bilibili.com/video/BV1qs41157ZZ/?p=12&vd_source=6a3f8a4ac0085023617b175841321a65 -->
{% include video id="BV1qs41157ZZ" provider="bilibili" danmaku="1"%}

<!-- 使用google-dive显示视频 -->
<!-- google-drive:https://drive.google.com/drive/my-drive -->
<!-- 其中id只放/file/d/后面的一段内容 -->
<!-- https://drive.google.com/file/d/18SfHoqYs5eTmK6a592sGI_I9GkPduGdA/view?usp=drive_link --> 
{% include video id="18SfHoqYs5eTmK6a592sGI_I9GkPduGdA" provider="google-drive" %}

<!-- 设置本地视频（无法播放） -->
<!-- <video width="500" controls>
  <source src="{{ site.url }}{{ site.baseurl }}/assets/videos/test.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video> -->

# 文本处理
## 文本排列
在文本下行添加{: .text-left}实现左对齐，{: .text-right}实现右对齐，{: .text-center}实现中间对齐，{: .text-justify}实现两端对齐，{: .text-nowrap}实现强制不换行

左对齐
{: .text-left}

右对齐
{: .text-right}

中间对齐
{: .text-center}

两端对齐
{: .text-justify}

强制不换行
{: .text-nowrap}

## 文本强调
在文本下方使用{: .notice}
{: .notice}

在文本下方使用{: .notice--primary}
{: .notice--primary}

在文本下方使用{: .notice--info}
{: .notice--info}

在文本下方使用{: .notice--warning}
{: .notice--warning}

在文本下方使用{: .notice--success}
{: .notice--success}

在文本下方使用{: .notice--danger}
{: .notice--danger}

# 添加按钮

`[按钮的名称]``(按钮对应的链接)``{按钮的样式}`其中按钮的样式也可以设置按钮的大小

包括的样式见：[按钮的样式](https://mmistakes.github.io/minimal-mistakes/docs/utility-classes/){: .btn .btn--info}



## Second Directory

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

# First Directory
Jekyll also offers powerful support for code snippets:

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
