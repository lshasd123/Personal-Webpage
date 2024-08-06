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
    .justified-text {
            text-align: justify;
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

## Selected Published Papers
<!-- **************************research************************** -->
### [Hierarchical Trajectory Planning Based on Adaptive Motion Primitives and Bilevel Corridor](https://ieeexplore.ieee.org/abstract/document/10574321)
{: .text-justify}
with Wenshuo Wang, Boyang Wang, Haijie Guan, Haiou Liu, Shaobin Wu, and Huiyan Chen.\\
**IEEE Transactions on Vehicular Technology**

<button class="collapsible" onclick="toggleContent('HMPabstract')"><strong>Abstract</strong></button>
[PDF](https://ieeexplore.ieee.org/abstract/document/10574321){: .btn .btn--inverse .btn--small}
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
  var popupContent = `@ARTICLE{10574321,
  author={Li, Shihao and Wang, Wenshuo and Wang, Boyang and Guan, Haijie and Liu, Haiou and Wu, Shaobin and Chen, Huiyan},
  journal={IEEE Transactions on Vehicular Technology}, 
  title={Hierarchical Trajectory Planning Based on Adaptive Motion Primitives and Bilevel Corridor}, 
  year={2024},
  volume={},
  number={},
  pages={1-17},
  keywords={Vehicle dynamics;Roads;Trajectory;Spatiotemporal phenomena;Dynamics;Trajectory planning;Optimization;Trajectory planning;motion risk;motion primitives;corridor-based optimization},
  doi={10.1109/TVT.2024.3420159}}`;
  // 创建一个新的窗口
  var popupWindow = window.open("", "_blank", "width=400, height=300");
  // 在新窗口中写入文本内容
  popupWindow.document.write("<pre>" + popupContent + "</pre>");
}
</script>

<!-- **************************research************************** -->
### [Multi-Vehicle Collaborative Lane Changing Based on Multi-Agent Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/10574321)
{: .text-justify}
with Xiang Zhang, Boyang Wang, Mingxuan Xue, Zhiwei Li, Haiou Liu\\
**2024 IEEE Intelligent Vehicles Symposium (IV)**

<button class="collapsible" onclick="toggleContent('HMPabstract')"><strong>Abstract</strong></button>
[PDF](https://ieeexplore.ieee.org/abstract/document/10588529){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0);){: onclick="MCLCbib()"}{: .btn .btn--inverse .btn--small}
<!-- [More Info](){: .btn .btn--primary .btn--small} -->
<div class="content" id="HMPabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> Achieving safe lane changing is a crucial function of autonomous vehicles, with the complexity and uncertainty of interaction involved. Learning-based approaches and vehicle collaboration techniques can enhance vehicles’ awareness of the dynamic environment, thereby enhancing the interactive capabilities. Therefore, this paper proposes a Multi-Agent Reinforcement Learning (MARL) approach to coordinate connected vehicles in reaching their respective lane changing targets. Vehicle state, scene elements, potential risk, and intention information are abstracted into highly expressive vectorized inputs. Based on this, a lightweight parameter-sharing network framework is designed to learn safe and robust cooperative lane changing policies. To address the challenges arising from multi-objects and multi-targets, a Prioritized Action Extrapolation (PAE) mechanism is employed to train the network. Through priority assignment and action extrapolation, the proposed MARL approach can optimize the decision sequence dynamically and enhance the interaction in multi-vehicle scenarios, thereby improving the vehicles’ intention attainment rate. Simulated experiments in 2-lane and 3-lane scenarios have been conducted to verify the adaptability and performance of the proposed MARL method.
    </p>
</div>

<script>
  function MCLCbib() {
  var popupContent = `@INPROCEEDINGS{10588529,
  author={Zhang, Xiang and Li, Shihao and Wang, Boyang and Xue, Mingxuan and Li, Zhiwei and Liu, Haiou},
  booktitle={2024 IEEE Intelligent Vehicles Symposium (IV)}, 
  title={Multi-Vehicle Collaborative Lane Changing Based on Multi-Agent Reinforcement Learning}, 
  year={2024},
  volume={},
  number={},
  pages={1214-1221},
  keywords={Training;Space vehicles;Extrapolation;Uncertainty;Simulation;Collaboration;Reinforcement learning},
  doi={10.1109/IV55156.2024.10588529}}`;
  // 创建一个新的窗口
  var popupWindow = window.open("", "_blank", "width=400, height=300");
  // 在新窗口中写入文本内容
  popupWindow.document.write("<pre>" + popupContent + "</pre>");
}
</script>

<!-- **************************research************************** -->
### [Modeling and Quantitative Evaluation Method of Environmental Complexity for Measuring Autonomous Capabilities for Unmanned Ground Vehicles]()
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

## Working Papers

<!-- **************************research************************** -->
### [Optimization-Based Spatiotemporal Trajectory Planning with Behavior Cells for Autonomous Driving](https://lshasd123.github.io/Behavior-Cells/)
{: .text-justify}
with Wenshuo Wang, Zhide Zhang, Xin Xia, Boyang Wang, Chao Lu and Haiou Liu.\\
**IEEE Transactions on Intelligent Transportation Systems** (under review)

<button class="collapsible" onclick="toggleContent('BCPabstract')"><strong>Abstract</strong></button>
[PDF](){: .btn .btn--inverse .btn--small}
[Bib](javascript:void(0); ){: onclick="BCPbib()"}{: .btn .btn--inverse .btn--small}
[Video]({{ site.url }}{{ site.baseurl }}/research/BC){: .btn .btn--primary .btn--small}
<!-- [More Info](){: .btn .btn--primary .btn--small} -->

<div class="content" id="BCPabstract">
  <p style="text-align: justify;">
    <strong>Abstract:</strong> Achieving safe and executable trajectory planning in traffic scenarios necessitates considering vital environmental elements, ego behaviors, and vehicle inematics, which poses challenges of real-time performance and convergence for optimization-based methods. To address these issues, we propose an optimization-based trajectory planning framework that handles environmental elements and provides heuristic behavior constraints at the spatiotemporal drivable domain level, followed by progressively optimization to achieve fast and stable convergence. Specifically, considering vehicle motion capabilities and the tactical decisions for various environmental elements, we first partition the spatiotemporal domain into modular drivable cells with behavior semantics, refer to Behavior Cells (BCs). All feasible candidate behaviors are then rapidly enumerated through BCs combinations.  ubsequently, the Finite-Horizon Markov Decision Process (FHMDP) is utilized to model and evaluate each behavior in the spatiotemporal drivable domain, with the optimal BCs combination serving as heuristic constraints. Finally, we utilize a dynamic two-stage optimization approach to progressively satisfy the planning-related requirements, generating trajectories within the selected BCs combination with fast convergence. Simulation in various typical traffic demonstrate that the proposed method showcases stable reliability and realtime performance compared to the baselines under different traffic densities. On-road experiments further validate the effectiveness of the proposed method in real-world traffic scenarios. Website: https://lshasd123.github.io/Behavior-Cells/.
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


## Work in Progress
### [PHISI: Suspension-aware Vehicle-Terrain Contact model for Pose Estimation in Unstructured Scenarios]()
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
- <div class="justified-text">
        <p>A method for safety verification and control in unmanned off-road vehicles navigating through obstacle terrain. NO. 202311088086.3, China.</p>
  </div>
- <div class="justified-text">
        <p>A method for safety behavior detection in autonomous off-road vehicles. NO. 202311088074.0, China.</p>
  </div>
- <div class="justified-text">
        <p>A method and system for evaluating the quality of unmanned vehicle path planning. NO. 202221836601.2, China.</p>
  </div>
- <div class="justified-text">
        <p>A convective heat exchange device based on vortex low-speed circulation air supply. NO. 201910247180.6, China.</p>
  </div>