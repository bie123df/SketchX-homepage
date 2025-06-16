---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- Section: About -->
<div class="section" id="about-section">
  <h2>Welcome to SketchX</h2>
  <p>
    The ultimate vision for <strong>SketchX</strong> is to understand how seeing can be explained by drawing. In other words, how a better understanding of human sketch data can be translated into insights on how human visual systems operate — and in turn, how such insights can benefit computer vision and cognitive science at large.
  </p>
  <p>
    SketchX has been actively investigating all aspects of sketch research since 2012. The problems we study range from conventional tasks such as sketch recognition and sketch synthesis, to those we have pioneered, such as fine-grained sketch-based image retrieval and memory-aware forensic sketch analysis.
  </p>
</div>

<!-- Section: Team Members -->
<div class="section" id="team-members-section" style="display: none;">
  <h2>👥 Team Members</h2>
  <img src="{{ '/images/team_member.png' | relative_url }}" alt="Team Member" style="max-width: 800px; display: block; margin-top: 1em;">
</div>

<!-- Section: Publications -->
<div class="section" id="publications-section" style="display: none;">
  <h2>📝 Team Publications</h2>
  <ol>
    <li><a href="http://openaccess.thecvf.com/content_iccv_2017/html/Li_Deeper_Broader_and_ICCV_2017_paper.html">Deeper, Broader and Artier Domain Generalization</a><br><em>Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M. Hospedales</em></li>
    <li><a href="https://ojs.aaai.org/index.php/AAAI/article/view/11596">Learning to generalize: Meta-learning for domain generalization</a><br><em>Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M Hospedales</em></li>
    <!-- ... 其余条目略 ... -->
    <li><a href="http://openaccess.thecvf.com/content/CVPR2022/html/He_Style-Based_Global_Appearance_Flow_for_Virtual_Try-On_CVPR_2022_paper.html">Style-based global appearance flow for virtual try-on</a><br><em>Sen He, Yi-Zhe Song, Tao Xiang</em></li>
    <li><a href="https://proceedings.neurips.cc/paper/2021/hash/cbcb58ac2e496207586df2854b17995f-Abstract.html">One loss for all: Deep hashing with a single cosine similarity based learning objective</a><br><em>Jiun Tian Hoe, Kam Woh Ng, Tianyu Zhang, Chee Seng Chan, Yi-Zhe Song, Tao Xiang</em></li>
  </ol>
</div>

<!-- Section: Awards -->
<div class="section" id="awards-section" style="display: none;">
  <h2>🎖 Honors and Awards</h2>
  <ul>
    <li>🏆 <strong>Best Science Paper Award</strong> at <strong>BMVC 2015</strong></li>
    <li>🤝 Collaborations with <strong>law enforcement agencies</strong></li>
    <li>🛍️ Partnerships with <strong>online retail platforms</strong></li>
    <li>27 x CVPR, 11 x ICCV, 11 x ECCV, 2 x SIGGRAPH Asia, 1 x ICLR, 1 x ICML, 1 x NeurIPS (as of July 2022)</li>
  </ul>
</div>

<!-- Section: News -->
<div class="section" id="news-section" style="display: none;">
  <h2>🔥 Team News</h2>
  <a class="twitter-timeline" data-height="600" href="https://twitter.com/SketchXlab?ref_src=twsrc%5Etfw">Tweets by SketchXlab</a>
  <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>

<!-- 页面控制脚本：控制 section 显隐 -->
<script>
  document.addEventListener("DOMContentLoaded", function () {
    const sections = document.querySelectorAll(".section");
    const links = document.querySelectorAll(".masthead__menu-item a");

    function showSection(id) {
      sections.forEach(section => {
        section.style.display = section.id === id + "-section" ? "block" : "none";
      });
    }

    links.forEach(link => {
      const sectionId = link.getAttribute("data-section");
      link.addEventListener("click", function (e) {
        e.preventDefault();  // 阻止默认跳转
        showSection(sectionId);
        history.replaceState(null, "", "#" + sectionId);  // 用 hash 更新 URL
      });
    });

    // 初始：根据 hash 显示
    const initial = window.location.hash ? window.location.hash.substring(1) : "about";
    showSection(initial);
  });
</script>

<script>
  function showSection(id) {
    const sections = document.querySelectorAll(".section");
    sections.forEach(section => {
      section.style.display = (section.id === id) ? "block" : "none";
    });
    // 更新地址栏的 hash（比如 #publications）
    if (id.endsWith("-section")) {
      const hash = id.replace("-section", "");
      history.replaceState(null, "", "#" + hash);
    }
  }

  document.addEventListener("DOMContentLoaded", function () {
    const hash = window.location.hash.replace("#", "") || "about";
    const sectionId = hash + "-section";
    showSection(sectionId);
  });
</script>

