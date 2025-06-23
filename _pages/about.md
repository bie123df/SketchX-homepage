---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<!-- 字体引入 -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display&family=Open+Sans&display=swap" rel="stylesheet">

<style>
  body {
    font-family: 'Open Sans', serif;
    background-color: #fdf8f0;
    color: #3c3c3c;
    line-height: 1.8;
    margin: 0;
    padding: 0;
  }

  .section {
    max-width: 900px;
    margin: 0 auto;
    padding: 3em 2em;
  }

.section h2 {
  font-family: 'Playfair Display', serif;
  font-size: 2.2em;
  color: #4d3f2b;
  margin-bottom: 0.6em; /* 原为 1em，减小下边距 */
  margin-top: 0; /* 可选：若父容器上方有内边距，这里设为0更紧凑 */
  position: relative;
}

.section h2::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -4px; /* 原为 -8px，调小下划线与标题文字的距离 */
  width: 50px;   /* 原为 60px，使下划线稍微更短 */
  height: 2px;   /* 原为 3px，更细一点 */
  background-color: #b89b72;
}

  .section p {
    font-size: 1.05em;
    text-align: justify;
    margin-bottom: 1.2em;
  }

  /* 首字母放大 */
  .dropcap::first-letter {
    float: left;
    font-size: 3em;
    font-family: 'Playfair Display', serif;
    margin-right: 10px;
    line-height: 1;
    color: #947c5e;
  }

  /* 引文风格人物介绍 */
  .bio-quote {
    background: #fffefb;
    border-left: 6px solid #ccb89c;
    padding: 1.5em 2em;
    margin-top: 2em;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(200, 180, 140, 0.1);
  }

  .bio-quote h3 {
    font-family: 'Playfair Display', serif;
    color: #5c4a3b;
    font-size: 1.4em;
    margin-top: 0;
  }

  .bio-quote blockquote {
    margin: 1em 0;
    padding-left: 1em;
    border-left: 3px solid #d4c4a8;
    color: #555;
    font-style: italic;
  }

  .bio-quote img {
    float: right;
    width: 140px;
    margin-left: 20px;
    border-radius: 8px;
    border: 2px solid #e1d8c3;
  }

  /* 团队成员区块 */
  #team-members-section .team-box {
    background: #ffffff;
    padding: 24px;
    border-radius: 12px;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.03);
    text-align: center;
    margin-top: 2em;
  }

  #team-members-section img {
    max-width: 85%;
    border-radius: 12px;
    border: 1px solid #d8cfc0;
    margin-top: 1em;
  }

  #team-members-section p {
    font-style: italic;
    color: #777;
    margin-top: 1em;
  }
</style>

<!-- Section: About -->
<div class="section" id="about-section">
  <h2>🌟 Welcome to SketchX</h2>

  <p class="dropcap">
    The ultimate vision for <strong>SketchX</strong> is to understand how seeing can be explained by drawing. In other words, how a better understanding of human sketch data can be translated into insights on how human visual systems operate — and in turn, how such insights can benefit computer vision and cognitive science at large.
  </p>
  <p>
    SketchX has been actively investigating all aspects of sketch research since 2012. The problems we study range from conventional tasks such as sketch recognition and sketch synthesis, to those we have pioneered, such as fine-grained sketch-based image retrieval and memory-aware forensic sketch analysis.
  </p>

  <!-- 人物介绍块：引文风格 -->
  <div class="bio-quote">
    <img src="{{ '/images/song.jpg' | relative_url }}" alt="Professor Yi-Zhe Song">
    <h3>👨‍🏫 Professor Yi-Zhe Song</h3>
    <blockquote>
      "Understanding vision through the act of drawing is not just a computational challenge, but a cognitive journey."
    </blockquote>
    <p>
      Yi-Zhe Song is a Professor of Computer Vision and Machine Learning at CVSSP, one of the UK's largest AI research centers.
      He leads the SketchX Lab — a group of 3 academics, 2 postdocs, and 14 PhD students.
    </p>
    <p>
      He is an Associate Editor for TPAMI, Programme Chair for BMVC 2021, and has served as Area Chair for ECCV, CVPR, ICCV.
      His work has won the Best Paper Award at BMVC 2015 and appeared in CVPR, ECCV, ICCV, SIGGRAPH Asia, and ICML.
    </p>
    <p>
      Yi-Zhe received his PhD from the University of Bath, MSc from Cambridge (Best Dissertation Award), and BSc from Bath with First Class Honours.
    </p>
  </div>
</div>

<!-- Section: Team Members -->
<div class="section" id="team-members-section">
  <h2>👥 Team Members</h2>

  <div class="team-box">
    <img src="{{ '/images/team_member.png' | relative_url }}" alt="Team Member">
  </div>
</div>



<!-- Section: Publications -->
<div class="section" id="publications-section" >
  <h2>📝 Team Publications</h2>
  <!-- 2025 年论文列表 -->
<h3>📚 2025</h3>
<ol style="padding-left: 1.2em;">
  <li style="margin-bottom: 1em; line-height: 1.6;">
    <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32894" target="_blank" rel="noopener noreferrer">
      <strong>VA-AR: Learning Velocity-Aware Action Representations with Mixture of Window Attention</strong>
    </a>
    Jiangning Wei, Lixiong Qin, Bo Yu, Tianjian Zou, Chuhan Yan, Dandan Xiao, Yang Yu, Lan Yang, Ke Li, Jun Liu — <em>AAAI 2025</em>
  </li>
  
  <li style="margin-bottom: 1em; line-height: 1.6;">
    <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32240" target="_blank" rel="noopener noreferrer">
      <strong>VersaGen: Unleashing Versatile Visual Control for Text-to-Image Synthesis</strong>
    </a>
    &nbsp;Zhipeng Chen, Lan Yang, Yonggang Qi, Honggang Zhang, Kaiyue Pang, Ke Li, Yi-Zhe Song &nbsp;<em>AAAI</em>
  </li>
