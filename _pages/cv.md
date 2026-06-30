---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
---

<style>
.cv-print-btn {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  background: #4a7aac;
  color: #fff !important;
  padding: 8px 18px;
  border-radius: 6px;
  font-size: 0.9em;
  font-weight: 600;
  cursor: pointer;
  border: none;
  margin-bottom: 1.5em;
  text-decoration: none !important;
  transition: background 0.2s;
}
.cv-print-btn:hover {
  background: #2c5f8a;
}
@media print {
  .masthead, .page__footer, .author__avatar,
  .author__content, .author__urls-wrapper,
  .sidebar, .nav__list, .cv-print-btn,
  .page__meta, .page__share, .pagination,
  #main > .page__hero { display: none !important; }
  body { font-size: 12pt; }
  .page { padding: 0; margin: 0; }
  .page__inner-wrap { float: none; width: 100%; }
  .cv-header-box { background: #eef4fb !important; -webkit-print-color-adjust: exact; print-color-adjust: exact; }
  .edu-card, .project-card { box-shadow: none; border: 1px solid #ccc; page-break-inside: avoid; }
  .research-tag, .tool-tag, .edu-badge, .pub-badge, .pub-badge-first, .conf-badge {
    -webkit-print-color-adjust: exact; print-color-adjust: exact;
  }
  a { color: inherit; text-decoration: none; }
}
.cv-header-box {
  background: linear-gradient(135deg, #f8fafc 0%, #eef4fb 100%);
  border: 1px solid #dce8f5;
  border-radius: 10px;
  padding: 20px 24px;
  margin-bottom: 2em;
}
.cv-name {
  font-size: 1.6em;
  font-weight: 700;
  color: #1a2e44;
  margin: 0 0 4px 0;
}
.cv-title {
  font-size: 1em;
  color: #4a7aac;
  margin: 0 0 14px 0;
}
.cv-meta-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 6px 20px;
  font-size: 0.88em;
  color: #555;
}
.cv-meta-item {
  display: flex;
  align-items: center;
  gap: 6px;
}
.cv-section-title {
  font-size: 1.2em;
  font-weight: 700;
  color: #1a2e44;
  border-left: 4px solid #4a7aac;
  padding-left: 10px;
  margin: 1.8em 0 1em 0;
}
.research-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin: 0.5em 0;
}
.research-tag {
  background: #eef4fb;
  border: 1px solid #c5ddf5;
  color: #2971b8;
  padding: 5px 14px;
  border-radius: 20px;
  font-size: 0.88em;
  font-weight: 500;
}
.edu-card {
  border: 1px solid #e3eaf2;
  border-radius: 10px;
  padding: 18px 22px;
  margin-bottom: 14px;
  background: #fff;
  box-shadow: 0 1px 4px rgba(74,122,172,0.06);
}
.edu-card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 4px;
  margin-bottom: 6px;
}
.edu-card-school {
  font-size: 1.05em;
  font-weight: 700;
  color: #1a2e44;
}
.edu-card-date {
  font-size: 0.83em;
  color: #8a9db5;
  white-space: nowrap;
  font-weight: 500;
}
.edu-card-degree {
  font-size: 0.93em;
  color: #4a7aac;
  margin-bottom: 4px;
  font-weight: 500;
}
.edu-card-body {
  font-size: 0.87em;
  color: #666;
  line-height: 1.6;
}
.edu-badge {
  display: inline-block;
  background: #fff3cd;
  color: #856404;
  border: 1px solid #ffc107;
  padding: 2px 9px;
  border-radius: 10px;
  font-size: 0.8em;
  margin: 2px 3px 2px 0;
}
.project-card {
  border: 1px solid #e3eaf2;
  border-radius: 10px;
  padding: 18px 22px;
  margin-bottom: 16px;
  background: #fff;
  box-shadow: 0 1px 4px rgba(74,122,172,0.06);
}
.project-card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 10px;
}
.project-card-title {
  font-size: 1.02em;
  font-weight: 700;
  color: #1a2e44;
}
.project-card-date {
  font-size: 0.82em;
  color: #8a9db5;
  font-weight: 500;
  white-space: nowrap;
}
.project-content {
  font-size: 0.88em;
  color: #444;
  line-height: 1.7;
}
.project-content ul {
  margin: 0;
  padding-left: 0;
  list-style: none;
}
.project-content li {
  padding: 2px 0;
}
.project-tools {
  margin-top: 10px;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 5px;
  font-size: 0.84em;
}
.tools-label {
  color: #888;
  font-weight: 600;
}
.tool-tag {
  display: inline-block;
  background: #f0f7ff;
  border: 1px solid #c5ddf5;
  color: #2971b8;
  padding: 2px 9px;
  border-radius: 12px;
  font-size: 0.85em;
}
.pub-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.pub-item {
  padding: 12px 0;
  border-bottom: 1px solid #f0f4f8;
  font-size: 0.9em;
  line-height: 1.6;
}
.pub-item:last-child {
  border-bottom: none;
}
.pub-title {
  font-weight: 600;
  color: #1a2e44;
}
.pub-meta {
  color: #777;
  font-size: 0.87em;
  margin-top: 2px;
}
.pub-badge {
  display: inline-block;
  background: #e8f5e9;
  color: #2e7d32;
  border: 1px solid #a5d6a7;
  padding: 1px 7px;
  border-radius: 8px;
  font-size: 0.78em;
  margin-left: 4px;
  vertical-align: middle;
}
.pub-badge-first {
  background: #fff3e0;
  color: #e65100;
  border: 1px solid #ffcc80;
}
.conf-badge {
  display: inline-block;
  background: #f3e5f5;
  color: #6a1b9a;
  border: 1px solid #ce93d8;
  padding: 1px 7px;
  border-radius: 8px;
  font-size: 0.78em;
  margin-left: 4px;
  vertical-align: middle;
}
</style>

