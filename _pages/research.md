---
permalink: /research/
title: "Research"
layout: single
author_profile: true
show_title: false
classes:  wide
---
<!-- 添加目录 -->
{% include toc title="Contents" %}
<!-- 添加折叠框 -->
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .collapsible {
      /* 背景颜色设置设置 */
      background-color: #777;
      color: white;
      cursor: pointer;
      /* 调整 padding 大小 */
      padding: 0.65em;
      height: auto; /* 自适应高度 */
      /* 宽度设置 */
      width: auto;
      border: 0px solid #555;
      justify-content: space-between; /* 文本两端对齐 */
      /* 字体设置 */
      outline: none;
      font-size: 16px;
      /* 圆角设置 */
      border-top-left-radius: 5px;
      border-top-right-radius: 5px;
      border-bottom-left-radius: 5px; 
      border-bottom-right-radius: 5px; 
      margin-bottom: 1px;
    }

    .content {
      padding: 0 12px;
      display: none;
      overflow: hidden;
      background-color: #f1f1f1;
      border-top-left-radius: 10px;
      border-top-right-radius: 10px;
      border-bottom-left-radius: 10px; 
      border-bottom-right-radius: 10px; 
    }

    .content p {
      margin-top: 20px; /* 调整文本距离上边的距离 */
      margin-bottom: 20px; /* 调整文本距离上边的距离 */
      margin-left: 10px; /* 调整文本距离上边的距离 */
      margin-right: 10px; /* 调整文本距离上边的距离 */
    }
  </style>
  <style>
    h3 {
      margin-top: 0.5em; /* 自定义行间距，可以根据需要调整 */
    }
    h2 {
      margin-top: 3em; /* 自定义行间距，可以根据需要调整 */
    }
</style>
</head>

<script>
  function toggleContent(contentId) {
    var content = document.getElementById(contentId);
    if (content.style.display === 'block') {
      content.style.display = 'none';
    } else {
      content.style.display = 'block';
    }
  }
</script>

## Working Papers
<!-- **************************research************************** -->
### [Hierarchical Trajectory Planning Based on Adaptive Motion Primitives and Bilevel Corridor]()
{: .text-justify}
with Wenshuo Wang, Boyang Wang, Haijie Guan, Haiou Liu, Shaobin Wu, and Huiyan Chen.\\
**IEEE Transactions on Vehicular Technology** (under review)

<button class="collapsible" onclick="toggleContent('HMPabstract')"><strong>Abstract</strong></button>
[PDF](){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0);){: onclick="HMPbib()"}{: .btn .btn--inverse .btn--small}
[Video]({{ site.url }}{{ site.baseurl }}/research/HMP){: .btn .btn--primary .btn--small} 
<!-- [More Info](){: .btn .btn--primary .btn--small} -->
<div class="content" id="HMPabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> This paper presents an efficient and risk-aware search-optimization hierarchical trajectory planning method for automated vehicles in different road structure. The proposed approach incorporates a time-series motion risk field, capturing diverse road structures through a spatiotemporal map. Then, an adaptive motion primitive is developed, dynamically adjusting action time windows based on evolving risk and expected deviation during the search process. This enables efficient and accurate initial trajectory generation. Additionally, a bilevel corridor is introduced to extract the drivable area and rerepresent the risk field, enabling trajectory smoothing to consider motion risk without resorting to non-convex optimization methods. The method is validated through simulation in structured and unstructured scenarios, demonstrating improved efficiency, flexibility, and optimization quality compared to fixed-step search and single-level corridor-based optimization approaches.
    </p>
</div>

<script>
  function HMPbib() {
    var popupContent = "Addendum After Publication of the Paper";
    // 创建一个新的窗口
    var popupWindow = window.open("", "_blank", "width=400, height=300");
    // 在新窗口中写入文本内容
    popupWindow.document.write("<p>" + popupContent + "</p>");
  }
</script>

<!-- **************************research************************** -->
### [Selecting Maneuver at Spatiotemporal Domain: A Generalized Framework Integrating Decision-making and Planning for Urban Driving]()
{: .text-justify}
with Xiang Zhang, Wenshuo Wang, Boyang Wang, Chao Lv, and Haiou Liu.\\
**IEEE Transactions on Intelligent Transportation Systems** (under review)

<button class="collapsible" onclick="toggleContent('BCPabstract')"><strong>Abstract</strong></button>
[PDF](){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0); ){: onclick="BCPbib()"}{: .btn .btn--inverse .btn--small}
[Video]({{ site.url }}{{ site.baseurl }}/research/BC){: .btn .btn--primary .btn--small}
<!-- [More Info](){: .btn .btn--primary .btn--small} -->

