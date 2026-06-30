---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
---

<style>
/* ── Language toggle ── */
.cv-topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1.4em;
  flex-wrap: wrap;
  gap: 8px;
}
.lang-toggle {
  display: inline-flex;
  border: 2px solid #4a7aac;
  border-radius: 20px;
  overflow: hidden;
}
.lang-toggle button {
  padding: 5px 18px;
  border: none;
  background: transparent;
  color: #4a7aac;
  cursor: pointer;
  font-size: 0.88em;
  font-weight: 600;
  transition: background 0.2s, color 0.2s;
}
.lang-toggle button.active {
  background: #4a7aac;
  color: #fff;
}
/* default: show CN, hide EN */
.lang-en { display: none; }
/* when EN is active, flip */
body.cv-lang-en .lang-en { display: revert !important; }
body.cv-lang-en .lang-cn { display: none !important; }

/* ── Print button ── */
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
  text-decoration: none !important;
  transition: background 0.2s;
}
.cv-print-btn:hover { background: #2c5f8a; }

/* ── Print media ── */
@media print {
  .masthead, .page__footer, .author__avatar,
  .author__content, .author__urls-wrapper,
  .sidebar, .nav__list, .cv-topbar,
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

/* ── Header box ── */
.cv-header-box {
  background: linear-gradient(135deg, #f8fafc 0%, #eef4fb 100%);
  border: 1px solid #dce8f5;
  border-radius: 10px;
  padding: 20px 24px;
  margin-bottom: 2em;
}
.cv-name { font-size: 1.6em; font-weight: 700; color: #1a2e44; margin: 0 0 4px 0; }
.cv-title { font-size: 1em; color: #4a7aac; margin: 0 0 14px 0; }
.cv-meta-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 6px 20px;
  font-size: 0.88em;
  color: #555;
}
.cv-meta-item { display: flex; align-items: center; gap: 6px; }

/* ── Section title ── */
.cv-section-title {
  font-size: 1.2em;
  font-weight: 700;
  color: #1a2e44;
  border-left: 4px solid #4a7aac;
  padding-left: 10px;
  margin: 1.8em 0 1em 0;
}

/* ── Research tags ── */
.research-tags { display: flex; flex-wrap: wrap; gap: 8px; margin: 0.5em 0; }
.research-tag {
  background: #eef4fb;
  border: 1px solid #c5ddf5;
  color: #2971b8;
  padding: 5px 14px;
  border-radius: 20px;
  font-size: 0.88em;
  font-weight: 500;
}

/* ── Education cards ── */
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
.edu-card-school { font-size: 1.05em; font-weight: 700; color: #1a2e44; }
.edu-card-date { font-size: 0.83em; color: #8a9db5; white-space: nowrap; font-weight: 500; }
.edu-card-degree { font-size: 0.93em; color: #4a7aac; margin-bottom: 4px; font-weight: 500; }
.edu-card-body { font-size: 0.87em; color: #666; line-height: 1.6; }
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

/* ── Project cards ── */
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
.project-card-title { font-size: 1.02em; font-weight: 700; color: #1a2e44; }
.project-card-date { font-size: 0.82em; color: #8a9db5; font-weight: 500; white-space: nowrap; }
.project-content { font-size: 0.88em; color: #444; line-height: 1.7; }
.project-content ul { margin: 0; padding-left: 0; list-style: none; }
.project-content li { padding: 2px 0; }
.project-tools {
  margin-top: 10px;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 5px;
  font-size: 0.84em;
}
.tools-label { color: #888; font-weight: 600; }
.tool-tag {
  display: inline-block;
  background: #f0f7ff;
  border: 1px solid #c5ddf5;
  color: #2971b8;
  padding: 2px 9px;
  border-radius: 12px;
  font-size: 0.85em;
}

/* ── Award list ── */
.award-list { list-style: none; padding: 0; margin: 0; }
.award-item {
  display: flex;
  align-items: baseline;
  gap: 12px;
  padding: 8px 0;
  border-bottom: 1px solid #f0f4f8;
  font-size: 0.9em;
  line-height: 1.5;
}
.award-item:last-child { border-bottom: none; }
.award-year {
  display: inline-block;
  background: #eef4fb;
  color: #2971b8;
  border: 1px solid #c5ddf5;
  padding: 1px 8px;
  border-radius: 10px;
  font-size: 0.82em;
  font-weight: 600;
  white-space: nowrap;
  flex-shrink: 0;
}
.award-level {
  display: inline-block;
  background: #fff3e0;
  color: #e65100;
  border: 1px solid #ffcc80;
  padding: 1px 7px;
  border-radius: 8px;
  font-size: 0.78em;
  margin-left: 6px;
  vertical-align: middle;
}

/* ── Publications ── */
.pub-list { list-style: none; padding: 0; margin: 0; }
.pub-item { padding: 12px 0; border-bottom: 1px solid #f0f4f8; font-size: 0.9em; line-height: 1.6; }
.pub-item:last-child { border-bottom: none; }
.pub-title { font-weight: 600; color: #1a2e44; }
.pub-meta { color: #777; font-size: 0.87em; margin-top: 2px; }
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
.pub-badge-first { background: #fff3e0; color: #e65100; border: 1px solid #ffcc80; }
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

<!-- ===================== TOP BAR ===================== -->
<div class="cv-topbar">
  <button class="cv-print-btn" onclick="window.print()">⬇ <span class="lang-cn">下载 / 打印 PDF</span><span class="lang-en">Download / Print PDF</span></button>
  <div class="lang-toggle">
    <button id="btn-cn" class="active" onclick="setLang('cn')">中文</button>
    <button id="btn-en" onclick="setLang('en')">English</button>
  </div>
</div>

<!-- ===================== HEADER ===================== -->
<div class="cv-header-box lang-cn">
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
<div class="cv-header-box lang-en">
  <div class="cv-name">Anqi Liu &nbsp;<span style="font-size:0.55em;font-weight:400;color:#4a7aac;">刘安琪</span></div>
  <div class="cv-title">PhD Student · 3D Reconstruction &amp; Intelligent Perception</div>
  <div class="cv-meta-grid">
    <div class="cv-meta-item">🎂 &nbsp;2002-01-27</div>
    <div class="cv-meta-item">🌏 &nbsp;Anqing, Anhui, China</div>
    <div class="cv-meta-item">📞 &nbsp;+86-187-2619-7276</div>
    <div class="cv-meta-item">📧 &nbsp;<a href="mailto:anqii0127@gmail.com">anqii0127@gmail.com</a></div>
    <div class="cv-meta-item">🏫 &nbsp;Chonnam National University, Korea</div>
    <div class="cv-meta-item">📍 &nbsp;Gwangju, South Korea</div>
  </div>
</div>

<!-- ===================== RESEARCH INTERESTS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">🔬 研究方向</span>
  <span class="lang-en">🔬 Research Interests</span>
</div>

<div class="research-tags lang-cn">
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
<div class="research-tags lang-en">
  <span class="research-tag">3D Point Cloud Reconstruction</span>
  <span class="research-tag">3D Gaussian Splatting (3DGS)</span>
  <span class="research-tag">Digital Twin</span>
  <span class="research-tag">Point Cloud Semantic Segmentation</span>
  <span class="research-tag">Graph Neural Networks (GNN)</span>
  <span class="research-tag">Spatial Target Localization</span>
  <span class="research-tag">6-DoF Pose Estimation</span>
  <span class="research-tag">Vision-LiDAR Fusion Perception</span>
  <span class="research-tag">Agricultural Robot Perception</span>
</div>

<!-- ===================== EDUCATION ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">🎓 教育经历</span>
  <span class="lang-en">🎓 Education</span>
</div>

<!-- CNU -->
<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">
      <span class="lang-cn">韩国全南国立大学（Chonnam National University）</span>
      <span class="lang-en">Chonnam National University, South Korea</span>
    </div>
    <div class="edu-card-date">
      <span class="lang-cn">2023.09 — 至今</span>
      <span class="lang-en">Sep 2023 — Present</span>
    </div>
  </div>
  <div class="lang-cn">
    <div class="edu-card-degree">融合生物系统机械工程系 &nbsp;｜&nbsp; IT-Bio融合系统（第二专业）&nbsp;｜&nbsp; 硕博连读 · 韩国光州</div>
    <div class="edu-card-body">
      <strong>GPA：</strong>4.33 / 4.5<br>
      <strong>相关课程：</strong>图像处理应用、机器视觉、人工智能、高等应用数学、先进动力学、先进机器人学<br>
      <strong>荣誉奖项：</strong>
      <span class="edu-badge">2024 大学奖学金（6万元）</span>
      <span class="edu-badge">2025 人才培养学金（7万元）</span>
    </div>
  </div>
  <div class="lang-en">
    <div class="edu-card-degree">Dept. of Biosystems Machinery Engineering &nbsp;|&nbsp; IT-Bio Convergence Systems (2nd Major) &nbsp;|&nbsp; Integrated MS-PhD · Gwangju, Korea</div>
    <div class="edu-card-body">
      <strong>GPA:</strong> 4.33 / 4.5<br>
      <strong>Relevant Courses:</strong> Image Processing Applications, Machine Vision, Artificial Intelligence, Advanced Applied Mathematics, Advanced Dynamics, Advanced Robotics<br>
      <strong>Honors &amp; Awards:</strong>
      <span class="edu-badge">2024 University Scholarship (₩60,000)</span>
      <span class="edu-badge">2025 Talent Development Scholarship (₩70,000)</span>
    </div>
  </div>
</div>

<!-- JUFE -->
<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">
      <span class="lang-cn">江西财经大学（Jiangxi University of Finance and Economics）</span>
      <span class="lang-en">Jiangxi University of Finance and Economics</span>
    </div>
    <div class="edu-card-date">2019.09 — 2023.09</div>
  </div>
  <div class="lang-cn">
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
  <div class="lang-en">
    <div class="edu-card-degree">Mathematical Statistics (Elite Talent Program) &nbsp;|&nbsp; School of Statistics and Data Science &nbsp;|&nbsp; B.S. · Nanchang</div>
    <div class="edu-card-body">
      <strong>GPA:</strong> 3.49 / 4.50 (Rank 14/53)<br>
      <strong>Relevant Courses:</strong> C++ Programming, Bayesian Statistics, Probability Theory, Ordinary Differential Equations, Statistical Learning Methods, Machine Learning<br>
      <strong>Honors &amp; Awards:</strong>
      <span class="edu-badge">Outstanding Student</span>
      <span class="edu-badge">Outstanding Cadre</span>
      <span class="edu-badge">University Scholarship</span>
    </div>
  </div>
</div>

<!-- UPF -->
<div class="edu-card">
  <div class="edu-card-header">
    <div class="edu-card-school">
      <span class="lang-cn">西班牙庞培法布拉大学（Universitat Pompeu Fabra）</span>
      <span class="lang-en">Universitat Pompeu Fabra, Spain</span>
    </div>
    <div class="edu-card-date">2022.01 — 2022.07</div>
  </div>
  <div class="lang-cn">
    <div class="edu-card-degree">交换生 · 数据分析方向 · 巴塞罗那</div>
    <div class="edu-card-body">
      <strong>相关课程：</strong>R语言统计分析、统计学习、概率论
    </div>
  </div>
  <div class="lang-en">
    <div class="edu-card-degree">Exchange Student · Data Analytics · Barcelona</div>
    <div class="edu-card-body">
      <strong>Relevant Courses:</strong> R Programming, Statistical Learning, Probability Theory
    </div>
  </div>
</div>

<!-- ===================== RESEARCH PROJECTS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">🧪 硕博科研项目</span>
  <span class="lang-en">🧪 Research Projects</span>
</div>

<!-- Project 1 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">冬季苹果园剪枝点识别</span>
      <span class="lang-en">Pruning Point Recognition in Winter Apple Orchards</span>
    </div>
    <div class="project-card-date">2024.06 — 2025.12</div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 <strong>3D点云重建：</strong>利用多视角RGB-D图像对冬季休眠期苹果树进行密集三维点云采集与重建，构建高精度枝干几何模型</li>
        <li>🔻 <strong>结构骨架提取：</strong>设计基于拓扑感知的骨架提取算法，从稀疏噪声点云中精确还原苹果树主干与侧枝的树形结构</li>
        <li>🔻 <strong>深度学习网络：</strong>构建图神经网络（GNN）剪枝点预测框架，在三维骨架图上完成节点级语义分割与关键剪枝位点定位，并开展点云语义补全研究</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 <strong>3D Point Cloud Reconstruction:</strong> Dense 3D point cloud acquisition and reconstruction of dormant-season apple trees using multi-view RGB-D images, building high-precision branch geometry models</li>
        <li>🔻 <strong>Structural Skeleton Extraction:</strong> Topology-aware skeleton extraction algorithm to accurately recover main trunk and lateral branch structures from sparse noisy point clouds</li>
        <li>🔻 <strong>Deep Learning Network:</strong> GNN-based pruning point prediction framework performing node-level semantic segmentation and key site localization on 3D skeleton graphs, with point cloud semantic completion research</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag">GNN</span>
      <span class="tool-tag"><span class="lang-cn">骨架提取</span><span class="lang-en">Skeleton Extraction</span></span>
      <span class="tool-tag"><span class="lang-cn">语义分割</span><span class="lang-en">Semantic Segmentation</span></span>
      <span class="tool-tag"><span class="lang-cn">点云补全</span><span class="lang-en">Point Cloud Completion</span></span>
      <span class="tool-tag">RGB-D</span>
    </div>
  </div>
</div>

<!-- Project 2 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">基于高斯的离线到在线剪枝目标重定位</span>
      <span class="lang-en">Gaussian-based Offline-to-Online Pruning Target Relocalization</span>
    </div>
    <div class="project-card-date">
      <span class="lang-cn">2025.12 — 至今</span>
      <span class="lang-en">Dec 2025 — Present</span>
    </div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 <strong>高斯重建：</strong>以3D Gaussian Splatting（3DGS）对果园离线场景进行高保真辐射场重建，建立包含结构感知先验的精密三维地图</li>
        <li>🔻 <strong>特征匹配：</strong>设计基于SuperPoint + LightGlue的跨域特征匹配流水线，实现高斯渲染视图与在线相机图像间的精准2D-3D对应关系</li>
        <li>🔻 <strong>6-DoF位姿估计：</strong>融合高斯场景深度渲染与单目深度估计，构建轻量级6自由度相机位姿回归器，支持在线剪枝目标的精确重定位与实时引导</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 <strong>Gaussian Reconstruction:</strong> High-fidelity neural radiance field reconstruction of offline orchard scenes using 3DGS, establishing a structure-aware precise 3D map</li>
        <li>🔻 <strong>Feature Matching:</strong> Cross-domain feature matching pipeline (SuperPoint + LightGlue) for precise 2D-3D correspondences between Gaussian-rendered views and online camera images</li>
        <li>🔻 <strong>6-DoF Pose Estimation:</strong> Lightweight 6-DoF camera pose regressor fusing Gaussian depth rendering and monocular depth estimation for real-time precise pruning target relocalization</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag">3D Gaussian Splatting</span>
      <span class="tool-tag">SuperPoint</span>
      <span class="tool-tag">LightGlue</span>
      <span class="tool-tag">6-DoF <span class="lang-cn">位姿估计</span><span class="lang-en">Pose Estimation</span></span>
    </div>
  </div>
</div>

<!-- Project 3 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">基于拓扑结构的跨季节高斯果园地图持久树木地标定位</span>
      <span class="lang-en">Topology-based Persistent Tree Landmark Localization in Cross-Season Gaussian Orchard Maps</span>
    </div>
    <div class="project-card-date">
      <span class="lang-cn">2026.04 — 至今</span>
      <span class="lang-en">Apr 2026 — Present</span>
    </div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 <strong>跨季节拓扑匹配：</strong>构建季节不变性拓扑图表征，在高斯地图框架内提取持久性树木地标，实现休眠期至生长期的跨季节稳健定位</li>
        <li>🔻 <strong>高斯地图持久化：</strong>研究3DGS地图的增量式更新与持久树木实体管理机制，支持季节变化下地标的语义一致性维护与长周期重定位</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 <strong>Cross-season Topological Matching:</strong> Season-invariant topological graph representation to extract persistent tree landmarks within the Gaussian map for robust dormant-to-growing-season localization</li>
        <li>🔻 <strong>Gaussian Map Persistence:</strong> Incremental 3DGS map update and persistent tree entity management mechanism supporting semantic-consistent landmark maintenance and long-cycle relocalization under seasonal change</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag"><span class="lang-cn">拓扑图匹配</span><span class="lang-en">Topological Graph Matching</span></span>
      <span class="tool-tag"><span class="lang-cn">3DGS地图</span><span class="lang-en">3DGS Map</span></span>
      <span class="tool-tag"><span class="lang-cn">跨季节定位</span><span class="lang-en">Cross-Season Localization</span></span>
      <span class="tool-tag"><span class="lang-cn">地标持久化</span><span class="lang-en">Landmark Persistence</span></span>
    </div>
  </div>
</div>

<!-- ===================== UNDERGRADUATE PROJECTS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">📊 本科项目经历</span>
  <span class="lang-en">📊 Undergraduate Projects</span>
</div>

<!-- UG Project 1 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">按地区分析疫苗接种数据</span>
      <span class="lang-en">Regional COVID-19 Vaccination Data Analysis</span>
    </div>
    <div class="project-card-date">2021.06 — 2021.09</div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 按不同年龄组统计分析第三剂疫苗接种完成情况，识别接种率偏低的区域与人群</li>
        <li>🔻 将分析结果可视化并交付地方政府，帮助其更精准地制定疫苗接种督促策略</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 Analyzed third-dose COVID-19 vaccination completion rates by age group and region, identifying under-vaccinated populations</li>
        <li>🔻 Delivered data visualizations to local government to support more targeted vaccination promotion campaigns</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag">R</span>
      <span class="tool-tag"><span class="lang-cn">统计分析</span><span class="lang-en">Statistical Analysis</span></span>
      <span class="tool-tag"><span class="lang-cn">数据可视化</span><span class="lang-en">Data Visualization</span></span>
    </div>
  </div>
</div>

<!-- UG Project 2 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">交通客流量分析</span>
      <span class="lang-en">Public Transportation Passenger Flow Analysis</span>
    </div>
    <div class="project-card-date">2021.09 — 2021.12</div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 分析同一地区疫情前后公共交通客流量的时序变化与结构差异</li>
        <li>🔻 基于统计建模结果为交通管理部门提供班次频率调整决策依据</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 Analyzed temporal and structural changes in public transportation ridership before and after the COVID-19 outbreak in a target region</li>
        <li>🔻 Provided evidence-based recommendations to transit authorities on adjusting service frequency based on statistical modeling results</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag">R</span>
      <span class="tool-tag"><span class="lang-cn">时间序列分析</span><span class="lang-en">Time Series Analysis</span></span>
      <span class="tool-tag">SAS</span>
    </div>
  </div>
</div>

<!-- UG Project 3 -->
<div class="project-card">
  <div class="project-card-header">
    <div class="project-card-title">
      <span class="lang-cn">财务信息真实性分析</span>
      <span class="lang-en">Financial Data Authenticity Analysis</span>
    </div>
    <div class="project-card-date">2022.01 — 2022.04</div>
  </div>
  <div class="project-content">
    <div class="lang-cn">
      <ul>
        <li>🔻 运用统计检验方法（本福特定律、异常值检测等）对某金融公司财务数据进行真实性核查</li>
        <li>🔻 识别数据异常模式，出具分析报告，辅助管理层完善财务风险管控机制</li>
      </ul>
    </div>
    <div class="lang-en">
      <ul>
        <li>🔻 Applied statistical methods (Benford's Law, outlier detection) to audit the authenticity of financial data from a financial institution</li>
        <li>🔻 Identified anomalous patterns and produced an analytical report to assist management in strengthening financial risk controls</li>
      </ul>
    </div>
    <div class="project-tools">
      <span class="tools-label">🔧</span>
      <span class="tool-tag">R</span>
      <span class="tool-tag"><span class="lang-cn">本福特定律</span><span class="lang-en">Benford's Law</span></span>
      <span class="tool-tag"><span class="lang-cn">异常检测</span><span class="lang-en">Anomaly Detection</span></span>
    </div>
  </div>
</div>

<!-- ===================== COMPETITIONS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">🏆 比赛经历</span>
  <span class="lang-en">🏆 Competitions &amp; Awards</span>
</div>

<ul class="award-list">
  <li class="award-item">
    <span class="award-year">2022</span>
    <span>
      <span class="lang-cn">"创青春"全国大学生创业大赛<span class="award-level">省铜奖</span></span>
      <span class="lang-en">"Chuang Qing Chun" National College Student Entrepreneurship Competition<span class="award-level">Provincial Bronze</span></span>
    </span>
  </li>
  <li class="award-item">
    <span class="award-year">2021</span>
    <span>
      <span class="lang-cn">全国SAS软件应用大赛<span class="award-level">国家三等奖</span></span>
      <span class="lang-en">National SAS Software Application Competition<span class="award-level">National 3rd Prize</span></span>
    </span>
  </li>
  <li class="award-item">
    <span class="award-year">2021</span>
    <span>
      <span class="lang-cn">华创杯市场分析大赛<span class="award-level">省二等奖</span></span>
      <span class="lang-en">Huachuang Cup Market Analysis Competition<span class="award-level">Provincial 2nd Prize</span></span>
    </span>
  </li>
  <li class="award-item">
    <span class="award-year">2019</span>
    <span>
      <span class="lang-cn">江西财经大学创新创业大赛<span class="award-level">优胜奖</span></span>
      <span class="lang-en">JUFE Innovation &amp; Entrepreneurship Competition<span class="award-level">Excellence Award</span></span>
    </span>
  </li>
</ul>

<!-- ===================== PUBLICATIONS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">📄 科研成果</span>
  <span class="lang-en">📄 Publications</span>
</div>

<p><strong><span class="lang-cn">期刊论文</span><span class="lang-en">Journal Articles</span></strong></p>

<ul class="pub-list">
  <li class="pub-item">
    <div class="pub-title">
      Realtime multi-RGBD SLAM framework for 3D reconstruction and phenotyping in large-scale apple orchards
      <span class="pub-badge"><span class="lang-cn">第二作者</span><span class="lang-en">2nd Author</span></span>
    </div>
    <div class="pub-meta lang-cn">期刊论文 · 大规模果园实时多RGB-D SLAM三维重建与表型分析框架</div>
    <div class="pub-meta lang-en">Journal Article · Real-time multi-RGBD SLAM for 3D reconstruction and phenotyping in large-scale apple orchards</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      Transformer-based cross-view LiDAR–Orthomosaic fusion for geo-localization and digital modeling in apple orchards
      <span class="pub-badge"><span class="lang-cn">第三作者</span><span class="lang-en">3rd Author</span></span>
    </div>
    <div class="pub-meta lang-cn">期刊论文 · 基于Transformer的LiDAR与正射影像跨视角融合用于苹果园地理定位与数字建模</div>
    <div class="pub-meta lang-en">Journal Article · Transformer-based cross-view LiDAR–Orthomosaic fusion for geo-localization and digital modeling in apple orchards</div>
  </li>
</ul>

<p><strong><span class="lang-cn">会议论文</span><span class="lang-en">Conference Papers</span></strong></p>

<ul class="pub-list">
  <li class="pub-item">
    <div class="pub-title">
      GNN-Driven Detection of Pruning Points in Apple Trees Using 3D Point Clouds
      <span class="pub-badge pub-badge-first"><span class="lang-cn">第一作者</span><span class="lang-en">1st Author</span></span>
      <span class="conf-badge">KSAM 2025 Spring</span>
    </div>
    <div class="pub-meta lang-cn">韩国农业机械学会春季学术大会 2025</div>
    <div class="pub-meta lang-en">Korean Society for Agricultural Machinery, Spring 2025</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      2D-3D Matching for High-Precision Camera Localization in Apple Orchards Using SuperPoint and LightGlue
      <span class="pub-badge pub-badge-first"><span class="lang-cn">第一作者</span><span class="lang-en">1st Author</span></span>
      <span class="conf-badge">KSAM 2025 Fall</span>
    </div>
    <div class="pub-meta lang-cn">韩国农业机械学会秋季学术大会 2025</div>
    <div class="pub-meta lang-en">Korean Society for Agricultural Machinery, Fall 2025</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      TopoSkel-GNN: A Topology-Aware Skeleton Graph Network for Efficient 3D Semantic Analysis
      <span class="pub-badge pub-badge-first"><span class="lang-cn">第一作者</span><span class="lang-en">1st Author</span></span>
      <span class="conf-badge">KAIA 2025 Fall</span>
    </div>
    <div class="pub-meta lang-cn">韩国人工智能学会秋季学术大会 2025</div>
    <div class="pub-meta lang-en">Korean Artificial Intelligence Association, Fall 2025</div>
  </li>
  <li class="pub-item">
    <div class="pub-title">
      StructGS: Structure-Aware 3D Gaussian Splatting for Complex Orchard Environments
      <span class="pub-badge pub-badge-first"><span class="lang-cn">第一作者</span><span class="lang-en">1st Author</span></span>
      <span class="conf-badge">KSAM 2026 Spring</span>
    </div>
    <div class="pub-meta lang-cn">韩国农业机械学会春季学术大会 2026</div>
    <div class="pub-meta lang-en">Korean Society for Agricultural Machinery, Spring 2026</div>
  </li>
</ul>

<!-- ===================== SKILLS ===================== -->
<div class="cv-section-title">
  <span class="lang-cn">🛠 技能</span>
  <span class="lang-en">🛠 Skills</span>
</div>

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

<p style="font-size:0.88em;color:#777;margin-top:1em;">
  <span class="lang-cn">语言：普通话（母语）· 英语（学术写作与交流）· 韩语（日常交流）· 西班牙语（日常交流）</span>
  <span class="lang-en">Languages: Mandarin (Native) · English (Academic) · Korean (Daily) · Spanish (Daily)</span>
</p>

<script>
function setLang(lang) {
  document.body.classList.toggle('cv-lang-en', lang === 'en');
  document.getElementById('btn-cn').classList.toggle('active', lang === 'cn');
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  try { localStorage.setItem('cv-lang', lang); } catch(e) {}
}
(function() {
  try {
    if (localStorage.getItem('cv-lang') === 'en') {
      document.body.classList.add('cv-lang-en');
      document.getElementById('btn-cn').classList.remove('active');
      document.getElementById('btn-en').classList.add('active');
    }
  } catch(e) {}
})();
</script>