<button class="cv-print-btn" onclick="window.print()">⬇ 下载 / 打印 PDF</button>

<!-- ===================== HEADER ===================== -->
<div class="cv-header-box">
  <div class="cv-name">刘安琪 &nbsp;<span style="font-size:0.55em;font-weight:400;color:#4a7aac;">Anqi Liu</span></div>
  <div class="cv-title">博士研究生 · 三维重建与智能感知</div>
  <div class="cv-meta-grid">
    <div class="cv-meta-item">🎂 &nbsp;2002-01-27</div>
    <div class="cv-meta-item">🌏 &nbsp;安徽省安庆市</div>
    <div class="cv-meta-item">📞 &nbsp;+86-187-2619-7276</div>
    <div class="cv-meta-item">📧 &nbsp;<a href="mailto:anqii0127@gmail.com">anqii0127@gmail.com</a></div>
    <div class="cv-meta-item">🏫 &nbsp;韩国全南国立大学（Chonnam National University）</div>
    <div class="cv-meta-item">📍 &nbsp;韩国 · 光州</div>
  </div>
</div>

<!-- ===================== RESEARCH INTERESTS ===================== -->
<div class="cv-section-title">🔬 研究方向</div>

<div class="research-tags">
  <span class="research-tag">三维点云重建与处理</span>
  <span class="research-tag">三维高斯泼溅（3DGS）</span>
  <span class="research-tag">数字孪生</span>
  <span class="research-tag">点云语义分割与识别</span>
  <span class="research-tag">图神经网络（GNN）</span>
  <span class="research-tag">空间目标点定位</span>
  <span class="research-tag">6-DoF 位姿估计</span>
  <span class="research-tag">视觉-LiDAR融合感知</span>
  <span class="research-tag">农业机器人感知</span>
</div>

<!-- ===================== EDUCATION ===================== -->
<div class="cv-section-title">🎓 教育经历</div>

<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">韩国全南国立大学（Chonnam National University）</div>
    <div class="edu-card-date">2023.09 — 至今</div>
  </div>
  <div class="edu-card-degree">融合生物系统机械工程系 &nbsp;｜&nbsp; IT-Bio融合系统（第二专业）&nbsp;｜&nbsp; 硕博连读 · 韩国光州</div>
  <div class="edu-card-body">
    <strong>GPA：</strong>4.33 / 4.5<br>
    <strong>相关课程：</strong>图像处理应用、机器视觉、人工智能、高等应用数学、先进动力学、先进机器人学<br>
    <strong>荣誉奖项：</strong>
    <span class="edu-badge">2024 大学奖学金（6万元）</span>
    <span class="edu-badge">2025 人才培养学金（7万元）</span>
  </div>