</ol>

  <ol>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2025</span><br>
      <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32894" target="_blank" rel="noopener noreferrer">VA-AR: Learning Velocity-Aware Action Representations with Mixture of Window Attention</a><br>
      <small>Jiangning Wei, Lixiong Qin, Bo Yu, Tianjian Zou, Chuhan Yan, Dandan Xiao, Yang Yu, Lan Yang, Ke Li, Jun Liu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2025</span><br>
      <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32240" target="_blank" rel="noopener noreferrer">VersaGen: Unleashing Versatile Visual Control for Text-to-Image Synthesis</a><br>
      <small>Zhipeng Chen, Lan Yang, Yonggang Qi, Honggang Zhang, Kaiyue Pang, Ke Li, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Du_DemoFusion_Democratising_High-Resolution_Image_Generation_With_No__CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Demofusion: Democratising high-resolution image generation with no $$$</a><br>
      <small>Ruoyi Du, Dongliang Chang, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Its_All_About_Your_Sketch_Democratising_Sketch_Control_in_Diffusion_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">It's All About Your Sketch: Democratising Sketch Control in Diffusion Models</a><br>
      <small>Subhadeep Koley, Ayan Kumar Bhunia, Deeptanshu Sekhri, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_How_to_Handle_Sketch-Abstraction_in_Sketch-Based_Image_Retrieval_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">How to handle sketch-abstraction in sketch-based image retrieval?</a><br>
      <small>Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Youll_Never_Walk_Alone_A_Sketch_and_Text_Duet_for_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">You'll Never Walk Alone: A Sketch and Text Duet for Fine-Grained Image Retrieval</a><br>
      <small>Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_Doodle_Your_3D_From_Abstract_Freehand_Sketches_to_Precise_3D_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Doodle your 3d: From abstract freehand sketches to precise 3d shapes</a><br>
      <small>Hmrishav Bandyopadhyay, Subhadeep Koley, Ayan Das, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_SketchINR_A_First_Look_into_Sketches_as_Implicit_Neural_Representations_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Sketchinr: A first look into sketches as implicit neural representations</a><br>
      <small>Hmrishav Bandyopadhyay, Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Tao Xiang, Timothy Hospedales, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Text-to-Image_Diffusion_Models_are_Great_Sketch-Photo_Matchmakers_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Text-to-image diffusion models are great sketch-photo matchmakers</a><br>
      <small>Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2024</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10472065/" target="_blank" rel="noopener noreferrer">Bi-directional ensemble feature reconstruction network for few-shot fine-grained classification</a><br>
      <small>Jijie Wu, Dongliang Chang, Aneeshan Sain, Xiaoxu Li, Zhanyu Ma, Jie Cao, Jun Guo, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Qu_Wired_Perspectives_Multi-View_Wire_Art_Embraces_Generative_AI_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Wired perspectives: Multi-view wire art embraces generative ai</a><br>
      <small>Zhiyu Qu, Lan Yang, Honggang Zhang, Tao Xiang, Kaiyue Pang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Chen_DemoCaricature_Democratising_Caricature_Generation_with_a_Rough_Sketch_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">Democaricature: Democratising caricature generation with a rough sketch</a><br>
      <small>Dar-Yen Chen, Ayan Kumar Bhunia, Subhadeep Koley, Aneeshan Sain, Pinaki Nath Chowdhury, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2024</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-72673-6_23" target="_blank" rel="noopener noreferrer">PartCraft: Crafting Creative Objects by Parts</a><br>
      <small>Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2024</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10471272/" target="_blank" rel="noopener noreferrer">Creativeseg: Semantic segmentation of creative sketches</a><br>
      <small>Yixiao Zheng, Kaiyue Pang, Ayan Das, Dongliang Chang, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2024</span><br>
      <a href="https://arxiv.org/abs/2405.18716" target="_blank" rel="noopener noreferrer">Sketchdeco: Decorating b&amp;w sketches with colour</a><br>
      <small>Chaitat Utintu, Pinaki Nath Chowdhury, Aneeshan Sain, Subhadeep Koley, Ayan Kumar Bhunia, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_What_Sketch_Explainability_Really_Means_for_Downstream_Tasks_CVPR_2024_paper.html" target="_blank" rel="noopener noreferrer">What Sketch Explainability Really Means for Downstream Tasks?</a><br>
      <small>Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICLR 2024</span><br>
      <a href="https://openreview.net/forum?id=O2jyuo89CK" target="_blank" rel="noopener noreferrer">Modelling complex vector drawings with stroke-clouds</a><br>
      <small>Alexander Ashcroft, Ayan Das, Yulia Gryaditskaya, Zhiyu Qu, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2024</span><br>
      <a href="https://openaccess.thecvf.com/content/CVPR2024W/FGVC11/html/Ng_ConceptHash_Interpretable_Fine-Grained_Hashing_via_Concept_Discovery_CVPRW_2024_paper.html" target="_blank" rel="noopener noreferrer">ConceptHash: Interpretable Fine-Grained Hashing via Concept Discovery</a><br>
      <small>Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICLR 2024</span><br>
      <a href="https://openreview.net/forum?id=nQsimt9atc" target="_blank" rel="noopener noreferrer">Ipr-nerf: Ownership verification meets neural radiance field</a><br>
      <small>Win Kent Ong, Kam Woh Ng, Chee Seng Chan, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2024</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-72992-8_13" target="_blank" rel="noopener noreferrer">Do Generalised Classifiers Really Work on Human Drawn Sketches?</a><br>
      <small>Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Ayan Kumar Bhunia, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICLR 2024</span><br>
      <a href="https://openreview.net/forum?id=5xadJmgwix" target="_blank" rel="noopener noreferrer">Scale-Adaptive Diffusion Model for Complex Sketch Synthesis</a><br>
      <small>Jijin Hu, Ke Li, Yonggang Qi, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICLR 2024</span><br>
      <a href="https://openreview.net/forum?id=5xadJmgwix" target="_blank" rel="noopener noreferrer">Scale-Adaptive Diffusion Model for Complex Sketch Synthesis</a><br>
      <small>Jijin Hu, Ke Li, Yonggang Qi, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2024</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-72998-0_9" target="_blank" rel="noopener noreferrer">Freeview Sketching: View-Aware Fine-Grained Sketch-Based Image Retrieval</a><br>
      <small>Aneeshan Sain, Pinaki Nath Chowdhury, Subhadeep Koley, Ayan Kumar Bhunia, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2024</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10707331/" target="_blank" rel="noopener noreferrer">Understanding Episode Hardness in Few-Shot Learning</a><br>
      <small>Yurong Guo, Ruoyi Du, Aneeshan Sain, Kongming Liang, Yuan Dong, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IJCV 2024</span><br>
      <a href="https://link.springer.com/article/10.1007/s11263-024-02001-1" target="_blank" rel="noopener noreferrer">Annotation-Free Human Sketch Quality Assessment</a><br>
      <small>Lan Yang, Kaiyue Pang, Honggang Zhang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2024</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10589301/" target="_blank" rel="noopener noreferrer">3D Reconstruction From a Single Sketch via View-Dependent Depth Sampling</a><br>
      <small>Chenjian Gao, Xilin Wang, Qian Yu, Lu Sheng, Jing Zhang, Xiaoguang Han, Yi-Zhe Song, Dong Xu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICANN 2024</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-72353-7_14" target="_blank" rel="noopener noreferrer">Advancing Free-Breathing Cardiac Cine MRI: Retrospective Respiratory Motion Correction Via Kspace-and-Image Guided Diffusion Model</a><br>
      <small>Hongming Guo, Ziqing Huang, Qian Yuan, Hanbo Song, Zhiyan Liu, Xianzhao Feng, Anqi Liu, Min Liu, Ke Li, Ruixi Zhou</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICANN 2024</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-78347-0_3" target="_blank" rel="noopener noreferrer">Sketch2Seg: Sketch-Based Image Segmentation with Pre-trained Diffusion Model</a><br>
      <small>Xin Dai, Haoge Deng, Ke Li, Yonggang Qi</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Sain_CLIP_for_All_Things_Zero-Shot_Sketch-Based_Image_Retrieval_Fine-Grained_or_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Clip for all things zero-shot sketch-based image retrieval, fine-grained or not</a><br>
      <small>Aneeshan Sain, Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Subhadeep Koley, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2023</span><br>
      <a href="https://ojs.aaai.org/index.php/AAAI/article/view/25383" target="_blank" rel="noopener noreferrer">Bi-directional feature reconstruction network for fine-grained few-shot image classification</a><br>
      <small>Jijie Wu, Dongliang Chang, Aneeshan Sain, Xiaoxu Li, Zhanyu Ma, Jie Cao, Jun Guo, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #ff9800; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">NeurIPS 2023</span><br>
      <a href="https://proceedings.neurips.cc/paper_files/paper/2023/hash/0fb98d483fa580e0354bcdd3a003a3f3-Abstract-Conference.html" target="_blank" rel="noopener noreferrer">Headsculpt: Crafting 3d head avatars with text</a><br>
      <small>Xiao Han, Yukang Cao, Kai Han, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang, Kwan-Yee K Wong</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Koley_Picture_That_Sketch_Photorealistic_Image_Generation_From_Abstract_Sketches_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Picture that sketch: Photorealistic image generation from abstract sketches</a><br>
      <small>Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Lin_Zero-Shot_Everything_Sketch-Based_Image_Retrieval_and_in_Explainable_Style_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Zero-shot everything sketch-based image retrieval, and in explainable style</a><br>
      <small>Fengyin Lin, Mingkang Li, Da Li, Timothy Hospedales, Yi-Zhe Song, Yonggang Qi</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Nag_DiffTAD_Temporal_Action_Detection_with_Proposal_Denoising_Diffusion_ICCV_2023_paper.html" target="_blank" rel="noopener noreferrer">Difftad: Temporal action detection with proposal denoising diffusion</a><br>
      <small>Sauradip Nag, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Han_FAME-ViL_Multi-Tasking_Vision-Language_Model_for_Heterogeneous_Fashion_Tasks_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Fame-vil: Multi-tasking vision-language model for heterogeneous fashion tasks</a><br>
      <small>Xiao Han, Xiatian Zhu, Licheng Yu, Li Zhang, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chowdhury_SceneTrilogy_On_Human_Scene-Sketch_and_Its_Complementarity_With_Photo_and_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Scenetrilogy: On human scene-sketch and its complementarity with photo and text</a><br>
      <small>Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICLR 2023</span><br>
      <a href="https://openreview.net/forum?id=4eJ43EN2g6l" target="_blank" rel="noopener noreferrer">SketchKnitter: Vectorized Sketch Generation with Diffusion Models</a><br>
      <small>Qiang Wang, Haoge Deng, Yonggang Qi, Da Li, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Han_Controllable_Person_Image_Synthesis_with_Pose-Constrained_Latent_Diffusion_ICCV_2023_paper.html" target="_blank" rel="noopener noreferrer">Controllable person image synthesis with pose-constrained latent diffusion</a><br>
      <small>Xiao Han, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10145054/" target="_blank" rel="noopener noreferrer">Prediction calibration for generalized few-shot semantic segmentation</a><br>
      <small>Zhihe Lu, Sen He, Da Li, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Sain_Exploiting_Unlabelled_Photos_for_Stronger_Fine-Grained_SBIR_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Exploiting unlabelled photos for stronger fine-grained SBIR</a><br>
      <small>Aneeshan Sain, Ayan Kumar Bhunia, Subhadeep Koley, Pinaki Nath Chowdhury, Soumitri Chattopadhyay, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Bhunia_Sketch2Saliency_Learning_To_Detect_Salient_Objects_From_Human_Drawings_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Sketch2saliency: Learning to detect salient objects from human drawings</a><br>
      <small>Ayan Kumar Bhunia, Subhadeep Koley, Amandeep Kumar, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chaudhuri_Data-Free_Sketch-Based_Image_Retrieval_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Data-free sketch-based image retrieval</a><br>
      <small>Abhra Chaudhuri, Ayan Kumar Bhunia, Yi-Zhe Song, Anjan Dutta</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10189399/" target="_blank" rel="noopener noreferrer">Uncertainty-aware source-free domain adaptive semantic segmentation</a><br>
      <small>Zhihe Lu, Da Li, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chang_An_Erudite_Fine-Grained_Visual_Classification_Model_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">An erudite fine-grained visual classification model</a><br>
      <small>Dongliang Chang, Yujun Tong, Ruoyi Du, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Guo_Task-aware_Adaptive_Learning_for_Cross-domain_Few-shot_Learning_ICCV_2023_paper.html" target="_blank" rel="noopener noreferrer">Task-aware adaptive learning for cross-domain few-shot learning</a><br>
      <small>Yurong Guo, Ruoyi Du, Yuan Dong, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Du_On-the-Fly_Category_Discovery_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">On-the-fly category discovery</a><br>
      <small>Ruoyi Du, Dongliang Chang, Kongming Liang, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://arxiv.org/abs/2304.03785" target="_blank" rel="noopener noreferrer">ChiroDiff: Modelling chirographic data with Diffusion Models</a><br>
      <small>Ayan Das, Yongxin Yang, Timothy Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Luo_3D_VR_Sketch_Guided_3D_Shape_Prototyping_and_Exploration_ICCV_2023_paper.html" target="_blank" rel="noopener noreferrer">3d vr sketch guided 3d shape prototyping and exploration</a><br>
      <small>Ling Luo, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, Yulia Gryaditskaya</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10214525/" target="_blank" rel="noopener noreferrer">Sketch-segformer: Transformer-based segmentation for figurative and creative sketches</a><br>
      <small>Yixiao Zheng, Jiyang Xie, Aneeshan Sain, Yi-Zhe Song, Zhanyu Ma</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Nag_Post-Processing_Temporal_Action_Detection_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Post-processing temporal action detection</a><br>
      <small>Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10122150/" target="_blank" rel="noopener noreferrer">Making a bird ai expert work for you and me</a><br>
      <small>Dongliang Chang, Kaiyue Pang, Ruoyi Du, Yujun Tong, Yi-Zhe Song, Zhanyu Ma, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Qu_SketchXAI_A_First_Look_at_Explainability_for_Human_Sketches_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Sketchxai: A first look at explainability for human sketches</a><br>
      <small>Zhiyu Qu, Yulia Gryaditskaya, Ke Li, Kaiyue Pang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://arxiv.org/abs/2308.14191" target="_blank" rel="noopener noreferrer">Sketchdreamer: Interactive text-augmented creative sketch ideation</a><br>
      <small>Zhiyu Qu, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Qu_SketchXAI_A_First_Look_at_Explainability_for_Human_Sketches_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Sketchxai: A first look at explainability for human sketches</a><br>
      <small>Zhiyu Qu, Yulia Gryaditskaya, Ke Li, Kaiyue Pang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10292696/" target="_blank" rel="noopener noreferrer">Mind the Gap: Open Set Domain Adaptation via Mutual-to-Separate Framework</a><br>
      <small>Dongliang Chang, Aneeshan Sain, Zhanyu Ma, Yi-Zhe Song, Ruiping Wang, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Chowdhury_Democratising_2D_Sketch_to_3D_Shape_Retrieval_Through_Pivoting_ICCV_2023_paper.html" target="_blank" rel="noopener noreferrer">Democratising 2D sketch to 3D shape retrieval through pivoting</a><br>
      <small>Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://arxiv.org/abs/2302.07669" target="_blank" rel="noopener noreferrer">Unsupervised hashing with similarity distribution calibration</a><br>
      <small>Kam Woh Ng, Xiatian Zhu, Jiun Tian Hoe, Chee Seng Chan, Tianyu Zhang, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2023</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10273439/" target="_blank" rel="noopener noreferrer">Semi-supervised learning for FGVC with out-of-category data</a><br>
      <small>Ruoyi Du, Dongliang Chang, Zhanyu Ma, Kongming Liang, Yi-Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://arxiv.org/abs/2311.07261" target="_blank" rel="noopener noreferrer">Sketch-based video object segmentation: benchmark and analysis</a><br>
      <small>Ruolin Yang, Da Li, Conghui Hu, Timothy Hospedales, Honggang Zhang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">PhD Thesis 2023</span><br>
      <a href="https://openresearch.surrey.ac.uk/esploro/outputs/doctoral/SceneTrilogy-On-Scene-Sketches-and-its/99958466602346" target="_blank" rel="noopener noreferrer">SceneTrilogy: on scene sketches and its relationship with text and photo</a><br>
      <small>Pinaki Nath Chowdhury</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Li_Photo_Pre-Training_but_for_Sketch_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Photo Pre-Training, But for Sketch</a><br>
      <small>, Ke Li, Kaiyue Pang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Li_Photo_Pre-Training_but_for_Sketch_CVPR_2023_paper.html" target="_blank" rel="noopener noreferrer">Photo Pre-Training, But for Sketch</a><br>
      <small>, Ke Li, Kaiyue Pang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://arxiv.org/abs/2303.05734" target="_blank" rel="noopener noreferrer">Generative Model Based Noise Robust Training for Unsupervised Domain Adaptation</a><br>
      <small>, Zhongying Deng, Da Li, Junjun He, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv230315149N/abstract" target="_blank" rel="noopener noreferrer">What Can Human Sketches Do for Object Detection?</a><br>
      <small>, Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2023</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv231115477W/abstract" target="_blank" rel="noopener noreferrer">DreamCreature: Crafting Photorealistic Virtual Creatures from Imagination</a><br>
      <small>, Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2023</span><br>
      <a href="https://openaccess.thecvf.com/content/CVPR2023/supplemental/Li_Photo_Pre-Training_but_CVPR_2023_supplemental.pdf" target="_blank" rel="noopener noreferrer">Supplementary material: Photo Pre-Training, But for Sketch</a><br>
      <small>, Ke Li, Kaiyue Pang, Yi-Zhe Song, CVSSP SketchX</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TNNLS 2022</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9706366/" target="_blank" rel="noopener noreferrer">Deep learning for free-hand sketch: A survey</a><br>
      <small>, Peng Xu, Timothy M Hospedales, Qiyue Yin, Yi-Zhe Song, Tao Xiang, Liang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022/html/He_Style-Based_Global_Appearance_Flow_for_Virtual_Try-On_CVPR_2022_paper.html" target="_blank" rel="noopener noreferrer">Style-based global appearance flow for virtual try-on</a><br>
      <small>, Sen He, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_39" target="_blank" rel="noopener noreferrer">Zero-shot temporal action detection via vision-language prompting</a><br>
      <small>, Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2022</span><br>
      <a href="https://ojs.aaai.org/index.php/AAAI/article/view/20226" target="_blank" rel="noopener noreferrer">Hybrid graph neural networks for few-shot learning</a><br>
      <small>, Tianyuan Yu, Sen He, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Bhunia_Sketching_Without_Worrying_Noise-Tolerant_Sketch-Based_Image_Retrieval_CVPR_2022_paper.html" target="_blank" rel="noopener noreferrer">Sketching without worrying: Noise-tolerant sketch-based image retrieval</a><br>
      <small>, Ayan Kumar Bhunia, Subhadeep Koley, Abdullah Faiz Ur Rahman Khilji, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_37" target="_blank" rel="noopener noreferrer">Proposal-free temporal action detection via global segmentation mask learning</a><br>
      <small>, Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Sain_Sketch3T_Test-Time_Training_for_Zero-Shot_SBIR_CVPR_2022_paper.html" target="_blank" rel="noopener noreferrer">Sketch3t: Test-time training for zero-shot sbir</a><br>
      <small>, Aneeshan Sain, Ayan Kumar Bhunia, Vaishnav Potlapalli, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-19833-5_37" target="_blank" rel="noopener noreferrer">Fashionvil: Fashion-focused vision-and-language representation learning</a><br>
      <small>, Xiao Han, Licheng Yu, Xiatian Zhu, Li Zhang, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2022</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9813442/" target="_blank" rel="noopener noreferrer">Dynamic instance domain adaptation</a><br>
      <small>, Zhongying Deng, Kaiyang Zhou, Da Li, Junjun He, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Bhunia_Doodle_It_Yourself_Class_Incremental_Learning_by_Drawing_a_Few_CVPR_2022_paper.html" target="_blank" rel="noopener noreferrer">Doodle it yourself: Class incremental learning by drawing a few sketches</a><br>
      <small>, Ayan Kumar Bhunia, Viswanatha Reddy Gajjala, Subhadeep Koley, Rohit Kundu, Aneeshan Sain, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-19836-6_10" target="_blank" rel="noopener noreferrer">Adaptive fine‑grained sketch‑based image retrieval</a><br>
      <small>, Ayan Kumar Bhunia, Aneeshan Sain, Parth Hiren Shah, Animesh Gupta, Pinaki Nath Chowdhury, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_38" target="_blank" rel="noopener noreferrer">Semi‑supervised temporal action detection with proposal‑free masking</a><br>
      <small>, Sauradip Nag, Xiatian Zhu, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2022</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-031-19769-7_27" target="_blank" rel="noopener noreferrer">Sketchsampler: Sketch‑based 3d reconstruction via view‑dependent depth sampling</a><br>
      <small>, Chenjian Gao, Qian Yu, Lu Sheng, Yi‑Zhe Song, Dong Xu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ArXiv 2022</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9739995/" target="_blank" rel="noopener noreferrer">One sketch for all: One‑shot personalized sketch segmentation</a><br>
      <small>, Anran Qi, Yulia Gryaditskaya, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ArXiv 2022</span><br>
      <a href="https://www.research.ed.ac.uk/en/publications/sketchode-learning-neural-sketch-representation-in-continuous-tim" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Sketchode: Learning neural sketch representation in continuous time</a><br>
      <small>Ayan Das, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ArXiv 2022</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9686584/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Exploring local detail perception for scene sketch semantic segmentation</a><br>
      <small>Ce Ge, Haifeng Sun, Yi‑Zhe Song, Zhanyu Ma, Jianxin Liao</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #e91e63; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TOG 2022</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/3550454.3555493" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Differsketching: How differently do people sketch 3d objects?</a><br>
      <small>Chufeng Xiao, Wanchao Su, Jing Liao, Zhouhui Lian, Yi‑Zhe Song, Hongbo Fu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IJCV 2022</span><br>
      <a href="https://link.springer.com/article/10.1007/s11263-022-01623-7" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Generative sketch healing</a><br>
      <small>Yonggang Qi, Guoyao Su, Qiang Wang, Jie Yang, Kaiyue Pang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">3DV 2022</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/10044450/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Structure‑aware 3d vr sketch to 3d shape retrieval</a><br>
      <small>Ling Luo, Yulia Gryaditskaya, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0097849322001078" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">A study of deep single sketch‑based modeling: View/style invariance, sparsity and latent space disentanglement</a><br>
      <small>Yue Zhong, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ArXiv 2022</span><br>
      <a href="https://arxiv.org/abs/2210.01676" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Robust target training for multi‑source domain adaptation</a><br>
      <small>Zhongying Deng, Da Li, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPRW 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022W/CVFAD/html/Han_UIGR_Unified_Interactive_Garment_Retrieval_CVPRW_2022_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Uigr: Unified interactive garment retrieval</a><br>
      <small>Xiao Han, Sen He, Li Zhang, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2022</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Yang_Finding_Badly_Drawn_Bunnies_CVPR_2022_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Finding badly drawn bunnies</a><br>
      <small>Lan Yang, Kaiyue Pang, Honggang Zhang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ArXiv 2022</span><br>
      <a href="https://arxiv.org/abs/2211.10715" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Single stage multi‑pose virtual try-on</a><br>
      <small>Sen He, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://arxiv.org/abs/2211.14905" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Multi-Modal Few-Shot Temporal Action Detection</a><br>
      <small>Sauradip Nag, Mengmeng Xu, Xiao Han, Xiatian Zhu, Bernard Ghanem, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://arxiv.org/abs/2210.14271" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Learning to Augment via Implicit Differentiation for Domain Generalization</a><br>
      <small>Tingwei Wang, Da Li, Kaiyang Zhou, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPRW 2022</span><br>
      <a href="https://openaccess.thecvf.com/content/CVPR2022W/L3D-IVU/html/Xiang_CDAD_A_Common_Daily_Action_Dataset_With_Collected_Hard_Negative_CVPRW_2022_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">CDAD: A Common Daily Action Dataset with Collected Hard Negative Samples</a><br>
      <small>Wangmeng Xiang, Chao Li, Ke Li, Biao Wang, Xian-sheng Hua, Lei Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220411964N/abstract" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">SceneTrilogy: On Human Scene-Sketch and its Complementarity with Photo and Text</a><br>
      <small>Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://arxiv.org/abs/2209.10020" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Towards 3D VR-Sketch to 3D Shape Retrieval</a><br>
      <small>Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220314804N/abstract" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Partially Does It: Towards Scene-Level FG-SBIR with Partial Input</a><br>
      <small>Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Viswanatha Reddy Gajjala, Aneeshan Sain, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2022</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220302113N/abstract" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">FS-COCO: Towards Understanding of Freehand Sketches of Common Objects in Context</a><br>
      <small>Pinaki Nath Chowdhury, Aneeshan Sain, Ayan Kumar Bhunia, Tao Xiang, Yulia Gryaditskaya, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">3DV 2022</span><br>
      <a href="https://www.pinakinathc.me/assets/papers/3DV_2022_supp.pdf" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Garment Ideation: Iterative View-Aware Sketch-Based Garment Modeling Supplemental</a><br>
      <small>Pinaki Nath Chowdhury, Tuanfeng Wang, Duygu Ceylan, Yi-Zhe Song, Yulia Gryaditskaya</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2021</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9609630/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Fine-grained image analysis with deep learning: A survey</a><br>
      <small>Xiu-Shen Wei, Yi-Zhe Song, Oisin Mac Aodha, Jianxin Wu, Yuxin Peng, Jinhui Tang, Jian Yang, Serge Belongie</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Lu_Simpler_Is_Better_Few-Shot_Semantic_Segmentation_With_Classifier_Weight_Transformer_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Simpler is better: Few-shot semantic segmentation with classifier weight transformer</a><br>
      <small>Zhihe Lu, Sen He, Xiatian Zhu, Li Zhang, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Chang_Your_Flamingo_is_My_Bird_Fine-Grained_or_Not_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Your "Flamingo" is My "Bird": Fine-Grained, or Not</a><br>
      <small>Dongliang Chang, Kaiyue Pang, Yixiao Zheng, Zhanyu Ma, Yi-Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Sain_StyleMeUp_Towards_Style-Agnostic_Sketch-Based_Image_Retrieval_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Stylemeup: Towards style-agnostic sketch-based image retrieval</a><br>
      <small>Aneeshan Sain, Ayan Kumar Bhunia, Yongxin Yang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TPAMI 2021</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9609669/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Progressive learning of category-consistent multi-granularity features for fine-grained visual classification</a><br>
      <small>Ruoyi Du, Jiyang Xie, Zhanyu Ma, Dongliang Chang, Yi-Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_More_Photos_Are_All_You_Need_Semi-Supervised_Learning_for_Fine-Grained_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">More photos are all you need: Semi-supervised learning for fine-grained sketch based image retrieval</a><br>
      <small>Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Yongxin Yang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Joint_Visual_Semantic_Reasoning_Multi-Stage_Decoder_for_Text_Recognition_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Joint visual semantic reasoning: Multi-stage decoder for text recognition</a><br>
      <small>Ayan Kumar Bhunia, Aneeshan Sain, Amandeep Kumar, Shuvozit Ghose, Pinaki Nath Chowdhury, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_Vectorization_and_Rasterization_Self-Supervised_Learning_for_Sketch_and_Handwriting_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Vectorization and rasterization: Self-supervised learning for sketch and handwriting</a><br>
      <small>Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/He_Context-Aware_Layout_to_Image_Generation_With_Enhanced_Object_Appearance_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Context-aware layout to image generation with enhanced object appearance</a><br>
      <small>Sen He, Wentong Liao, Michael Ying Yang, Yongxin Yang, Yi-Zhe Song, Bodo Rosenhahn, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Chen_Variational_Attention_Propagating_Domain-Specific_Knowledge_for_Multi-Domain_Learning_in_Crowd_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Variational attention: Propagating domain-specific knowledge for multi-domain learning in crowd counting</a><br>
      <small>Binghui Chen, Zhaoyi Yan, Ke Li, Pengyu Li, Biao Wang, Wangmeng Zuo, Lei Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IJCV 2021</span><br>
      <a href="https://link.springer.com/article/10.1007/s11263-020-01382-3" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Fine-grained instance-level sketch-based image retrieval</a><br>
      <small>Qian Yu, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9573376/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Toward fine-grained sketch-based 3D shape retrieval</a><br>
      <small>Anran Qi, Yulia Gryaditskaya, Jifei Song, Yongxin Yang, Yonggang Qi, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_MetaHTR_Towards_Writer-Adaptive_Handwritten_Text_Recognition_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Metahtr: Towards writer-adaptive handwritten text recognition</a><br>
      <small>Ayan Kumar Bhunia, Shuvozit Ghose, Amandeep Kumar, Pinaki Nath Chowdhury, Aneeshan Sain, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Das_Cloud2Curve_Generation_and_Vectorization_of_Parametric_Sketches_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Cloud2curve: Generation and vectorization of parametric sketches</a><br>
      <small>Ayan Das, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/He_Disentangled_Lifespan_Face_Synthesis_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Disentangled lifespan face synthesis</a><br>
      <small>Sen He, Wentong Liao, Michael Ying Yang, Yi-Zhe Song, Bodo Rosenhahn, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Text_Is_Text_No_Matter_What_Unifying_Text_Recognition_Using_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Text is text, no matter what: Unifying text recognition using knowledge distillation</a><br>
      <small>Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Yang_SketchAA_Abstract_Representation_for_Abstract_Sketches_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Sketchaa: Abstract representation for abstract sketches</a><br>
      <small>Lan Yang, Kaiyue Pang, Honggang Zhang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Qi_SketchLattice_Latticed_Representation_for_Sketch_Manipulation_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Sketchlattice: Latticed representation for sketch manipulation</a><br>
      <small>Yonggang Qi, Guoyao Su, Pinaki Nath Chowdhury, Mingkang Li, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Towards_the_Unseen_Iterative_Text_Recognition_by_Distilling_From_Errors_ICCV_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Towards the unseen: Iterative text recognition by distilling from errors</a><br>
      <small>Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">3DV 2021</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9665875/" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Fine-grained vr sketching: Dataset and insights</a><br>
      <small>Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2021</span><br>
      <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Qi_PQA_Perceptual_Question_Answering_CVPR_2021_paper.html" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Pqa: Perceptual question answering</a><br>
      <small>Yonggang Qi, Kai Zhang, Aneeshan Sain, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2021</span><br>
      <a href="https://arxiv.org/abs/2105.08237" target="_blank" rel="noopener noreferrer" target="_blank" rel="noopener noreferrer">Towards unsupervised sketch-based image retrieval</a><br>
      <small>Conghui Hu, Yongxin Yang, Yunpeng Li, Timothy M Hospedales, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #ff9800; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">NeurIPS 2021</span><br>
      <a href="https://openreview.net/forum?id=VuEqOs9Yp7Q" target="_blank" target="_blank" rel="noopener noreferrer">Temporal action localization with global segmentation mask transformers</a><br>
      <small>, Sauradip Nag, Xiatian Zhu, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2021</span><br>
      <a href="https://arxiv.org/abs/2112.02825" target="_blank" target="_blank" rel="noopener noreferrer">Clue me in: Semi-supervised FGVC with Out-of-Distribution Data</a><br>
      <small>, Ruoyi Du, Dongliang Chang, Zhanyu Ma, Yi‑Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2021</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2021arXiv210914449T/abstract" target="_blank" target="_blank" rel="noopener noreferrer">One Loss for All: Deep Hashing with a Single Cosine Similarity based Learning Objective</a><br>
      <small>, Jiun Tian Hoe, Kam Woh Ng, Tianyu Zhang, Chee Seng Chan, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2020</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-030-58565-5_10" target="_blank" target="_blank" rel="noopener noreferrer">Fine-grained visual classification via progressive multi-granularity training of jigsaw patches</a><br>
      <small>, Ruoyi Du, Dongliang Chang, Ayan Kumar Bhunia, Jiyang Xie, Yi‑Zhe Song, Zhanyu Ma, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9005389/" target="_blank" target="_blank" rel="noopener noreferrer">The devil is in the channels: Mutual-channel loss for fine-grained image classification</a><br>
      <small>, Dongliang Chang, Yifeng Ding, Jiyang Xie, Ayan Kumar Bhunia, Xiaoxu Li, Zhanyu Ma, Ming Wu, Jun Guo, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2020</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Lu_Stochastic_Classifiers_for_Unsupervised_Domain_Adaptation_CVPR_2020_paper.html" target="_blank" target="_blank" rel="noopener noreferrer">Stochastic classifiers for unsupervised domain adaptation</a><br>
      <small>, Zhihe Lu, Yongxin Yang, Xiatian Zhu, Cong Liu, Yi‑Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2020</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Bhunia_Sketch_Less_for_More_On-the-Fly_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2020_paper" target="_blank" target="_blank" rel="noopener noreferrer">Sketch less for more: On-the-fly fine-grained sketch-based image retrieval</a><br>
      <small>, Ayan Kumar Bhunia, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2020</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Pang_Solving_Mixed-Modal_Jigsaw_Puzzle_for_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2020_paper.html" target="_blank" target="_blank" rel="noopener noreferrer">Solving mixed-modal jigsaw puzzle for fine-grained sketch-based image retrieval</a><br>
      <small>, Kaiyue Pang, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #4caf50; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICML 2020</span><br>
      <a href="https://proceedings.mlr.press/v119/zhang20g.html" target="_blank" target="_blank" rel="noopener noreferrer">A Tree-Structured Decoder for Image-to-Markup Generation</a><br>
      <small>, Jianshu Zhang, Jun Du, Yongxin Yang, Yi‑Zhe Song, Si Wei, Lirong Dai</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2020</span><br>
      <a href="https://arxiv.org/abs/2007.15103" target="_blank" target="_blank" rel="noopener noreferrer">Cross-Modal Hierarchical Modelling for Fine-Grained Sketch Based Image Retrieval</a><br>
      <small>, Aneeshan Sain, Ayan Kumar Bhunia, Yongxin Yang, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2020</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-030-58574-7_38" target="_blank" target="_blank" rel="noopener noreferrer">BézierSketch: A generative model for scalable vector sketches</a><br>
      <small>, Ayan Das, Yongxin Yang, Timothy Hospedales, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #e91e63; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TOG 2020</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/3414685.3417840" target="_blank" target="_blank" rel="noopener noreferrer">Pixelor: A Competitive Sketching AI Agent. So you think you can sketch?</a><br>
      <small>, Ayan Kumar Bhunia, Ayan Das, Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yulia Gryaditskaya, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9119480/" target="_blank" target="_blank" rel="noopener noreferrer">Deep Self-Supervised Representation Learning for Free-Hand Sketch</a><br>
      <small>, Peng Xu, Zeyu Song, Qiyue Yin, Yi‑Zhe Song, Liang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9272370/" target="_blank" target="_blank" rel="noopener noreferrer">Towards practical sketch-based 3d shape generation: The role of professional sketches</a><br>
      <small>, Yue Zhong, Yonggang Qi, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9161000/" target="_blank" target="_blank" rel="noopener noreferrer">Fine-Grained Instance-Level Sketch-Based Video Retrieval</a><br>
      <small>, Peng Xu, Kun Liu, Tao Xiang, Timothy M Hospedales, Zhanyu Ma, Jun Guo, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">3DV 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9320101/" target="_blank" target="_blank" rel="noopener noreferrer">Deep Sketch-Based Modeling: Tips and Tricks</a><br>
      <small>, Yue Zhong, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2020</span><br>
      <a href="https://openresearch.surrey.ac.uk/esploro/outputs/conferencePresentation/SketchHealer-A-Graph-to-Sequence-Network-for-Recreating/99514536202346?institution=44SUR_INST" target="_blank" target="_blank" rel="noopener noreferrer">Sketchhealer a graph-to-sequence network for recreating partial human sketches</a><br>
      <small>, Guoyao Su, Yonggang Qi, Kaiyue Pang, Jie Yang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TMM 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9147045/" target="_blank" target="_blank" rel="noopener noreferrer">SRD: a tree structure based decoder for online handwritten mathematical expression recognition</a><br>
      <small>, Jianshu Zhang, Jun Du, Yongxin Yang, Yi‑Zhe Song, Lirong Dai</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2020</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-030-66415-2_39" target="_blank" target="_blank" rel="noopener noreferrer">Sequential Learning for Domain Generalization</a><br>
      <small>, Da Li, Yongxin Yang, Yi‑Zhe Song, Timothy Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICME 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9102957/" target="_blank" target="_blank" rel="noopener noreferrer">S3Net: Graph Representational Network For Sketch Recognition</a><br>
      <small>, Lan Yang, Aneeshan Sain, Linpeng Li, Yonggang Qi, Honggang Zhang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9216574/" target="_blank" rel="noopener noreferrer">Sketch-a-Segmenter: Sketch-based Photo Segmenter Generation</a><br>
      <small>Conghui Hu, Da Li, Yongxin Yang, Timothy M Hospedales, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9163150/" target="_blank" rel="noopener noreferrer">SketchDesc: Learning Local Sketch Descriptors for Multi-view Correspondence</a><br>
      <small>Deng Yu, Lei Li, Youyi Zheng, Manfred Lau, Yi‑Zhe Song, Chew‑Lan Tai, Hongbo Fu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">3DV 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9320353/" target="_blank" rel="noopener noreferrer">Towards 3D VR-Sketch to 3D Shape Retrieval</a><br>
      <small>Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9274399/" target="_blank" rel="noopener noreferrer">On learning semantic representations for large-scale abstract sketches</a><br>
      <small>Peng Xu, Yongye Huang, Tongtong Yuan, Tao Xiang, Timothy Hospedales, Yi‑Zhe Song, Liang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IEEE 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/9254098/" target="_blank" rel="noopener noreferrer">IEEE access special section editorial: AI-driven big data processing: Theory, methodology, and applications</a><br>
      <small>Zhanyu Ma, Sunwoo Kim, Pascual Martínez‑Gómez, Jalil Taghia, Yi‑Zhe Song, Huiji Gao</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2020</span><br>
      <a href="https://arxiv.org/abs/2003.03787" target="_blank" rel="noopener noreferrer">Mind the gap: Enlarging the domain gap in open set domain adaptation</a><br>
      <small>Dongliang Chang, Aneeshan Sain, Zhanyu Ma, Yi‑Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2020</span><br>
      <a href="https://arxiv.org/abs/2007.04101" target="_blank" rel="noopener noreferrer">On Learning Semantic Representations for Million-Scale Free-Hand Sketches</a><br>
      <small>Peng Xu, Yongye Huang, Tongtong Yuan, Tao Xiang, Timothy M Hospedales, Yi‑Zhe Song, Liang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #e91e63; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TOG 2020</span><br>
      <a href="https://scholar.google.com/scholar?cluster=10431522207885335387&hl=en&oi=scholarr" target="_blank" rel="noopener noreferrer">Pixelor: a competitive sketching AI agent</a><br>
      <small>Ayan Kumar Bhunia, Ayan Das, Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yulia Gryaditskaya, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TCSVT 2020</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8949551/" target="_blank" rel="noopener noreferrer">Sketch fewer to recognize more by learning a co-regularized sparse representation</a><br>
      <small>Yonggang Qi, Yi‑Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2019</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Song_Generalizable_Person_Re-Identification_by_Domain-Invariant_Mapping_Network_CVPR_2019_paper.html" target="_blank" rel="noopener noreferrer">Generalizable person re-identification by domain-invariant mapping network</a><br>
      <small>Jifei Song, Yongxin Yang, Yi‑Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2019</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Dey_Doodle_to_Search_Practical_Zero-Shot_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" target="_blank" rel="noopener noreferrer">Doodle to search: Practical zero-shot sketch-based image retrieval</a><br>
      <small>Sounak Dey, Pau Riba, Anjan Dutta, Josep Llados, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2019</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Pang_Generalising_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" target="_blank" rel="noopener noreferrer">Generalising fine-grained sketch-based image retrieval</a><br>
      <small>Kaiyue Pang, Ke Li, Yongxin Yang, Honggang Zhang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2019</span><br>
      <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Pang_Generalising_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" target="_blank" rel="noopener noreferrer">Generalising fine-grained sketch-based image retrieval</a><br>
      <small>Kaiyue Pang, Ke Li, Yongxin Yang, Honggang Zhang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2019</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/3306618.3314233" target="_blank" rel="noopener noreferrer">AI+ art= human</a><br>
      <small>Antonio Daniele, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2019</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8809264/" target="_blank" rel="noopener noreferrer">Semi-heterogeneous three-way joint embedding network for sketch-based image retrieval</a><br>
      <small>Jianjun Lei, Yuxin Song, Bo Peng, Zhanyu Ma, Ling Shao, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2019</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8626530/" target="_blank" rel="noopener noreferrer">Toward deep universal sketch perceptual grouper</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2019</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8626530/" target="_blank" rel="noopener noreferrer">Toward deep universal sketch perceptual grouper</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">xCoAx 2019</span><br>
      <a href="https://scholar.google.com/scholar?cluster=11059045185456022370&hl=en&oi=scholarr" target="_blank" rel="noopener noreferrer">Artistic Assemblage</a><br>
      <small>Yi-Zhe Song, Daniele Antonio</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2019</span><br>
      <a href="https://ui.adsabs.harvard.edu/abs/2019arXiv190712336R/abstract" target="_blank" rel="noopener noreferrer">Goal-Driven Sequential Data Abstraction</a><br>
      <small>Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2018</span><br>
      <a href="https://ojs.aaai.org/index.php/AAAI/article/view/11596" target="_blank" rel="noopener noreferrer">Learning to generalize: Meta-learning for domain generalization</a><br>
      <small>Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Xu_SketchMate_Deep_Hashing_CVPR_2018_paper.html" target="_blank" rel="noopener noreferrer">Sketchmate: Deep hashing for million-scale human sketch retrieval</a><br>
      <small>, Peng Xu, Yongye Huang, Tongtong Yuan, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Zhanyu Ma, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Song_Learning_to_Sketch_CVPR_2018_paper.html" target="_blank" rel="noopener noreferrer">Learning to sketch with shortcut cycle consistency</a><br>
      <small>, Jifei Song, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TNNLS 2018</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8401709/" target="_blank" rel="noopener noreferrer">Variational Bayesian learning for Dirichlet process mixture of inverted Dirichlet distributions in non-Gaussian image feature modeling</a><br>
      <small>, Zhanyu Ma, Yuping Lai, W Bastiaan Kleijn, Yi-Zhe Song, Liang Wang, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Muhammad_Learning_Deep_Sketch_CVPR_2018_paper.html" target="_blank" rel="noopener noreferrer">Learning deep sketch abstraction</a><br>
      <small>, Umar Riaz Muhammad, Yongxin Yang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Changqing_Zou_SketchyScene_Richly-Annotated_Scene_ECCV_2018_paper.html" target="_blank" rel="noopener noreferrer">Sketchyscene: Richly-annotated scene sketches</a><br>
      <small>, Changqing Zou, Qian Yu, Ruofei Du, Haoran Mo, Yi-Zhe Song, Tao Xiang, Chengying Gao, Baoquan Chen, Hao Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ACM 2018</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/3240508.3240606" target="_blank" rel="noopener noreferrer">Cross-domain adversarial feature learning for sketch re-identification</a><br>
      <small>, Lu Pang, Yaowei Wang, Yi-Zhe Song, Tiejun Huang, Yonghong Tian</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Ke_LI_Universal_Sketch_Perceptual_ECCV_2018_paper.html" target="_blank" rel="noopener noreferrer">Universal sketch perceptual grouping</a><br>
      <small>, Ke Li, Kaiyue Pang, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Ke_LI_Universal_Sketch_Perceptual_ECCV_2018_paper.html" target="_blank" rel="noopener noreferrer">Universal sketch perceptual grouping</a><br>
      <small>, Ke Li, Kaiyue Pang, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2018</span><br>
      <a href="https://scholar.archive.org/work/i7rkm2e5abexnn7ekmbthedx2e/access/wayback/http://bmvc2018.org/contents/papers/0040.pdf" target="_blank" rel="noopener noreferrer">Semantic Embedding for Sketch-Based 3D Shape Retrieval</a><br>
      <small>, Anran Qi, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Hu_Sketch-a-Classifier_Sketch-Based_Photo_CVPR_2018_paper.html" target="_blank" rel="noopener noreferrer">Sketch-a-classifier: Sketch-based photo classifier generation</a><br>
      <small>, Conghui Hu, Da Li, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2018</span><br>
      <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Kaiyue_Pang_Deep_Factorised_Inverse-Sketching_ECCV_2018_paper.html" target="_blank" rel="noopener noreferrer">Deep factorised inverse-sketching</a><br>
      <small>, Kaiyue Pang, Da Li, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">NIPS 2018</span><br>
      <a href="https://scholar.google.com/scholar?cluster=11748417708108091907&hl=en&oi=scholarr" target="_blank" rel="noopener noreferrer">Greedy hash: Towards fast optimization for accurate hash coding in CNN</a><br>
      <small>, Jiun Tian Hoe, Kam Woh Ng, Tianyu Zhang, Chee Seng Chan, Yi-Zhe Song, Tao Xiang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IEEE Access 2018</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8395088/" target="_blank" rel="noopener noreferrer">IEEE Access special section editorial: Recent advantages of computer vision</a><br>
      <small>, Zhanyu Ma, Haibin Ling, Yi-Zhe Song, Timothy Hospedales, Wei Jia, Yuxin Peng, Aili Han</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #673ab7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">Neurocomputing 2018</span><br>
      <a href="https://openresearch.surrey.ac.uk/esploro/outputs/journalArticle/Recent-advances-in-machine-learning-for/99511114602346" target="_blank" rel="noopener noreferrer">Recent advances in machine learning for non-Gaussian data processing</a><br>
      <small>, Zhanyu Ma, J-T Chien, Z-H Tan, Yi-Zhe Song, Jalil Taghia, Ming Xiao</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2017</span><br>
      <a href="http://openaccess.thecvf.com/content_iccv_2017/html/Li_Deeper_Broader_and_ICCV_2017_paper.html" target="_blank" rel="noopener noreferrer">Deeper, Broader and Artier Domain Generalization</a><br>
      <small>, Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M. Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IJCV 2017</span><br>
      <a href="https://link.springer.com/article/10.1007/s11263-016-0932-3" target="_blank" rel="noopener noreferrer">Sketch-a-net: A deep neural network that beats humans</a><br>
      <small>, Qian Yu, Yongxin Yang, Feng Liu, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICCV 2017</span><br>
      <a href="http://openaccess.thecvf.com/content_iccv_2017/html/Song_Deep_Spatial-Semantic_Attention_ICCV_2017_paper.html" target="_blank" rel="noopener noreferrer">Deep Spatial-Semantic Attention for Fine-Grained Sketch-Based Image Retrieval</a><br>
      <small>, Jifei Song, Yu Qian, Yi-Zhe Song, Tao Xiang, Timothy Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">arXiv 2017</span><br>
      <a href="https://arxiv.org/abs/1711.08106" target="_blank" rel="noopener noreferrer">The devil is in the middle: Exploiting mid-level representations for cross-domain instance matching</a><br>
      <small>, Qian Yu, Xiaobin Chang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2017</span><br>
      <a href="https://www.research.ed.ac.uk/en/publications/cross-domain-generative-learning-for-fine-grained-sketch-based-im" target="_blank" rel="noopener noreferrer">Cross-domain Generative Learning for Fine-Grained Sketch-Based Image Retrieval</a><br>
      <small>, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M. Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #673ab7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">Neurocomputing 2017</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0925231217314364" target="_blank" rel="noopener noreferrer">Cross-modal Subspace Learning for Fine-grained Sketch-based Image Retrieval</a><br>
      <small>, Peng Xu, Qiyue Yin, Yongye Huang, Yi-Zhe Song, Zhanyu Ma, Liang Wang, Tao Xiang, W Bastiaan Kleijn, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2017</span><br>
      <a href="https://www.research.ed.ac.uk/en/publications/fine-grained-image-retrieval-the-textsketch-input-dilemma" target="_blank" target="_blank" rel="noopener noreferrer">Fine-Grained Image Retrieval: the Text/Sketch Input Dilemma</a><br>
      <small>Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M. Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2017</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8016664/" target="_blank" target="_blank" rel="noopener noreferrer">Synergistic instance-level subspace alignment for fine-grained sketch-based image retrieval</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy M Hospedales, Tao Xiang, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2017</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/8016664/" target="_blank" target="_blank" rel="noopener noreferrer">Synergistic instance-level subspace alignment for fine-grained sketch-based image retrieval</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy M Hospedales, Tao Xiang, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2017</span><br>
      <a href="https://scholar.google.com/scholar?cluster=6337503410293765834&hl=en&oi=scholarr" target="_blank" target="_blank" rel="noopener noreferrer">Sketch-a-net that beats humans [OL]</a><br>
      <small>Q Yu, Y Yang, YZ Song, T Xiang, TM Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2017</span><br>
      <a href="https://www.research.ed.ac.uk/en/publications/now-you-see-me-deep-face-hallucination-for-unviewed-sketches" target="_blank" target="_blank" rel="noopener noreferrer">Now You See Me: Deep Face Hallucination for Unviewed Sketches</a><br>
      <small>Conghui Hu, Da Li, Yi-Zhe Song, Timothy M. Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2017</span><br>
      <a href="https://scholar.google.com/scholar?cluster=197706842303472179&hl=en&oi=scholarr" target="_blank" target="_blank" rel="noopener noreferrer">„Deeper</a><br>
      <small>D Li, Y Yang, YZ Song, T Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7532801/" target="_blank" target="_blank" rel="noopener noreferrer">Sketch-based image retrieval via siamese convolutional neural network</a><br>
      <small>Yonggang Qi, Yi-Zhe Song, Honggang Zhang, Jun Liu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IVC 2016</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0262885616301524" target="_blank" target="_blank" rel="noopener noreferrer">A survey on heterogeneous face recognition: Sketch, infra-red, 3D and low-resolution</a><br>
      <small>Shuxin Ouyang, Timothy Hospedales, Yi-Zhe Song, Xueming Li, Chen Change Loy, Xiaogang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2016</span><br>
      <a href="http://openaccess.thecvf.com/content_cvpr_2016/html/Ouyang_ForgetMeNot_Memory-Aware_Forensic_CVPR_2016_paper.html" target="_blank" target="_blank" rel="noopener noreferrer">Forgetmenot: Memory-aware forensic facial sketch matching</a><br>
      <small>Shuxin Ouyang, Timothy M Hospedales, Yi-Zhe Song, Xueming Li</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IJCV 2016</span><br>
      <a href="https://link.springer.com/article/10.1007/s11263-016-0963-9" target="_blank" target="_blank" rel="noopener noreferrer">Free-hand sketch synthesis with deformable stroke models</a><br>
      <small>Y. Li, Y-Z. Song, T. Hospedales, S. Gong</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #f44336; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">AAAI 2016</span><br>
      <a href="https://www.research.ed.ac.uk/en/publications/deep-multi-task-attribute-driven-ranking-for-fine-grained-sketch-" target="_blank" target="_blank" rel="noopener noreferrer">Deep multi-task attribute-driven ranking for fine-grained sketch-based image retrieval</a><br>
      <small>Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy Hospedales, Xiang Ruan</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">WACV 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7477615/" target="_blank" target="_blank" rel="noopener noreferrer">Fine-grained sketch-based image retrieval: The role of part-aware attributes</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy Hospedales, Honggang Zhang, Yichuan Hu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">WACV 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7477615/" target="_blank" target="_blank" rel="noopener noreferrer">Fine-grained sketch-based image retrieval: The role of part-aware attributes</a><br>
      <small>Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy Hospedales, Honggang Zhang, Yichuan Hu</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2016</span><br>
      <a href="https://scholar.google.com/scholar?cluster=13550880441023903228&hl=en&oi=scholarr" target="_blank" target="_blank" rel="noopener noreferrer">Sketch me that shoe</a><br>
      <small>Yyu Qian, Liu Feng, Yi-Zhe Song, Xiang Tao, Change Loy Chen</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IC-NIDC 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7974625/" target="_blank" target="_blank" rel="noopener noreferrer">Cross-modal subspace learning for sketch-based image retrieval: A comparative study</a><br>
      <small>Peng Xu, Ke Li, Zhanyu Ma, Yi-Zhe Song, Liang Wang, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IC-NIDC 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7974625/" target="_blank" target="_blank" rel="noopener noreferrer">Cross-modal subspace learning for sketch-based image retrieval: A comparative study</a><br>
      <small>Peng Xu, Ke Li, Zhanyu Ma, Yi-Zhe Song, Liang Wang, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">VCIP 2016</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7805451/" target="_blank" target="_blank" rel="noopener noreferrer">Cross-modal face matching: Tackling visual abstraction using fine-grained attributes</a><br>
      <small>Yichuan Hu, Ke Li, Honggang Zhang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2015</span><br>
      <a href="https://arxiv.org/abs/1501.07873" target="_blank" target="_blank" rel="noopener noreferrer">Sketch-a-net that beats humans</a><br>
      <small>Qian Yu, Yongxin Yang, Yi-Zhe Song, Tao Xiang, Timothy Hospedales</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #2196f3; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVIU 2015</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S1077314215000375" target="_blank" target="_blank" rel="noopener noreferrer">Free-hand sketch recognition by multi-kernel feature learning</a><br>
      <small>Yi Li, Timothy M Hospedales, Yi-Zhe Song, Shaogang Gong</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVPR 2015</span><br>
      <a href="https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Qi_Making_Better_Use_2015_CVPR_paper.html" target="_blank" target="_blank" rel="noopener noreferrer">Making better use of edges via perceptual grouping</a><br>
      <small>Yonggang Qi, Yi-Zhe Song, Tao Xiang, Honggang Zhang, Timothy Hospedales, Yi Li, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2015</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0925231215003082" target="_blank" rel="noopener noreferrer">Im2sketch: Sketch generation by unconflicted perceptual grouping</a><br>
      <small>Yonggang Qi, Jun Guo, Yi-Zhe Song, Tao Xiang, Honggang Zhang, Zheng-Hua Tan</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TIP 2015</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0925231215000260" target="_blank" rel="noopener noreferrer">Multi-label learning with prior knowledge for facial expression analysis</a><br>
      <small>Kaili Zhao, Honggang Zhang, Zhanyu Ma, Yi-Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICME 2015</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7177409/" target="_blank" rel="noopener noreferrer">Refining graph matching using inherent structure information</a><br>
      <small>Wenzhao Li, Yi-Zhe Song, Andrea Cavallaro</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVG 2014</span><br>
      <a href="https://qmro.qmul.ac.uk/jspui/handle/123456789/6440" target="_blank" rel="noopener noreferrer">Fine-Grained Sketch-Based Image Retrieval by Matching Deformable Part Models</a><br>
      <small>Yi Li, Timothy M Hospedales, Yi-Zhe Song, Shaogang Gong</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">SHM 2014</span><br>
      <a href="https://journals.sagepub.com/doi/abs/10.1177/1475921714522841" target="_blank" rel="noopener noreferrer">Virtual visual sensors and their application in structural health monitoring</a><br>
      <small>Yi-Zhe Song, Chris R Bowen, Alicia H Kim, Aydin Nassehi, Julian Padget, Nick Gathercole</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ACCV 2014</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-319-16808-1_15" target="_blank" rel="noopener noreferrer">Cross-modal face matching: beyond viewed sketches</a><br>
      <small>Shuxin Ouyang, Timothy Hospedales, Yi-Zhe Song, Xueming Li</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #9c27b0; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">SPIE 2014</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0888327013006808" target="_blank" rel="noopener noreferrer">Non-invasive damage detection in beams using marker extraction and wavelets</a><br>
      <small>Yi-Zhe Song, Chris R Bowen, H Alicia Kim, Aydin Nassehi, Julian Padget, Nick Gathercole, Andrew Dent</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #0078d7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">IEEE NIDC 2014</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/7000322/" target="_blank" rel="noopener noreferrer">A Patch-based Sparse Representation for Sketch Recognition</a><br>
      <small>Yonggong Qi, Honggang Zhang, Yi-Zhe Song, Zheng-Hua Tan</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #ff5722; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ISVC 2014</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-319-14364-4_8" target="_blank" rel="noopener noreferrer">One-shot learning of sketch categories with co-regularized sparse coding</a><br>
      <small>Yonggang Qi, Wei-Shi Zheng, Tao Xiang, Yi-Zhe Song, Honggang Zhang, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #673ab7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">Neurocomputing 2013</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0925231213006309" target="_blank" rel="noopener noreferrer">Text extraction from natural scene image: A survey</a><br>
      <small>Honggang Zhang, Kaili Zhao, Yi-Zhe Song, Jun Guo</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2013</span><br>
      <a href="https://www.eecs.qmul.ac.uk/~sgg/papers/LiEtAl_BMVC2013.pdf" target="_blank" rel="noopener noreferrer">Sketch recognition by ensemble matching of structured features.</a><br>
      <small>Yi Li, Yi-Zhe Song, Shaogang Gong</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2013</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/6738056/" target="_blank" rel="noopener noreferrer">Sketching by perceptual grouping</a><br>
      <small>Yonggang Qi, Jun Guo, Yi Li, Honggang Zhang, Tao Xiang, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2013</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/6461879/" target="_blank" rel="noopener noreferrer">Abstract art by shape classification</a><br>
      <small>Yi-Zhe Song, David Pickup, Chuan Li, Paul Rosin, Peter Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CAE 2013</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/2487276.2487288" target="_blank" rel="noopener noreferrer">Simple art as abstractions of photographs</a><br>
      <small>Peter Hall, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">VCIP 2013</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/6706384/" target="_blank" rel="noopener noreferrer">Perceptual grouping via untangling Gestalt principles</a><br>
      <small>Yonggang Qi, Jun Guo, Yi Li, Honggang Zhang, Tao Xiang, Yi-Zhe Song, Zheng-Hua Tan</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #795548; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">VCIP 2013</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/6706330/" target="_blank" rel="noopener noreferrer">A multi-label classification approach for facial expression recognition</a><br>
      <small>Kaili Zhao, Honggang Zhang, Mingzhi Dong, Jun Guo, Yonggang Qi, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #673ab7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">Neurocomputing 2012</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S0925231212001956" target="_blank" rel="noopener noreferrer">Robust visual tracking using structural region hierarchy and graph matching</a><br>
      <small>Yi-Zhe Song, Chuan Li, Liang Wang, Peter Hall, Peiyi Shen</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2012</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/6418792/" target="_blank" rel="noopener noreferrer">A dataset for scene classification based on camera metadata</a><br>
      <small>Kaili Zhao, Can Cao, Honggang Zhang, Yizhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #e91e63; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">TOG 2011</span><br>
      <a href="https://dl.acm.org/doi/abs/10.1145/2070781.2024161" target="_blank" rel="noopener noreferrer">Modeling and generating moving trees from video</a><br>
      <small>Chuan Li, Oliver Deussen, Yi-Zhe Song, Phil Willis, Peter Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #2196f3; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">CVIU 2011</span><br>
      <a href="https://www.sciencedirect.com/science/article/pii/S1077314211000841" target="_blank" rel="noopener noreferrer">Learning invariant structure for object identification by using graph methods</a><br>
      <small>Bai Xiao, Song Yi-Zhe, Peter Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #9c27b0; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">SPIE 2011</span><br>
      <a href="https://www.spiedigitallibrary.org/conference-proceedings-of-spie/7983/79830R/Non-invasive-damage-detection-in-composite-beams-using-marker-extraction/10.1117/12.880055.short" target="_blank" rel="noopener noreferrer">Non-invasive damage detection in composite beams using marker extraction and wavelets</a><br>
      <small>Yi-Zhe Song, Chris Bowen, H Alicia Kim, Aydin Nassehi, Julian Padget, Nick Gathercore, Andrew Dent</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2010</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-642-15561-1_50" target="_blank" rel="noopener noreferrer">Finding semantic structures in image hierarchies using Laplacian graph energy</a><br>
      <small>Yi-Zhe Song, Pablo Arbelaez, Peter Hall, Chuan Li, Anupriya Balikai</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2010</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/5604693/" target="_blank" rel="noopener noreferrer">In search of perceptually salient groupings</a><br>
      <small>Yi-Zhe Song, Bai Xiao, Peter Hall, Liang Wang</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ISMAR 2009</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/5336462/" target="_blank" rel="noopener noreferrer">Mobile augmented reality based 3D snapshots</a><br>
      <small>Peter Keitler, Frieder Pankratz, Bjorn Schwerdtfeger, Daniel Pustka, Wolf Rodiger, Gudrun Klinker, Christian Rauch, Anup Chathoth, John Collomosse, Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">University of Bath 2009</span><br>
      <a href="https://scholar.google.com/scholar?cluster=1156167040563393860&hl=en&oi=scholarr" target="_blank" rel="noopener noreferrer">Hierarchical image descriptions for classification and painting</a><br>
      <small>Yi-Zhe Song</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #673ab7; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">EG 2008</span><br>
      <a href="https://diglib.eg.org/bitstream/handle/10.2312/COMPAESTH.COMPAESTH08.065-072/065-072.pdf?sequence=1" target="_blank" rel="noopener noreferrer">Arty Shapes.</a><br>
      <small>Yi-Zhe Song, Paul L Rosin, Peter M Hall, John P Collomosse</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #3f51b5; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ECCV 2008</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-540-89689-0_37" target="_blank" rel="noopener noreferrer">Structure is a visual class invariant</a><br>
      <small>Bai Xiao, Yi-Zhe Song, Anupriya Balika, Peter M Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #555555; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">SSPR 2008</span><br>
      <a href="https://link.springer.com/chapter/10.1007/978-3-540-89639-5_31" target="_blank" rel="noopener noreferrer">Stable image descriptions using Gestalt principles</a><br>
      <small>Yi-Zhe Song, Peter M Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2008</span><br>
      <a href="https://www.researchgate.net/profile/Paul-Rosin/publication/221259874_Shapes_Fit_For_Purpose/links/0fcfd5107ee7911fef000000/Shapes-Fit-For-Purpose.pdf" target="_blank" rel="noopener noreferrer">Shapes Fit For Purpose.</a><br>
      <small>Anupriya Balikai, Paul L Rosin, Yi-Zhe Song, Peter M Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">ICIP 2007</span><br>
      <a href="https://ieeexplore.ieee.org/abstract/document/4276077/" target="_blank" rel="noopener noreferrer">RTcams: A new perspective on nonphotorealistic rendering from photographs</a><br>
      <small>Peter M Hall, John P Collomosse, Yi-Zhe Song, Peiyi Shen, Chuan Li</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #009688; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">BMVC 2007</span><br>
      <a href="https://scholar.google.com/scholar?cluster=3987824411733545783&hl=en&oi=scholarr" target="_blank" rel="noopener noreferrer">Learning Object Classes from Structure.</a><br>
      <small>Xiao Bai, Yi-Zhe Song, Peter M Hall</small>
    </li>