<div class="content" id="BCPabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> The decision-making and planning modules in the autonomous driving system are highly interconnected to cope with various urban driving scenarios. Inconsistent cognition of the drivable area between them can lead to system failure or even pose safety risks. This work bridges the gap and tightly integrates the two modules into a generalizable framework by modelling and estimating maneuvers from various scenarios in the spatiotemporal domain. We abstract different environment elements into a unified spatiotemporal map. Based on this, a novel structure, Behavior Cells (BCs), is presented to describe maneuvers’ domain within lanes in a unit-based manner, and feasible homotopies can be semantically enumerated by the combination of BCs. By modelling as the finite horizon Markov decision process (FHMDP), the BCs combination with the highest benefits is transferred as boundary constraints to the planning process. Finally, the dynamic two-stage optimization uses the simplified mixed-integer quadratic program (MIQP) stage and risk-aware nonlinear programming (NLP) stage to hierarchical generate trajectory with high real-time and convergent. We demonstrate the effectiveness of our framework via simulated experiments with various complex urban driving scenarios, outperforming state-of-the-art baselines in metrics of reliability, real-time, efficiency, comfort, and low-risk performance.
    </p>
</div>

<script>
  function BCPbib() {
    var popupContent = "Addendum After Publication of the Paper";
    // 创建一个新的窗口
    var popupWindow = window.open("", "_blank", "width=400, height=300");
    // 在新窗口中写入文本内容
    popupWindow.document.write("<p>" + popupContent + "</p>");
  }
</script>



## Selected Published Papers
<!-- **************************research************************** -->
### [Modeling and Quantitative Evaluation Method of Environmental Complexity for Measuring Autonomous capabilities for Unmanned Ground Vehicles]()
{: .text-justify}
with Shaobin Wu, Jianwei Gong, Zexin Yan\\
**Unmanned Systems** 

<button class="collapsible" onclick="toggleContent('EECabstract')"><strong>Abstract</strong></button>
[PDF](){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0);){: onclick="EECbib()"}{: .btn .btn--inverse .btn--small}
<!-- [More Info](){: .btn .btn--primary .btn--small} -->

<div class="content" id="EECabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> This paper proposes a sampling-based multi-dimensional entropy hierarchical evaluation method to evaluate the environmental complexity for measuring autonomous capabilities of unmanned ground vehicles. Through establishing the multi-dimensional environment model, the complexity of environmental elements in various dimensions is measured by combining the analytic hierarchy process and the improved gravitational field model. Based on the graph entropy and the environment segmentation sampling strategy, the environmental complexity is comprehensively evaluated from the two perspectives of the objective complexity of the environmental structure and the subjective complexity of environmental characteristics. The evaluation of the actual test environment shows that the environmental complexity evaluation model can effectively reflect the individual complexity differences of environmental elements, and achieve the comprehensive complexity evaluation of the environment including multiple test scenarios, which provides a basis for the test scenario design and measuring autonomous capabilities of unmanned ground vehicles.
    </p>
</div>

<script>
  function EECbib() {
    var popupContent = "@article\{wu2023modeling,<br>title=\{Modeling and Quantitative Evaluation Method of Environmental Complexity for Measuring Autonomous Capabilities of Military Unmanned Ground Vehicles\},<br>author=\{Wu, Shaobin and Li, Shihao and Gong, Jianwei and Yan, Zexin\},<br>journal=\{Unmanned Systems\},<br>volume=\{11\},<br>number=\{04\},<br>pages=\{367--382\},<br>year=\{2023\},\npublisher=\{World Scientific\}\}";
    // 创建一个新的窗口
    var popupWindow = window.open("", "_blank", "width=400, height=300");
    // 在新窗口中写入文本内容
    popupWindow.document.write("<p>" + popupContent + "</p>");
  }
</script>


## Work in Progress
### [PHISI: Suspension-aware Vehicle-Terrain Contact model for Pose Estimation in Unstrucured Scenarios]()
with Ji Li.

<button class="collapsible" onclick="toggleContent('PEabstract')"><strong>Abstract</strong></button>
[PDF](){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0); ){: onclick="PEbib()"}{: .btn .btn--inverse .btn--small}
[Video]({{ site.url }}{{ site.baseurl }}/research/PHISI){: .btn .btn--primary .btn--small} 
<!-- [More Info](){: .btn .btn--primary .btn--small} -->

<div class="content" id="PEabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> 
    </p>
</div>

<script>
  function PEbib() {
    var popupContent = "Addendum After Publication of the Paper";
    // 创建一个新的窗口
    var popupWindow = window.open("", "_blank", "width=400, height=300");
    // 在新窗口中写入文本内容
    popupWindow.document.write("<p>" + popupContent + "</p>");
  }
</script>



## Patents
- A method and system for evaluating the quality of unmanned vehicle path planning.\[P\] CN113759938B, 2021
- A method for autonomous safety behavior detection in unmanned off-road vehicles.\[P\](Work in Progress)
- A method for detecting the safety behavior of unmanned off-road vehicles overcoming obstacles.\[P\](Work in Progress)