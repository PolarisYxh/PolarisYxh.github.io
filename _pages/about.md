---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>
<!-- 硕士：北京航空航天大学 计算机学院 虚拟现实技术与系统国家重点实验室，导师是周彬副教授。
本科：北京航空航天大学 机械工程及自动化学院。 -->
 <!-- <a href='https://scholar.google.com/citations?user=WMkMTb4AAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=引用"></a>。 -->

# 研究领域
- 三维数字人生成及驱动
- 计算机图形图像算法
- aigc、大模型
- 三维视觉

<span class='anchor' id='-xl'></span>

# 🎓 学历
- *2019.09 - 2022.01 硕士*, <a href="https://vrlab.buaa.edu.cn/index.htm"><img class="jpeg" src="/images/bhcom.jpeg" width="23pt"></a> 北京航空航天大学 计算机学院 虚拟现实技术与系统国家重点实验室 导师周彬副教授
- *2015.09 - 2019.09 本科*, <a href="http://www.me.buaa.edu.cn/"><img class="jpeg" src="/images/bhme.jpeg" width="20pt"></a> 北京航空航天大学 机械工程及自动化学院
 

<span class='anchor' id='-gzsx'></span>

# 💻 工作实习
## *2022.05 - 至今*, 浙江同花顺智能科技有限公司
<div><h3>卡通形象生成-2022</h3></div>
<div class='paper-box'>

<div class='paper-box-image'><div><div class="badge">卡通生成</div><img src='images/cartoon.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	2022年，研发三维卡通虚拟人生成算法，用户输入人脸照片，输出一个三维卡通人脸模型。在该项目中负责人脸解析，以及卡通发型、卡通五官等部件的分类、变换参数生成算法及各器官组合变形平滑算法，对接美术处理卡通模型库得到各个器官降维后的blendshape，并部署上线。

</div>
</div>
<div><h3>室内场景重建-2022</h3></div>
<div class='paper-box'>
<div class='paper-box-image'>
<div><div class="badge">重建效果对比</div><img src='images/3d recon.png' alt="sym" width="100%"></div></div>

<div class='paper-box-text' markdown="1">

-	2022年负责公司内场景重建的demo开发，完成了从iphone手机录制视频到生成场景模型及纹理的重建流程，ios logger得到带内外参视频+neural recon三维重建+mvs-texturing进行三维重建。同时用colmap完成重建并对比。

</div>
</div>
<div><h3>头发生成-2023</h3></div>
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">头发生成</div><img src='images/hairgen.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	2023年，负责研发单视角三维头发丝发型生成算法，创建500G头发相关训练数据集，编写算法训练且优化了输入单视角图像生成头发丝三维模型的相关网络模型，并编写发型吸附头皮算法将发型和人头模型组合，使得单视角写实头发生成达到领先水平并部署。和美术对接加速头发模型制作并扩大训练数据集进一步提升性能及效果，并建立高质量发型库，并完成头发分类算法用于用户挑选。

</div>
</div>

<div><h3>关键点提升-2023</h3></div>
<div class='paper-box'>
<div class='paper-box-image'>
<div><div class="badge">关键点对比</div><img src='images/lmk5.png' alt="sym" width="100%"></div></div>
<div class='paper-box-image'>
<div><div class="badge">更多关键点结果</div><img src='images/lmk6.png' alt="sym" width="60%"></div>
</div>
<div class='paper-box-text' markdown="1">

-	2023年负责提升人脸五官及脸边缘关键点检测算法效果，使用metahuman animator的关键点检测算法制作精确的人脸关键点数据集，训练模型，得到精确的眉毛、眼睛眼球、口型、鼻子、鼻翼两侧褶皱、脸边缘及牙齿的关键点。同时使用开源的耳朵关键点数据集训练得到耳朵关键点模型，上述关键点效果堪比脸上在画点。

</div>
</div>