<li style="margin-bottom: 1em;">
      <span style="display: inline-block; background: #607d8b; color: white; padding: 2px 6px; border-radius: 4px; font-size: 0.9em;">VVG 2005</span><br>
      <a href="https://diglib.eg.org/bitstreams/bd37c179-e25c-4076-ac93-6a9b0ccadfe6/download" target="_blank" rel="noopener noreferrer">Visual Recognition of Man-made Materials and Structures in an Office Environment.</a><br>
      <small>Yi-Zhe Song, Christopher P Town</small>
    </li>

  </ol>
</div>

<!-- Section: Awards -->
<div class="section" id="awards-section">
  <h2>🎖 Honors and Awards</h2>
  <ul>
    <li>🏆 <strong>Best Science Paper Award</strong> at <strong>BMVC 2015</strong></li>
    <li>🤝 Collaborations with <strong>law enforcement agencies</strong></li>
    <li>🛍️ Partnerships with <strong>online retail platforms</strong></li>
    <li>📄59 x CVPR, 15 x ICCV, 17 x ECCV, 5 x ICLR, 1 x ICML, 3 x NeurIPS </li>
  </ul>
</div>

<!-- Section: Projects -->
<div class="section" id="projects-section" >
  <h2>🚀Projects</h2>
  projects
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