</div>

<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">江西财经大学（Jiangxi University of Finance and Economics）</div>
    <div class="edu-card-date">2019.09 — 2023.09</div>
  </div>
  <div class="edu-card-degree">数理统计（拔尖人才实验班）&nbsp;｜&nbsp; 统计与数据科学学院 &nbsp;｜&nbsp; 本科 · 南昌</div>
  <div class="edu-card-body">
    <strong>GPA：</strong>3.49 / 4.50（专业排名 14/53）<br>
    <strong>相关课程：</strong>程序设计（C++）、贝叶斯统计、概率论、常微分方程、统计学习方法、机器学习<br>
    <strong>荣誉奖项：</strong>
    <span class="edu-badge">三好学生</span>
    <span class="edu-badge">优秀干部</span>
    <span class="edu-badge">校级奖学金</span>
  </div>
</div>

<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">西班牙庞培法布拉大学（Universitat Pompeu Fabra）</div>
    <div class="edu-card-date">2022.01 — 2022.07</div>
  </div>
  <div class="edu-card-degree">交换生 · 数据分析方向 · 巴塞罗那</div>
  <div class="edu-card-body">
    <strong>相关课程：</strong>R语言统计分析、统计学习、概率论
  </div>
</div>

<!-- ===================== RESEARCH PROJECTS ===================== -->
<div class="cv-section-title">🧪 硕博科研项目</div>

<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">冬季苹果园剪枝点识别</div>
    <div class="project-card-date">2024.06 — 2025.12</div>
  </div>
  <div class="project-content">
    <ul>
      <li>🔻 <strong>3D点云重建：</strong>利用多视角RGB-D图像对冬季休眠期苹果树进行密集三维点云采集与重建，构建高精度枝干几何模型</li>
      <li>🔻 <strong>结构骨架提取：</strong>设计基于拓扑感知的骨架提取算法，从稀疏噪声点云中精确还原苹果树主干与侧枝的树形结构</li>
      <li>🔻 <strong>深度学习网络：</strong>构建图神经网络（GNN）剪枝点预测框架，在三维骨架图上完成节点级语义分割与关键剪枝位点定位，并开展点云语义补全研究</li>
    </ul>
    <div class="project-tools">
      <span class="tools-label">🔧 技术栈：</span>
      <span class="tool-tag">图神经网络 GNN</span>
      <span class="tool-tag">骨架提取</span>
      <span class="tool-tag">语义分割</span>
      <span class="tool-tag">点云补全</span>
      <span class="tool-tag">RGB-D重建</span>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">基于高斯的离线到在线剪枝目标重定位</div>
    <div class="project-card-date">2025.12 — 至今</div>
  </div>
  <div class="project-content">
    <ul>
      <li>🔻 <strong>高斯重建：</strong>以3D Gaussian Splatting（3DGS）对果园离线场景进行高保真辐射场重建，建立包含结构感知先验的精密三维地图</li>
      <li>🔻 <strong>特征匹配：</strong>设计基于SuperPoint + LightGlue的跨域特征匹配流水线，实现高斯渲染视图与在线相机图像间的精准2D-3D对应关系</li>
      <li>🔻 <strong>6-DoF位姿估计：</strong>融合高斯场景深度渲染与单目深度估计，构建轻量级6自由度相机位姿回归器，支持在线剪枝目标的精确重定位与实时引导</li>
    </ul>
    <div class="project-tools">
      <span class="tools-label">🔧 技术栈：</span>
      <span class="tool-tag">3D Gaussian Splatting</span>
      <span class="tool-tag">SuperPoint</span>
      <span class="tool-tag">LightGlue</span>
      <span class="tool-tag">6-DoF位姿估计</span>
      <span class="tool-tag">特征匹配</span>
    </div>
  </div>
</div>

