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
<div class="section" id="team-members-section" >
  <h2>👥 Team Members</h2>
  <img src="{{ '/images/team_member.png' | relative_url }}" alt="Team Member" style="max-width: 800px; display: block; margin-top: 1em;">
</div>

<!-- Section: Publications -->
<div class="section" id="publications-section" >
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
<div class="section" id="awards-section">
  <h2>🎖 Honors and Awards</h2>
  <ul>
    <li>🏆 <strong>Best Science Paper Award</strong> at <strong>BMVC 2015</strong></li>
    <li>🤝 Collaborations with <strong>law enforcement agencies</strong></li>
    <li>🛍️ Partnerships with <strong>online retail platforms</strong></li>
    <li>27 x CVPR, 11 x ICCV, 11 x ECCV, 2 x SIGGRAPH Asia, 1 x ICLR, 1 x ICML, 1 x NeurIPS (as of July 2022)</li>
  </ul>
</div>

<!-- Section: Projects -->
<div class="section" id="projects-section" >
  <h2>Projects</h2>
  projects list
</div>

<!-- Section: News -->
<div class="section" id="news-section" >
  <h2>🔥 Team News</h2>
  <a class="twitter-timeline" data-height="600" href="https://twitter.com/SketchXlab?ref_src=twsrc%5Etfw">Tweets by SketchXlab</a>
  <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>

<!-- 页面切换脚本 -->
<script>
  function showSection(id) {
    const sections = document.querySelectorAll(".section");
    sections.forEach(section => {
      if (section.id === id) {
        // 激活新 section
        section.classList.add("active");
      } else if (section.classList.contains("active")) {
        // 淡出旧 section 后再移除 active
        section.classList.remove("active");
      }
    });

    // 更新地址栏的 hash
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