<div><h3>metahuman 3D人脸生成-2024</h3></div>
<div class='paper-box'><div class='paper-box-image'><div>
<!-- <div class="badge">3D metahuman</div> -->
<img src='images/3D1.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	2024年负责处理公司3D相机矩阵拍摄的人脸人体图像数据构建多视角图像-3D人脸模型数据集。编写了多视角图像的三维重建脚本，参考metahuman animator编写了metahuman拓扑的3dmm人脸模型拟合重建模型及纹理迁移的算法，自动化创建了metahuman拓扑的600组人脸图像-3D人脸模型数据集，模型效果和真人几乎一致，由于关键点准确，五官语义能够对准；为了进一步补充人脸图像-3D人脸模型数据集，采用3dmm人脸模型随机拟合人脸id并渲染合成图像的方法，处理得到关键点及置信度标注、深度图标注。上述数据集支持了稠密人脸关键点检测算法及gaussion head avatar算法。

</div>
</div>
<div><h3>metahuman 4D无标记点离线面捕-2024</h3></div>
<div class='paper-box'><div>
<div class="badge">4D无标记点离线面捕</div>
<!-- <video width="640" controls>
  <source src="images/4D_1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video> -->
<!-- <video width="640" controls>
  <source src="https://www.bilibili.com/video/BV1tzA5eWEvX/?vd_source=e428689d58bc7fbca7c1db2f540c0123" type="video/mp4" width="100%">
  Your browser does not support the video tag.
</video> -->
<iframe src="//player.bilibili.com/player.html?bvid=BV1tzA5eWEvX&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
<div class='paper-box-text' markdown="1">

-	2024年负责处理4D相机矩阵拍摄的语音人脸多视角动画，构建语音-4D表情动画数据集。编写了从多视角人脸三维重建开始拟合人脸4D图像得到174维表情系数、球谐光照、位姿的离线无标记点面捕算法，创建了多个人脸4D图像数据-metahuman拓扑的4D动画数据集，完成的可微渲染优化算法得到的动画稳定没有抖动且嘴型眼睛精确，效果达到metahuman animator水平。上述数据集支持大屏虚拟人及虚拟试衣项目的语音驱动口型算法。

</div>
</div>

<div><h3>服装生成-2025</h3></div>
<div class='paper-box'>
<div>
<div class="badge">服装仿真</div>

<!-- <video width="640" controls>
  <source src="https://www.bilibili.com/video/BV1UzA5eWExs/" type="video/mp4" width="100%">
  Your browser does not support the video tag.
</video> -->
<iframe src="//player.bilibili.com/player.html?bvid=BV1UzA5eWExs&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>
<div class='paper-box-text' markdown="1">

-	2024年至今负责单视角图像的服装版型生成算法，输入穿衣图像，输出服装版型及缝合信息。使用warp4d对版片服装缝合后进行物理仿真并渲染得到合成试衣图像，使用comfyui的2d虚拟试衣流程将合成图像转为真实图像，构建了真实的人体服装图像-服装版型数据的数据集；将原版模型的编码器替换为用mae预训练的1b vit人体编码器，训练新的服装版型1B生成大模型，解决原版模型不能泛化到真实人体图像的问题

</div>
</div>

<div><h3>机械臂自主操作家具仿真 Unity 3D-2020</h3></div>
<div class='paper-box'><div>
<div class="badge">制作工具</div>
<!-- <video width="640" controls>
  <source src="images/4D_1.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video> -->
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=424775460&bvid=BV1R3411W7rX&cid=549893691&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
<!-- <video width="640" controls>
  <source src="https://www.bilibili.com/video/BV1R3411W7rX?t=22.2" type="video/mp4">
  Your browser does not support the video tag.
</video> -->
</div>
<div class='paper-box-text' markdown="1">