<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">基于拓扑结构的跨季节高斯果园地图持久树木地标定位</div>
    <div class="project-card-date">2026.04 — 至今</div>
  </div>
  <div class="project-content">
    <ul>
      <li>🔻 <strong>跨季节拓扑匹配：</strong>构建季节不变性拓扑图表征，在高斯地图框架内提取持久性树木地标，实现休眠期至生长期的跨季节稳健定位</li>
      <li>🔻 <strong>高斯地图持久化：</strong>研究3DGS地图的增量式更新与持久树木实体管理机制，支持季节变化下地标的语义一致性维护与长周期重定位</li>
    </ul>
    <div class="project-tools">
      <span class="tools-label">🔧 技术栈：</span>
      <span class="tool-tag">拓扑图匹配</span>
      <span class="tool-tag">3DGS地图</span>
      <span class="tool-tag">跨季节定位</span>
      <span class="tool-tag">地标持久化</span>
    </div>
  </div>
</div>

<!-- ===================== PUBLICATIONS ===================== -->
<div class="cv-section-title">📄 科研成果</div>

**期刊论文**

<ul class="pub-list">
  <li class="pub-item">
    <div class="pub-title">
      Realtime multi-RGBD SLAM framework for 3D reconstruction and phenotyping in large-scale apple orchards
      <span class="pub-badge">第二作者</span>
    </div>
    <div class="pub-meta">期刊论文 · 大规模果园实时多RGB-D SLAM三维重建与表型分析框架</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      Transformer-based cross-view LiDAR–Orthomosaic fusion for geo-localization and digital modeling in apple orchards
      <span class="pub-badge">第三作者</span>
    </div>
    <div class="pub-meta">期刊论文 · 基于Transformer的LiDAR与正射影像跨视角融合用于苹果园地理定位与数字建模</div>
  </li>
</ul>

**会议论文**

<ul class="pub-list">
  <li class="pub-item">
    <div class="pub-title">
      GNN-Driven Detection of Pruning Points in Apple Trees Using 3D Point Clouds
      <span class="pub-badge pub-badge-first">第一作者</span>
      <span class="conf-badge">KSAM 2025 Spring</span>
    </div>
    <div class="pub-meta">韩国农业机械学会春季学术大会 2025 · 基于GNN的苹果树三维点云剪枝点检测</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      2D-3D Matching for High-Precision Camera Localization in Apple Orchards Using SuperPoint and LightGlue
      <span class="pub-badge pub-badge-first">第一作者</span>
      <span class="conf-badge">KSAM 2025 Fall</span>
    </div>
    <div class="pub-meta">韩国农业机械学会秋季学术大会 2025 · 基于SuperPoint与LightGlue的果园高精度相机2D-3D定位</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      TopoSkel-GNN: A Topology-Aware Skeleton Graph Network for Efficient 3D Semantic Analysis
      <span class="pub-badge pub-badge-first">第一作者</span>
      <span class="conf-badge">KAIA 2025 Fall</span>
    </div>
    <div class="pub-meta">韩国人工智能学会秋季学术大会 2025 · 拓扑感知骨架图网络用于高效三维语义分析</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      StructGS: Structure-Aware 3D Gaussian Splatting for Complex Orchard Environments
      <span class="pub-badge pub-badge-first">第一作者</span>
      <span class="conf-badge">KSAM 2026 Spring</span>
    </div>
    <div class="pub-meta">韩国农业机械学会春季学术大会 2026 · 结构感知三维高斯泼溅用于复杂果园场景重建</div>
  </li>
</ul>

<!-- ===================== SKILLS ===================== -->
<div class="cv-section-title">🛠 技能</div>

<div class="research-tags">
  <span class="research-tag">Python</span>
  <span class="research-tag">C++</span>
  <span class="research-tag">PyTorch</span>
  <span class="research-tag">Open3D</span>
  <span class="research-tag">ROS 2</span>
  <span class="research-tag">COLMAP / SfM</span>
  <span class="research-tag">3DGS</span>
  <span class="research-tag">PCL</span>
  <span class="research-tag">PyTorch Geometric</span>
  <span class="research-tag">R</span>
  <span class="research-tag">MATLAB</span>
  <span class="research-tag">LaTeX</span>
</div>

<p style="font-size:0.88em;color:#777;margin-top:1em;">语言：普通话（母语）· 英语（学术写作与交流）· 韩语（日常交流）· 西班牙语（日常交流）</p>