-	负责并实现在仿真环境下机械臂拉抽屉、开门的任务。在Unity中搭建kinova机械臂仿真环境及家居场景物理仿真模型。训练gg-cnn深度神经网络，使机械臂视觉识别家具部件抓取点。编写Moveit机械臂控制代码，根据抓取点和机械臂相对位姿速度伺服控制机械臂实现拉抽屉、开门等任务。迁移到真实机械臂完成上述任务。

</div>
</div>
<span class='anchor' id='-lwzl'></span>

# 📝 专利

<!-- ### 英文
---
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Sensors 2022</div><img src='images/sensors2022.svg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

-	`Jian Tang`, Rongbiao Wang, Gongzhe Qiu, Yu Hu, Yihua Kang. Mechanism of magnetic flux leakage detection method based on the slotted ferromagnetic lift-off layer. *Sensors*, 2022, 22(9): 3587. (JCR:Q2; IF:3.847)  
[[网页]](https://dx.doi.org/10.3390/s22093587) [[预览]](https://github.com/tangjyan/tangjyan.github.io/blob/main/pdf/TangJ-2022-Mechanism%20of%20Magnetic%20Flux%20Leakage%20Detection%20Method%20Based%20on%20the%20Slotted.pdf) [[下载]](/pdf/TangJ-2022-Mechanism%20of%20Magnetic%20Flux%20Leakage%20Detection%20Method%20Based%20on%20the%20Slotted.pdf)

</div>
</div>

- Bo Feng, Jianbo Wu, Hongming Tu, `Jian Tang`, Yihua Kang. A Review of Magnetic Flux Leakage Nondestructive Testing. *Materials*. 2022, 15 (20): 7362. (JCR:Q1; IF:3.748)  
[[网页]](https://dx.doi.org/10.3390/ma15207362) [[预览]](https://github.com/tangjyan/tangjyan.github.io/blob/main/pdf/FengB-2022-A%20Review%20of%20Magnetic%20Flux%20Leakage%20Nondestructive%20Testing.pdf) [[下载]](/pdf/FengB-2022-A%20Review%20of%20Magnetic%20Flux%20Leakage%20Nondestructive%20Testing.pdf) -->

<!-- ### 中文
---

- 	`唐健`，王荣彪，康宜华. 大提离漏磁无损检测方法. *无损检测*. 2022,44(4): 67. (核心期刊)  
[[网页]](https://dx.doi.org/10.11973/wsjc202204000) [[预览]](https://github.com/tangjyan/tangjyan.github.io/blob/main/pdf/%E5%94%90%E5%81%A5-2022-%E5%A4%A7%E6%8F%90%E7%A6%BB%E6%BC%8F%E7%A3%81%E6%97%A0%E6%8D%9F%E6%A3%80%E6%B5%8B%E6%96%B9%E6%B3%95.pdf) [[下载]](/pdf/%E5%94%90%E5%81%A5-2022-%E5%A4%A7%E6%8F%90%E7%A6%BB%E6%BC%8F%E7%A3%81%E6%97%A0%E6%8D%9F%E6%A3%80%E6%B5%8B%E6%96%B9%E6%B3%95.pdf)    -->
<!-- ### 专利 -->
---
- 杨新航, `杨新航`. 一种虚拟人三维头发丝发型的生成方法及系统. 
<!-- [网页]](https://cprs.patentstar.com.cn/Search/Detail?ANE=9IBC8DFA9GCB8DEA6FAA9HHFCICA1BAA9ACB9EGC9GAA6AAA) -->
- 杨新航, `杨新航`. 用户形象生成方法、相关装置及计算机程序产品

<span class='anchor' id='-ryjx'></span>

# 🏅 荣誉奖项
- *2020* 获得 校级优秀奖学金 `一等奖`  


<span class='anchor' id='-xshy'></span>

# 🏛️ 学术会议
- InstanceFusion: Real-time Instance-level 3D Reconstruction Using a Single RGBD Camera,pacific graphic 2020,ccf-B



