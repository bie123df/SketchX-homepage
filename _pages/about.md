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

  #slider-banner {
    position: relative;
    max-width: 800px;
    margin: 40px auto;
    overflow: hidden;
    border-radius: 10px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  }

  .bx-slider {
    display: flex;
    transition: transform 0.5s ease-in-out;
  }

  .slides {
    min-width: 100%;
    box-sizing: border-box;
  }

  .slides img {
    width: 100%;
    display: block;
    border-radius: 10px;
  }

  #slider-prev, #slider-next {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    font-size: 2em;
    color: rgba(0, 0, 0, 0.5);
    cursor: pointer;
    user-select: none;
    padding: 0 10px;
    z-index: 1;
  }

  #slider-prev { left: 0; }
  #slider-next { right: 0; }

  #slider-prev:hover, #slider-next:hover {
    color: #000;
  }

.dataset-gallery {
  display: flex;
  flex-direction: column;
  gap: 30px;
  margin-top: 1em;
}

.dataset-item {
  max-width: 650px;
}

.dataset-item img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  display: block;
}

.dataset-item figcaption {
  margin-top: 0.5em;
  font-size: 1em;
}

#downloads-section h3 {
  font-size: 1.6em;
  font-weight: 600;
  margin-top: 1.8em;
  margin-bottom: 0.6em;
  color: #ff6600;
}
  
</style>

<!-- Section: About -->
<div class="section" id="about-section">
  <h2>🌟 Welcome to SketchX</h2>

    <!-- Image Slider Banner (新增部分) -->
  <section id="slider-banner">
    <div class="bx-slider">
<div class="slides">
  <img src="{{ '/images/1.jpg' | relative_url }}" alt="SIGGRAPH Asia paper accepted!">
</div>
<div class="slides">
  <img src="{{ '/images/2.jpg' | relative_url }}" alt="Two Sketch papers in CVPR’20!">
</div>
<div class="slides">
  <img src="{{ '/images/3.jpg' | relative_url }}" alt="One paper in ECCV’20!">
</div>
<div class="slides">
  <img src="{{ '/images/4.jpg' | relative_url }}" alt="Two papers in ICCV’19!">
</div>

    </div>
    <span id="slider-prev">&#10094;</span>
    <span id="slider-next">&#10095;</span>
  </section>

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


<div class="entry-content">

<h3>Director:</h3>
<figure id="attachment_888" aria-describedby="caption-attachment-888" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.uk/citations?user=irZFP_AAAAAJ&amp;hl=en">
        <img decoding="async" class="wp-image-888" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/3-1-225x300.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-888" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=irZFP_AAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Yi-Zhe Song</a>
    </figcaption>
</figure>

<h3>Co-Directors:</h3>
<figure id="attachment_884" aria-describedby="caption-attachment-884" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.uk/citations?user=nHhtvqkAAAAJ&amp;hl=en">
        <img decoding="async" class="wp-image-884" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/19-224x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-884" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=nHhtvqkAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Timothy Hospedales</a>
    </figcaption>
</figure>
<figure id="attachment_883" aria-describedby="caption-attachment-883" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.uk/citations?user=MeS5d4gAAAAJ&amp;hl=en">
        <img decoding="async" class="wp-image-883" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/18-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-883" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=MeS5d4gAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Tao (Tony) Xiang</a>
    </figcaption>
</figure>
<figure id="attachment_868" aria-describedby="caption-attachment-868" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.de/citations?user=cBB96b4AAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-868" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/7fbee80a49088009cdcbaedb272af8f9.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-868" class="wp-caption-text">
        <a href="https://scholar.google.de/citations?user=cBB96b4AAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Yulia Gryaditskaya</a>
    </figcaption>
</figure>

<h3>Postdocs:</h3>
<figure id="attachment_867" aria-describedby="caption-attachment-867" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=kR3zzeUAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-868" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/Kaiyue_Jul2022-e1657365223297.jpeg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-867" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=kR3zzeUAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Kaiyue Pang</a>
    </figcaption>
</figure>

<h3>Affiliated Academics:</h3>
<figure id="attachment_869" aria-describedby="caption-attachment-869" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.uk/citations?user=F7PtrL8AAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-869" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2016/04/Yongxin-e1657364073846.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-869" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=F7PtrL8AAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Yongxin Yang</a>
    </figcaption>
</figure>
<figure id="attachment_881" aria-describedby="caption-attachment-881" style="width: 150px" class="wp-caption alignleft">
    <a href="https://qugank.github.io">
        <img loading="lazy" decoding="async" class="wp-image-881" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/yonggang-43.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-881" class="wp-caption-text">
        <a href="https://scholar.google.com.hk/citations?user=pQNpf7cAAAAJ&amp;hl=zh-CN" target="_blank" rel="noopener noreferrer">Yonggang Qi</a>
    </figcaption>
</figure>
<figure id="attachment_879" aria-describedby="caption-attachment-879" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=KZOFaz4AAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-879" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/WechatIMG17563.jpeg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-879" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=KZOFaz4AAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Ke Li</a>
    </figcaption>
</figure>

<h3>Current PhD Students:</h3>
<figure id="attachment_872" aria-describedby="caption-attachment-872" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-872" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/7-225x300.png" alt="" width="150" height="200">
    <figcaption id="caption-attachment-872" class="wp-caption-text">
        <a href="http://www.letitbrain.it/letitbrain/" target="_blank" rel="noopener noreferrer">Antonio Daniele</a>
    </figcaption>
</figure>
<figure id="attachment_871" aria-describedby="caption-attachment-871" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-871" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/6-225x300.png" alt="" width="150" height="200">
    <figcaption id="caption-attachment-871" class="wp-caption-text">Yue Zhong</figcaption>
</figure>
<figure id="attachment_1004" aria-describedby="caption-attachment-1004" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-1004" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2021/11/IMG_2892.jpg" alt="" width="150" height="200">
    <figcaption id="caption-attachment-1004" class="wp-caption-text">Lan Yang</figcaption>
</figure>
<figure id="attachment_905" aria-describedby="caption-attachment-905" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=tIf50PgAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-905" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/Dongliang-e1657361508702.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-905" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=tIf50PgAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Dongliang Chang</a>
    </figcaption>
</figure>
<figure id="attachment_908" aria-describedby="caption-attachment-908" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.in/citations?user=gjslbzsAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-908 size-full" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/85c2d7efffcb4849de402f1929796bb4.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-908" class="wp-caption-text">
        <a href="https://scholar.google.co.in/citations?user=gjslbzsAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Ayan Kumar Bhunia</a>
    </figcaption>
</figure>
<figure id="attachment_906" aria-describedby="caption-attachment-906" style="width: 150px" class="wp-caption alignleft">
    <a href="https://rowl1ng.com">
        <img loading="lazy" decoding="async" class="wp-image-906" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/0b4b78d024da3b6046badb8759e0ce5c.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-906" class="wp-caption-text">
        <a href="https://rowl1ng.com" target="_blank" rel="noopener noreferrer">Ling Luo</a>
    </figcaption>
</figure>
<figure id="attachment_907" aria-describedby="caption-attachment-907" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=x-WI_EgAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-907" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/lori-hoy.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-907" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=x-WI_EgAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Ayan Das</a>
    </figcaption>
</figure>
<figure id="attachment_904" aria-describedby="caption-attachment-904" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=_QWFBvoAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-904" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/8a3814d35e046cda138f04bfebe203c1.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-904" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=_QWFBvoAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Aneeshan Sain</a>
    </figcaption>
</figure>
<figure id="attachment_1003" aria-describedby="caption-attachment-1003" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-1003" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/f15a56e40cdad561f1b57188b9664369.jpg" alt="" width="150" height="200">
    <figcaption id="caption-attachment-1003" class="wp-caption-text">Zhiyu Qu</figcaption>
</figure>
<figure id="attachment_904" aria-describedby="caption-attachment-904" style="width: 150px" class="wp-caption alignleft">
    <a href="http://pinakinathc.me">
        <img loading="lazy" decoding="async" class="wp-image-904" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/IMG_00631.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-904" class="wp-caption-text">
        <a href="http://pinakinathc.me" target="_blank" rel="noopener noreferrer">Pinaki Chowdhury</a>
    </figcaption>
</figure>
<figure id="attachment_1003" aria-describedby="caption-attachment-1003" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-1003" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/self-photo-225x300.jpg" alt="" width="150" height="200">
    <figcaption id="caption-attachment-1003" class="wp-caption-text">Yixiao Zheng</figcaption>
</figure>
<figure id="attachment_1002" aria-describedby="caption-attachment-1002" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-1002" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2021/04/mmexport1619692839658_mh1619693201290.jpg" alt="" width="150" height="200">
    <figcaption id="caption-attachment-1002" class="wp-caption-text">Ruolin Yang</figcaption>
</figure>
<figure id="attachment_904" aria-describedby="caption-attachment-904" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=-mOrpz8AAAAJ">
        <img loading="lazy" decoding="async" class="wp-image-904" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/04/sk02100.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-904" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=-mOrpz8AAAAJ" target="_blank" rel="noopener noreferrer">Subhadeep Koley</a>
    </figcaption>
</figure>
<figure id="attachment_904" aria-describedby="caption-attachment-904" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.in/citations?hl=en&amp;user=aBturOYAAAAJ&amp;view_op=list_works&amp;sortby=pubdate">
        <img loading="lazy" decoding="async" class="wp-image-904" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/IMG_20220710_021548.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-904" class="wp-caption-text">
        <a href="https://scholar.google.co.in/citations?hl=en&amp;user=aBturOYAAAAJ&amp;view_op=list_works&amp;sortby=pubdate" target="_blank" rel="noopener noreferrer">Hmrishav Bandyopadhyay</a>
    </figcaption>
</figure>
<figure id="attachment_1003" aria-describedby="caption-attachment-1003" style="width: 150px" class="wp-caption alignleft">
    <img loading="lazy" decoding="async" class="wp-image-1003" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/08/Me.jpg" alt="" width="150" height="200">
    <figcaption id="caption-attachment-1003" class="wp-caption-text">Alexander Ashcroft</figcaption>
</figure>
<figure id="attachment_904" aria-describedby="caption-attachment-904" style="width: 150px" class="wp-caption alignleft">
    <a href="https://ruoyidu.github.io">
        <img loading="lazy" decoding="async" class="wp-image-904" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/08/RuoyiDu.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-904" class="wp-caption-text">
        <a href="https://ruoyidu.github.io" target="_blank" rel="noopener noreferrer">Ruoyi Du</a>
    </figcaption>
</figure>

<h3>Past PhD Students:</h3>
<figure id="attachment_874" aria-describedby="caption-attachment-874" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=1D4xX8MAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-874" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2022/07/68b794403df3fd57f5f87670afed023f.jpg" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-874" class="wp-caption-text">
        <a href="https://anranqi.github.io/" target="_blank" rel="noopener noreferrer">Anran Qi</a>
        <p style="font-size: small" align="center">(now Postdoc at University of Tokyo)</p>
    </figcaption>
</figure>
<figure id="attachment_874" aria-describedby="caption-attachment-874" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=1D4xX8MAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-874" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/11-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-874" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=1D4xX8MAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Conghui Hu</a>
        <p style="font-size: small" align="center">(now Postdoc at National University of Singapore)</p>
    </figcaption>
</figure>
<figure id="attachment_874" aria-describedby="caption-attachment-874" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.co.uk/citations?user=aRBLzfEAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-874" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/9-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-874" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=aRBLzfEAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Umar Riaz Muhammad</a>
        <p style="font-size: small" align="center">(now Senior AI Developer at Huawei UK)</p>
    </figcaption>
</figure>
<figure id="attachment_877" aria-describedby="caption-attachment-877" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=9a1PjCIAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-877" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/12-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-877" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=9a1PjCIAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Jifei Song</a>
        <p style="font-size: small" align="center">(now Senior Research Scientist at Huawei UK)</p>
    </figcaption>
</figure>
<figure id="attachment_875" aria-describedby="caption-attachment-875" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=RPvaE3oAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-875" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/10-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-875" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=RPvaE3oAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Da Li</a>
        <p style="font-size: small" align="center">(now Research Scientist at Samsung AI UK)</p>
    </figcaption>
</figure>
<figure id="attachment_880" aria-describedby="caption-attachment-880" style="width: 150px" class="wp-caption alignleft">
    <a href="https://scholar.google.com/citations?user=mmm90qgAAAAJ&amp;hl=en">
        <img loading="lazy" decoding="async" class="wp-image-880" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/15-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-880" class="wp-caption-text">
        <a href="https://scholar.google.com/citations?user=mmm90qgAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Qian Yu</a>
        <p style="font-size: small" align="center">(now Associate Professor at Beihang University)</p>
    </figcaption>
</figure>
<figure id="attachment_881" aria-describedby="caption-attachment-881" style="width: 150px" class="wp-caption alignleft">
    <a href="https://qugank.github.io">
        <img loading="lazy" decoding="async" class="wp-image-881" src="http://sketchx.eecs.qmul.ac.uk/wp-content/uploads/sites/27/2020/10/17-225x300.png" alt="" width="150" height="200">
    </a>
    <figcaption id="caption-attachment-881" class="wp-caption-text">
        <a href="https://scholar.google.co.uk/citations?user=SeEfMBkAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Yi Li</a>
        <p style="font-size: small" align="center">(now Senior Research Scientist at JD.com</p>
    </figcaption>
</figure>

<h3>Visitors (Past & Present):</h3>
<p>
    <a href="https://scholar.google.com/citations?user=9yg80qYAAAAJ&amp;hl=zh-CN" target="_blank" rel="noopener noreferrer">Jianshu Zhang</a>, University of Science and Technology of China/iFlyTek.
</p>
<p>
    <a href="https://scholar.google.es/citations?user=ZyjQEiwAAAAJ&amp;hl=en" target="_blank" rel="noopener noreferrer">Sounak Dey</a>, Computer Vision Center, Universitat Autònoma de Barcelona.
</p>
<p>
    <a href="https://scholar.google.com/citations?user=o_DllmIAAAAJ&amp;hl=zh-CN" target="_blank" rel="noopener noreferrer">Yaowei Wang</a>, Peking University Shenzhen Graduate School.
</p>

</div>
</div>



<!-- Section: Publications -->
<div class="section" id="publications-section" >
  <h2>📝 Team Publications</h2>
  <!-- 2025 年论文列表 -->
<h3>📚 2025</h3>
<ol style="padding-left: 1.2em;">
  
  <li style="margin-bottom: 0.4em; line-height: 1.4;">
    <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32240" target="_blank" rel="noopener noreferrer">
      <strong>VersaGen: Unleashing Versatile Visual Control for Text-to-Image Synthesis</strong>
    </a>
    , Zhipeng Chen, Lan Yang, Yonggang Qi, Honggang Zhang, Kaiyue Pang, Ke Li, Yi-Zhe Song, <em>AAAI</em>
  </li>
</ol>
<h3>📚 2024</h3>
<ol style="padding-left: 1.2em;">
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Du_DemoFusion_Democratising_High-Resolution_Image_Generation_With_No__CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Demofusion: Democratising high-resolution image generation with no $$$
   </strong>
  </a>
  , Ruoyi Du, Dongliang Chang, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Its_All_About_Your_Sketch_Democratising_Sketch_Control_in_Diffusion_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    It's All About Your Sketch: Democratising Sketch Control in Diffusion Models
   </strong>
  </a>
  , Subhadeep Koley, Ayan Kumar Bhunia, Deeptanshu Sekhri, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_How_to_Handle_Sketch-Abstraction_in_Sketch-Based_Image_Retrieval_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    How to handle sketch-abstraction in sketch-based image retrieval?
   </strong>
  </a>
  , Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Youll_Never_Walk_Alone_A_Sketch_and_Text_Duet_for_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    You'll Never Walk Alone: A Sketch and Text Duet for Fine-Grained Image Retrieval
   </strong>
  </a>
  , Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_Doodle_Your_3D_From_Abstract_Freehand_Sketches_to_Precise_3D_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Doodle your 3d: From abstract freehand sketches to precise 3d shapes
   </strong>
  </a>
  , Hmrishav Bandyopadhyay, Subhadeep Koley, Ayan Das, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_SketchINR_A_First_Look_into_Sketches_as_Implicit_Neural_Representations_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchinr: A first look into sketches as implicit neural representations
   </strong>
  </a>
  , Hmrishav Bandyopadhyay, Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Tao Xiang, Timothy Hospedales, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Koley_Text-to-Image_Diffusion_Models_are_Great_Sketch-Photo_Matchmakers_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Text-to-image diffusion models are great sketch-photo matchmakers
   </strong>
  </a>
  , Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10472065/" rel="noopener noreferrer" target="_blank">
   <strong>
    Bi-directional ensemble feature reconstruction network for few-shot fine-grained classification
   </strong>
  </a>
  , Jijie Wu, Dongliang Chang, Aneeshan Sain, Xiaoxu Li, Zhanyu Ma, Jie Cao, Jun Guo, Yi-Zhe Song,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Qu_Wired_Perspectives_Multi-View_Wire_Art_Embraces_Generative_AI_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Wired perspectives: Multi-view wire art embraces generative ai
   </strong>
  </a>
  , Zhiyu Qu, Lan Yang, Honggang Zhang, Tao Xiang, Kaiyue Pang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Chen_DemoCaricature_Democratising_Caricature_Generation_with_a_Rough_Sketch_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Democaricature: Democratising caricature generation with a rough sketch
   </strong>
  </a>
  , Dar-Yen Chen, Ayan Kumar Bhunia, Subhadeep Koley, Aneeshan Sain, Pinaki Nath Chowdhury, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-72673-6_23" rel="noopener noreferrer" target="_blank">
   <strong>
    PartCraft: Crafting Creative Objects by Parts
   </strong>
  </a>
  , Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10471272/" rel="noopener noreferrer" target="_blank">
   <strong>
    Creativeseg: Semantic segmentation of creative sketches
   </strong>
  </a>
  , Yixiao Zheng, Kaiyue Pang, Ayan Das, Dongliang Chang, Yi-Zhe Song, Zhanyu Ma,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2405.18716" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchdeco: Decorating b&amp;w sketches with colour
   </strong>
  </a>
  , Chaitat Utintu, Pinaki Nath Chowdhury, Aneeshan Sain, Subhadeep Koley, Ayan Kumar Bhunia, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2024/html/Bandyopadhyay_What_Sketch_Explainability_Really_Means_for_Downstream_Tasks_CVPR_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    What Sketch Explainability Really Means for Downstream Tasks?
   </strong>
  </a>
  , Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=O2jyuo89CK" rel="noopener noreferrer" target="_blank">
   <strong>
    Modelling complex vector drawings with stroke-clouds
   </strong>
  </a>
  , Alexander Ashcroft, Ayan Das, Yulia Gryaditskaya, Zhiyu Qu, Yi-Zhe Song,
  <em>
   ICLR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openaccess.thecvf.com/content/CVPR2024W/FGVC11/html/Ng_ConceptHash_Interpretable_Fine-Grained_Hashing_via_Concept_Discovery_CVPRW_2024_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    ConceptHash: Interpretable Fine-Grained Hashing via Concept Discovery
   </strong>
  </a>
  , Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=nQsimt9atc" rel="noopener noreferrer" target="_blank">
   <strong>
    Ipr-nerf: Ownership verification meets neural radiance field
   </strong>
  </a>
  , Win Kent Ong, Kam Woh Ng, Chee Seng Chan, Yi-Zhe Song, Tao Xiang,
  <em>
   ICLR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-72992-8_13" rel="noopener noreferrer" target="_blank">
   <strong>
    Do Generalised Classifiers Really Work on Human Drawn Sketches?
   </strong>
  </a>
  , Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Ayan Kumar Bhunia, Yi-Zhe Song,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=5xadJmgwix" rel="noopener noreferrer" target="_blank">
   <strong>
    Scale-Adaptive Diffusion Model for Complex Sketch Synthesis
   </strong>
  </a>
  , Jijin Hu, Ke Li, Yonggang Qi, Yi-Zhe Song,
  <em>
   ICLR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=5xadJmgwix" rel="noopener noreferrer" target="_blank">
   <strong>
    Scale-Adaptive Diffusion Model for Complex Sketch Synthesis
   </strong>
  </a>
  , Jijin Hu, Ke Li, Yonggang Qi, Yi-Zhe Song,
  <em>
   ICLR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-72998-0_9" rel="noopener noreferrer" target="_blank">
   <strong>
    Freeview Sketching: View-Aware Fine-Grained Sketch-Based Image Retrieval
   </strong>
  </a>
  , Aneeshan Sain, Pinaki Nath Chowdhury, Subhadeep Koley, Ayan Kumar Bhunia, Yi-Zhe Song,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10707331/" rel="noopener noreferrer" target="_blank">
   <strong>
    Understanding Episode Hardness in Few-Shot Learning
   </strong>
  </a>
  , Yurong Guo, Ruoyi Du, Aneeshan Sain, Kongming Liang, Yuan Dong, Yi-Zhe Song, Zhanyu Ma,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/article/10.1007/s11263-024-02001-1" rel="noopener noreferrer" target="_blank">
   <strong>
    Annotation-Free Human Sketch Quality Assessment
   </strong>
  </a>
  , Lan Yang, Kaiyue Pang, Honggang Zhang, Yi-Zhe Song,
  <em>
   IJCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10589301/" rel="noopener noreferrer" target="_blank">
   <strong>
    3D Reconstruction From a Single Sketch via View-Dependent Depth Sampling
   </strong>
  </a>
  , Chenjian Gao, Xilin Wang, Qian Yu, Lu Sheng, Jing Zhang, Xiaoguang Han, Yi-Zhe Song, Dong Xu,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-72353-7_14" rel="noopener noreferrer" target="_blank">
   <strong>
    Advancing Free-Breathing Cardiac Cine MRI: Retrospective Respiratory Motion Correction Via Kspace-and-Image Guided Diffusion Model
   </strong>
  </a>
  , Hongming Guo, Ziqing Huang, Qian Yuan, Hanbo Song, Zhiyan Liu, Xianzhao Feng, Anqi Liu, Min Liu, Ke Li, Ruixi Zhou,
  <em>
   ICANN
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-78347-0_3" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch2Seg: Sketch-Based Image Segmentation with Pre-trained Diffusion Model
   </strong>
  </a>
  , Xin Dai, Haoge Deng, Ke Li, Yonggang Qi,
  <em>
   ICANN
  </em>
 </li>
</ol>

<h3>📚 2023</h3>
<ol style="padding-left: 1.2em;">
   <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Sain_CLIP_for_All_Things_Zero-Shot_Sketch-Based_Image_Retrieval_Fine-Grained_or_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Clip for all things zero-shot sketch-based image retrieval, fine-grained or not
   </strong>
  </a>
  , Aneeshan Sain, Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Subhadeep Koley, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ojs.aaai.org/index.php/AAAI/article/view/25383" rel="noopener noreferrer" target="_blank">
   <strong>
    Bi-directional feature reconstruction network for fine-grained few-shot image classification
   </strong>
  </a>
  , Jijie Wu, Dongliang Chang, Aneeshan Sain, Xiaoxu Li, Zhanyu Ma, Jie Cao, Jun Guo, Yi-Zhe Song,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://proceedings.neurips.cc/paper_files/paper/2023/hash/0fb98d483fa580e0354bcdd3a003a3f3-Abstract-Conference.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Headsculpt: Crafting 3d head avatars with text
   </strong>
  </a>
  , Xiao Han, Yukang Cao, Kai Han, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang, Kwan-Yee K Wong,
  <em>
   NeurIPS
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Koley_Picture_That_Sketch_Photorealistic_Image_Generation_From_Abstract_Sketches_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Picture that sketch: Photorealistic image generation from abstract sketches
   </strong>
  </a>
  , Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Lin_Zero-Shot_Everything_Sketch-Based_Image_Retrieval_and_in_Explainable_Style_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Zero-shot everything sketch-based image retrieval, and in explainable style
   </strong>
  </a>
  , Fengyin Lin, Mingkang Li, Da Li, Timothy Hospedales, Yi-Zhe Song, Yonggang Qi,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Nag_DiffTAD_Temporal_Action_Detection_with_Proposal_Denoising_Diffusion_ICCV_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Difftad: Temporal action detection with proposal denoising diffusion
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Han_FAME-ViL_Multi-Tasking_Vision-Language_Model_for_Heterogeneous_Fashion_Tasks_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Fame-vil: Multi-tasking vision-language model for heterogeneous fashion tasks
   </strong>
  </a>
  , Xiao Han, Xiatian Zhu, Licheng Yu, Li Zhang, Yi-Zhe Song, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chowdhury_SceneTrilogy_On_Human_Scene-Sketch_and_Its_Complementarity_With_Photo_and_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Scenetrilogy: On human scene-sketch and its complementarity with photo and text
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=4eJ43EN2g6l" rel="noopener noreferrer" target="_blank">
   <strong>
    SketchKnitter: Vectorized Sketch Generation with Diffusion Models
   </strong>
  </a>
  , Qiang Wang, Haoge Deng, Yonggang Qi, Da Li, Yi-Zhe Song,
  <em>
   ICLR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Han_Controllable_Person_Image_Synthesis_with_Pose-Constrained_Latent_Diffusion_ICCV_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Controllable person image synthesis with pose-constrained latent diffusion
   </strong>
  </a>
  , Xiao Han, Xiatian Zhu, Jiankang Deng, Yi-Zhe Song, Tao Xiang,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10145054/" rel="noopener noreferrer" target="_blank">
   <strong>
    Prediction calibration for generalized few-shot semantic segmentation
   </strong>
  </a>
  , Zhihe Lu, Sen He, Da Li, Yi-Zhe Song, Tao Xiang,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Sain_Exploiting_Unlabelled_Photos_for_Stronger_Fine-Grained_SBIR_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Exploiting unlabelled photos for stronger fine-grained SBIR
   </strong>
  </a>
  , Aneeshan Sain, Ayan Kumar Bhunia, Subhadeep Koley, Pinaki Nath Chowdhury, Soumitri Chattopadhyay, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Bhunia_Sketch2Saliency_Learning_To_Detect_Salient_Objects_From_Human_Drawings_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch2saliency: Learning to detect salient objects from human drawings
   </strong>
  </a>
  , Ayan Kumar Bhunia, Subhadeep Koley, Amandeep Kumar, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chaudhuri_Data-Free_Sketch-Based_Image_Retrieval_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Data-free sketch-based image retrieval
   </strong>
  </a>
  , Abhra Chaudhuri, Ayan Kumar Bhunia, Yi-Zhe Song, Anjan Dutta,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10189399/" rel="noopener noreferrer" target="_blank">
   <strong>
    Uncertainty-aware source-free domain adaptive semantic segmentation
   </strong>
  </a>
  , Zhihe Lu, Da Li, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Chang_An_Erudite_Fine-Grained_Visual_Classification_Model_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    An erudite fine-grained visual classification model
   </strong>
  </a>
  , Dongliang Chang, Yujun Tong, Ruoyi Du, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Guo_Task-aware_Adaptive_Learning_for_Cross-domain_Few-shot_Learning_ICCV_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Task-aware adaptive learning for cross-domain few-shot learning
   </strong>
  </a>
  , Yurong Guo, Ruoyi Du, Yuan Dong, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Du_On-the-Fly_Category_Discovery_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    On-the-fly category discovery
   </strong>
  </a>
  , Ruoyi Du, Dongliang Chang, Kongming Liang, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2304.03785" rel="noopener noreferrer" target="_blank">
   <strong>
    ChiroDiff: Modelling chirographic data with Diffusion Models
   </strong>
  </a>
  , Ayan Das, Yongxin Yang, Timothy Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Luo_3D_VR_Sketch_Guided_3D_Shape_Prototyping_and_Exploration_ICCV_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    3d vr sketch guided 3d shape prototyping and exploration
   </strong>
  </a>
  , Ling Luo, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, Yulia Gryaditskaya,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10214525/" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-segformer: Transformer-based segmentation for figurative and creative sketches
   </strong>
  </a>
  , Yixiao Zheng, Jiyang Xie, Aneeshan Sain, Yi-Zhe Song, Zhanyu Ma,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Nag_Post-Processing_Temporal_Action_Detection_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Post-processing temporal action detection
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10122150/" rel="noopener noreferrer" target="_blank">
   <strong>
    Making a bird ai expert work for you and me
   </strong>
  </a>
  , Dongliang Chang, Kaiyue Pang, Ruoyi Du, Yujun Tong, Yi-Zhe Song, Zhanyu Ma, Jun Guo,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Qu_SketchXAI_A_First_Look_at_Explainability_for_Human_Sketches_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchxai: A first look at explainability for human sketches
   </strong>
  </a>
  , Zhiyu Qu, Yulia Gryaditskaya, Ke Li, Kaiyue Pang, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2308.14191" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchdreamer: Interactive text-augmented creative sketch ideation
   </strong>
  </a>
  , Zhiyu Qu, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Qu_SketchXAI_A_First_Look_at_Explainability_for_Human_Sketches_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchxai: A first look at explainability for human sketches
   </strong>
  </a>
  , Zhiyu Qu, Yulia Gryaditskaya, Ke Li, Kaiyue Pang, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10292696/" rel="noopener noreferrer" target="_blank">
   <strong>
    Mind the Gap: Open Set Domain Adaptation via Mutual-to-Separate Framework
   </strong>
  </a>
  , Dongliang Chang, Aneeshan Sain, Zhanyu Ma, Yi-Zhe Song, Ruiping Wang, Jun Guo,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2023/html/Chowdhury_Democratising_2D_Sketch_to_3D_Shape_Retrieval_Through_Pivoting_ICCV_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Democratising 2D sketch to 3D shape retrieval through pivoting
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2302.07669" rel="noopener noreferrer" target="_blank">
   <strong>
    Unsupervised hashing with similarity distribution calibration
   </strong>
  </a>
  , Kam Woh Ng, Xiatian Zhu, Jiun Tian Hoe, Chee Seng Chan, Tianyu Zhang, Yi-Zhe Song, Tao Xiang,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10273439/" rel="noopener noreferrer" target="_blank">
   <strong>
    Semi-supervised learning for FGVC with out-of-category data
   </strong>
  </a>
  , Ruoyi Du, Dongliang Chang, Zhanyu Ma, Kongming Liang, Yi-Zhe Song, Jun Guo,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2311.07261" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-based video object segmentation: benchmark and analysis
   </strong>
  </a>
  , Ruolin Yang, Da Li, Conghui Hu, Timothy Hospedales, Honggang Zhang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openresearch.surrey.ac.uk/esploro/outputs/doctoral/SceneTrilogy-On-Scene-Sketches-and-its/99958466602346" rel="noopener noreferrer" target="_blank">
   <strong>
    SceneTrilogy: on scene sketches and its relationship with text and photo
   </strong>
  </a>
  , Pinaki Nath Chowdhury,
  <em>
   PhD
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Li_Photo_Pre-Training_but_for_Sketch_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Photo Pre-Training, But for Sketch
   </strong>
  </a>
  , , Ke Li, Kaiyue Pang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2023/html/Li_Photo_Pre-Training_but_for_Sketch_CVPR_2023_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Photo Pre-Training, But for Sketch
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2303.05734" rel="noopener noreferrer" target="_blank">
   <strong>
    Generative Model Based Noise Robust Training for Unsupervised Domain Adaptation
   </strong>
  </a>
  , Zhongying Deng, Da Li, Junjun He, Yi-Zhe Song, Tao Xiang,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv230315149N/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    What Can Human Sketches Do for Object Detection?
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2023arXiv231115477W/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    DreamCreature: Crafting Photorealistic Virtual Creatures from Imagination
   </strong>
  </a>
  , Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openaccess.thecvf.com/content/CVPR2023/supplemental/Li_Photo_Pre-Training_but_CVPR_2023_supplemental.pdf" rel="noopener noreferrer" target="_blank">
   <strong>
    Supplementary material: Photo Pre-Training, But for Sketch
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, CVSSP SketchX,
  <em>
   CVPR
  </em>
 </li>

</ol>

<h3>📚 2022</h3>
<ol style="padding-left: 1.2em;">
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9706366/" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep learning for free-hand sketch: A survey
   </strong>
  </a>
  , Peng Xu, Timothy M Hospedales, Qiyue Yin, Yi-Zhe Song, Tao Xiang, Liang Wang,
  <em>
   TNNLS
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022/html/He_Style-Based_Global_Appearance_Flow_for_Virtual_Try-On_CVPR_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Style-based global appearance flow for virtual try-on
   </strong>
  </a>
  , Sen He, Yi-Zhe Song, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_39" rel="noopener noreferrer" target="_blank">
   <strong>
    Zero-shot temporal action detection via vision-language prompting
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ojs.aaai.org/index.php/AAAI/article/view/20226" rel="noopener noreferrer" target="_blank">
   <strong>
    Hybrid graph neural networks for few-shot learning
   </strong>
  </a>
  , Tianyuan Yu, Sen He, Yi-Zhe Song, Tao Xiang,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Bhunia_Sketching_Without_Worrying_Noise-Tolerant_Sketch-Based_Image_Retrieval_CVPR_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketching without worrying: Noise-tolerant sketch-based image retrieval
   </strong>
  </a>
  , Ayan Kumar Bhunia, Subhadeep Koley, Abdullah Faiz Ur Rahman Khilji, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_37" rel="noopener noreferrer" target="_blank">
   <strong>
    Proposal-free temporal action detection via global segmentation mask learning
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Yi-Zhe Song, Tao Xiang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Sain_Sketch3T_Test-Time_Training_for_Zero-Shot_SBIR_CVPR_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch3t: Test-time training for zero-shot sbir
   </strong>
  </a>
  , Aneeshan Sain, Ayan Kumar Bhunia, Vaishnav Potlapalli, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-19833-5_37" rel="noopener noreferrer" target="_blank">
   <strong>
    Fashionvil: Fashion-focused vision-and-language representation learning
   </strong>
  </a>
  , Xiao Han, Licheng Yu, Xiatian Zhu, Li Zhang, Yi-Zhe Song, Tao Xiang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9813442/" rel="noopener noreferrer" target="_blank">
   <strong>
    Dynamic instance domain adaptation
   </strong>
  </a>
  , Zhongying Deng, Kaiyang Zhou, Da Li, Junjun He, Yi-Zhe Song, Tao Xiang,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Bhunia_Doodle_It_Yourself_Class_Incremental_Learning_by_Drawing_a_Few_CVPR_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Doodle it yourself: Class incremental learning by drawing a few sketches
   </strong>
  </a>
  , Ayan Kumar Bhunia, Viswanatha Reddy Gajjala, Subhadeep Koley, Rohit Kundu, Aneeshan Sain, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-19836-6_10" rel="noopener noreferrer" target="_blank">
   <strong>
    Adaptive fine‑grained sketch‑based image retrieval
   </strong>
  </a>
  , Ayan Kumar Bhunia, Aneeshan Sain, Parth Hiren Shah, Animesh Gupta, Pinaki Nath Chowdhury, Tao Xiang, Yi‑Zhe Song,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-20062-5_38" rel="noopener noreferrer" target="_blank">
   <strong>
    Semi‑supervised temporal action detection with proposal‑free masking
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Yi‑Zhe Song, Tao Xiang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-031-19769-7_27" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchsampler: Sketch‑based 3d reconstruction via view‑dependent depth sampling
   </strong>
  </a>
  , Chenjian Gao, Qian Yu, Lu Sheng, Yi‑Zhe Song, Dong Xu,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9739995/" rel="noopener noreferrer" target="_blank">
   <strong>
    One sketch for all: One‑shot personalized sketch segmentation
   </strong>
  </a>
  , Anran Qi, Yulia Gryaditskaya, Tao Xiang, Yi‑Zhe Song,
  <em>
   ArXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.research.ed.ac.uk/en/publications/sketchode-learning-neural-sketch-representation-in-continuous-tim" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchode: Learning neural sketch representation in continuous time
   </strong>
  </a>
  , Ayan Das, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song,
  <em>
   ArXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9686584/" rel="noopener noreferrer" target="_blank">
   <strong>
    Exploring local detail perception for scene sketch semantic segmentation
   </strong>
  </a>
  , Ce Ge, Haifeng Sun, Yi‑Zhe Song, Zhanyu Ma, Jianxin Liao,
  <em>
   ArXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/3550454.3555493" rel="noopener noreferrer" target="_blank">
   <strong>
    Differsketching: How differently do people sketch 3d objects?
   </strong>
  </a>
  , Chufeng Xiao, Wanchao Su, Jing Liao, Zhouhui Lian, Yi‑Zhe Song, Hongbo Fu,
  <em>
   TOG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/article/10.1007/s11263-022-01623-7" rel="noopener noreferrer" target="_blank">
   <strong>
    Generative sketch healing
   </strong>
  </a>
  , Yonggang Qi, Guoyao Su, Qiang Wang, Jie Yang, Kaiyue Pang, Yi‑Zhe Song,
  <em>
   IJCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/10044450/" rel="noopener noreferrer" target="_blank">
   <strong>
    Structure‑aware 3d vr sketch to 3d shape retrieval
   </strong>
  </a>
  , Ling Luo, Yulia Gryaditskaya, Tao Xiang, Yi‑Zhe Song,
  <em>
   3DV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0097849322001078" rel="noopener noreferrer" target="_blank">
   <strong>
    A study of deep single sketch‑based modeling: View/style invariance, sparsity and latent space disentanglement
   </strong>
  </a>
  , Yue Zhong, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2210.01676" rel="noopener noreferrer" target="_blank">
   <strong>
    Robust target training for multi‑source domain adaptation
   </strong>
  </a>
  , Zhongying Deng, Da Li, Yi‑Zhe Song, Tao Xiang,
  <em>
   ArXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022W/CVFAD/html/Han_UIGR_Unified_Interactive_Garment_Retrieval_CVPRW_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Uigr: Unified interactive garment retrieval
   </strong>
  </a>
  , Xiao Han, Sen He, Li Zhang, Yi‑Zhe Song, Tao Xiang,
  <em>
   CVPRW
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2022/html/Yang_Finding_Badly_Drawn_Bunnies_CVPR_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Finding badly drawn bunnies
   </strong>
  </a>
  , Lan Yang, Kaiyue Pang, Honggang Zhang, Yi‑Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2211.10715" rel="noopener noreferrer" target="_blank">
   <strong>
    Single stage multi‑pose virtual try-on
   </strong>
  </a>
  , Sen He, Yi‑Zhe Song, Tao Xiang,
  <em>
   ArXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2211.14905" rel="noopener noreferrer" target="_blank">
   <strong>
    Multi-Modal Few-Shot Temporal Action Detection
   </strong>
  </a>
  , Sauradip Nag, Mengmeng Xu, Xiao Han, Xiatian Zhu, Bernard Ghanem, Yi-Zhe Song, Tao Xiang,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2210.14271" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning to Augment via Implicit Differentiation for Domain Generalization
   </strong>
  </a>
  , Tingwei Wang, Da Li, Kaiyang Zhou, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openaccess.thecvf.com/content/CVPR2022W/L3D-IVU/html/Xiang_CDAD_A_Common_Daily_Action_Dataset_With_Collected_Hard_Negative_CVPRW_2022_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    CDAD: A Common Daily Action Dataset with Collected Hard Negative Samples
   </strong>
  </a>
  , Wangmeng Xiang, Chao Li, Ke Li, Biao Wang, Xian-sheng Hua, Lei Zhang,
  <em>
   CVPRW
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220411964N/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    SceneTrilogy: On Human Scene-Sketch and its Complementarity with Photo and Text
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2209.10020" rel="noopener noreferrer" target="_blank">
   <strong>
    Towards 3D VR-Sketch to 3D Shape Retrieval
   </strong>
  </a>
  , Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220314804N/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    Partially Does It: Towards Scene-Level FG-SBIR with Partial Input
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Viswanatha Reddy Gajjala, Aneeshan Sain, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2022arXiv220302113N/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    FS-COCO: Towards Understanding of Freehand Sketches of Common Objects in Context
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Aneeshan Sain, Ayan Kumar Bhunia, Tao Xiang, Yulia Gryaditskaya, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.pinakinathc.me/assets/papers/3DV_2022_supp.pdf" rel="noopener noreferrer" target="_blank">
   <strong>
    Garment Ideation: Iterative View-Aware Sketch-Based Garment Modeling Supplemental
   </strong>
  </a>
  , Pinaki Nath Chowdhury, Tuanfeng Wang, Duygu Ceylan, Yi-Zhe Song, Yulia Gryaditskaya,
  <em>
   3DV
  </em>
 </li>
</ol>


<h3>📚 2021</h3>
<ol style="padding-left: 1.2em;">
  
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9609630/" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained image analysis with deep learning: A survey
   </strong>
  </a>
  , Xiu-Shen Wei, Yi-Zhe Song, Oisin Mac Aodha, Jianxin Wu, Yuxin Peng, Jinhui Tang, Jian Yang, Serge Belongie,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Lu_Simpler_Is_Better_Few-Shot_Semantic_Segmentation_With_Classifier_Weight_Transformer_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Simpler is better: Few-shot semantic segmentation with classifier weight transformer
   </strong>
  </a>
  , Zhihe Lu, Sen He, Xiatian Zhu, Li Zhang, Yi-Zhe Song, Tao Xiang,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Chang_Your_Flamingo_is_My_Bird_Fine-Grained_or_Not_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Your "Flamingo" is My "Bird": Fine-Grained, or Not
   </strong>
  </a>
  , Dongliang Chang, Kaiyue Pang, Yixiao Zheng, Zhanyu Ma, Yi-Zhe Song, Jun Guo,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Sain_StyleMeUp_Towards_Style-Agnostic_Sketch-Based_Image_Retrieval_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Stylemeup: Towards style-agnostic sketch-based image retrieval
   </strong>
  </a>
  , Aneeshan Sain, Ayan Kumar Bhunia, Yongxin Yang, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9609669/" rel="noopener noreferrer" target="_blank">
   <strong>
    Progressive learning of category-consistent multi-granularity features for fine-grained visual classification
   </strong>
  </a>
  , Ruoyi Du, Jiyang Xie, Zhanyu Ma, Dongliang Chang, Yi-Zhe Song, Jun Guo,
  <em>
   TPAMI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_More_Photos_Are_All_You_Need_Semi-Supervised_Learning_for_Fine-Grained_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    More photos are all you need: Semi-supervised learning for fine-grained sketch based image retrieval
   </strong>
  </a>
  , Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Yongxin Yang, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Joint_Visual_Semantic_Reasoning_Multi-Stage_Decoder_for_Text_Recognition_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Joint visual semantic reasoning: Multi-stage decoder for text recognition
   </strong>
  </a>
  , Ayan Kumar Bhunia, Aneeshan Sain, Amandeep Kumar, Shuvozit Ghose, Pinaki Nath Chowdhury, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_Vectorization_and_Rasterization_Self-Supervised_Learning_for_Sketch_and_Handwriting_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Vectorization and rasterization: Self-supervised learning for sketch and handwriting
   </strong>
  </a>
  , Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/He_Context-Aware_Layout_to_Image_Generation_With_Enhanced_Object_Appearance_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Context-aware layout to image generation with enhanced object appearance
   </strong>
  </a>
  , Sen He, Wentong Liao, Michael Ying Yang, Yongxin Yang, Yi-Zhe Song, Bodo Rosenhahn, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Chen_Variational_Attention_Propagating_Domain-Specific_Knowledge_for_Multi-Domain_Learning_in_Crowd_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Variational attention: Propagating domain-specific knowledge for multi-domain learning in crowd counting
   </strong>
  </a>
  , Binghui Chen, Zhaoyi Yan, Ke Li, Pengyu Li, Biao Wang, Wangmeng Zuo, Lei Zhang,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/article/10.1007/s11263-020-01382-3" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained instance-level sketch-based image retrieval
   </strong>
  </a>
  , Qian Yu, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   IJCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9573376/" rel="noopener noreferrer" target="_blank">
   <strong>
    Toward fine-grained sketch-based 3D shape retrieval
   </strong>
  </a>
  , Anran Qi, Yulia Gryaditskaya, Jifei Song, Yongxin Yang, Yonggang Qi, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Bhunia_MetaHTR_Towards_Writer-Adaptive_Handwritten_Text_Recognition_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Metahtr: Towards writer-adaptive handwritten text recognition
   </strong>
  </a>
  , Ayan Kumar Bhunia, Shuvozit Ghose, Amandeep Kumar, Pinaki Nath Chowdhury, Aneeshan Sain, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Das_Cloud2Curve_Generation_and_Vectorization_of_Parametric_Sketches_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Cloud2curve: Generation and vectorization of parametric sketches
   </strong>
  </a>
  , Ayan Das, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/He_Disentangled_Lifespan_Face_Synthesis_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Disentangled lifespan face synthesis
   </strong>
  </a>
  , Sen He, Wentong Liao, Michael Ying Yang, Yi-Zhe Song, Bodo Rosenhahn, Tao Xiang,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Text_Is_Text_No_Matter_What_Unifying_Text_Recognition_Using_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Text is text, no matter what: Unifying text recognition using knowledge distillation
   </strong>
  </a>
  , Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Yang_SketchAA_Abstract_Representation_for_Abstract_Sketches_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchaa: Abstract representation for abstract sketches
   </strong>
  </a>
  , Lan Yang, Kaiyue Pang, Honggang Zhang, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Qi_SketchLattice_Latticed_Representation_for_Sketch_Manipulation_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchlattice: Latticed representation for sketch manipulation
   </strong>
  </a>
  , Yonggang Qi, Guoyao Su, Pinaki Nath Chowdhury, Mingkang Li, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/ICCV2021/html/Bhunia_Towards_the_Unseen_Iterative_Text_Recognition_by_Distilling_From_Errors_ICCV_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Towards the unseen: Iterative text recognition by distilling from errors
   </strong>
  </a>
  , Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Yi-Zhe Song,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9665875/" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained vr sketching: Dataset and insights
   </strong>
  </a>
  , Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi-Zhe Song,
  <em>
   3DV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content/CVPR2021/html/Qi_PQA_Perceptual_Question_Answering_CVPR_2021_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Pqa: Perceptual question answering
   </strong>
  </a>
  , Yonggang Qi, Kai Zhang, Aneeshan Sain, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2105.08237" rel="noopener noreferrer" target="_blank">
   <strong>
    Towards unsupervised sketch-based image retrieval
   </strong>
  </a>
  , Conghui Hu, Yongxin Yang, Yunpeng Li, Timothy M Hospedales, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openreview.net/forum?id=VuEqOs9Yp7Q" rel="noopener noreferrer" target="_blank">
   <strong>
    Temporal action localization with global segmentation mask transformers
   </strong>
  </a>
  , Sauradip Nag, Xiatian Zhu, Yi‑Zhe Song, Tao Xiang,
  <em>
   NeurIPS
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2112.02825" rel="noopener noreferrer" target="_blank">
   <strong>
    Clue me in: Semi-supervised FGVC with Out-of-Distribution Data
   </strong>
  </a>
  , Ruoyi Du, Dongliang Chang, Zhanyu Ma, Yi‑Zhe Song, Jun Guo,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2021arXiv210914449T/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    One Loss for All: Deep Hashing with a Single Cosine Similarity based Learning Objective
   </strong>
  </a>
  , Jiun Tian Hoe, Kam Woh Ng, Tianyu Zhang, Chee Seng Chan, Yi‑Zhe Song, Tao Xiang,
  <em>
   arXiv
  </em>
 </li>
</ol>

<h3>📚 2020</h3>
<ol style="padding-left: 1.2em;">
   <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-030-58565-5_10" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained visual classification via progressive multi-granularity training of jigsaw patches
   </strong>
  </a>
  , Ruoyi Du, Dongliang Chang, Ayan Kumar Bhunia, Jiyang Xie, Yi‑Zhe Song, Zhanyu Ma, Jun Guo,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9005389/" rel="noopener noreferrer" target="_blank">
   <strong>
    The devil is in the channels: Mutual-channel loss for fine-grained image classification
   </strong>
  </a>
  , Dongliang Chang, Yifeng Ding, Jiyang Xie, Ayan Kumar Bhunia, Xiaoxu Li, Zhanyu Ma, Ming Wu, Jun Guo, Yi‑Zhe Song,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Lu_Stochastic_Classifiers_for_Unsupervised_Domain_Adaptation_CVPR_2020_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Stochastic classifiers for unsupervised domain adaptation
   </strong>
  </a>
  , Zhihe Lu, Yongxin Yang, Xiatian Zhu, Cong Liu, Yi‑Zhe Song, Tao Xiang,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Bhunia_Sketch_Less_for_More_On-the-Fly_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2020_paper" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch less for more: On-the-fly fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Ayan Kumar Bhunia, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2020/html/Pang_Solving_Mixed-Modal_Jigsaw_Puzzle_for_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2020_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Solving mixed-modal jigsaw puzzle for fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Kaiyue Pang, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi‑Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://proceedings.mlr.press/v119/zhang20g.html" rel="noopener noreferrer" target="_blank">
   <strong>
    A Tree-Structured Decoder for Image-to-Markup Generation
   </strong>
  </a>
  , Jianshu Zhang, Jun Du, Yongxin Yang, Yi‑Zhe Song, Si Wei, Lirong Dai,
  <em>
   ICML
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2007.15103" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-Modal Hierarchical Modelling for Fine-Grained Sketch Based Image Retrieval
   </strong>
  </a>
  , Aneeshan Sain, Ayan Kumar Bhunia, Yongxin Yang, Tao Xiang, Yi‑Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-030-58574-7_38" rel="noopener noreferrer" target="_blank">
   <strong>
    BézierSketch: A generative model for scalable vector sketches
   </strong>
  </a>
  , Ayan Das, Yongxin Yang, Timothy Hospedales, Tao Xiang, Yi‑Zhe Song,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/3414685.3417840" rel="noopener noreferrer" target="_blank">
   <strong>
    Pixelor: A Competitive Sketching AI Agent. So you think you can sketch?
   </strong>
  </a>
  , Ayan Kumar Bhunia, Ayan Das, Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yulia Gryaditskaya, Yi‑Zhe Song,
  <em>
   TOG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9119480/" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep Self-Supervised Representation Learning for Free-Hand Sketch
   </strong>
  </a>
  , Peng Xu, Zeyu Song, Qiyue Yin, Yi‑Zhe Song, Liang Wang,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9272370/" rel="noopener noreferrer" target="_blank">
   <strong>
    Towards practical sketch-based 3d shape generation: The role of professional sketches
   </strong>
  </a>
  , Yue Zhong, Yonggang Qi, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9161000/" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-Grained Instance-Level Sketch-Based Video Retrieval
   </strong>
  </a>
  , Peng Xu, Kun Liu, Tao Xiang, Timothy M Hospedales, Zhanyu Ma, Jun Guo, Yi‑Zhe Song,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9320101/" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep Sketch-Based Modeling: Tips and Tricks
   </strong>
  </a>
  , Yue Zhong, Yulia Gryaditskaya, Honggang Zhang, Yi‑Zhe Song,
  <em>
   3DV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openresearch.surrey.ac.uk/esploro/outputs/conferencePresentation/SketchHealer-A-Graph-to-Sequence-Network-for-Recreating/99514536202346?institution=44SUR_INST" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchhealer a graph-to-sequence network for recreating partial human sketches
   </strong>
  </a>
  , Guoyao Su, Yonggang Qi, Kaiyue Pang, Jie Yang, Yi‑Zhe Song,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9147045/" rel="noopener noreferrer" target="_blank">
   <strong>
    SRD: a tree structure based decoder for online handwritten mathematical expression recognition
   </strong>
  </a>
  , Jianshu Zhang, Jun Du, Yongxin Yang, Yi‑Zhe Song, Lirong Dai,
  <em>
   TMM
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-030-66415-2_39" rel="noopener noreferrer" target="_blank">
   <strong>
    Sequential Learning for Domain Generalization
   </strong>
  </a>
  , Da Li, Yongxin Yang, Yi‑Zhe Song, Timothy Hospedales,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9102957/" rel="noopener noreferrer" target="_blank">
   <strong>
    S3Net: Graph Representational Network For Sketch Recognition
   </strong>
  </a>
  , Lan Yang, Aneeshan Sain, Linpeng Li, Yonggang Qi, Honggang Zhang, Yi‑Zhe Song,
  <em>
   ICME
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9216574/" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-a-Segmenter: Sketch-based Photo Segmenter Generation
   </strong>
  </a>
  , Conghui Hu, Da Li, Yongxin Yang, Timothy M Hospedales, Yi‑Zhe Song,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9163150/" rel="noopener noreferrer" target="_blank">
   <strong>
    SketchDesc: Learning Local Sketch Descriptors for Multi-view Correspondence
   </strong>
  </a>
  , Deng Yu, Lei Li, Youyi Zheng, Manfred Lau, Yi‑Zhe Song, Chew‑Lan Tai, Hongbo Fu,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9320353/" rel="noopener noreferrer" target="_blank">
   <strong>
    Towards 3D VR-Sketch to 3D Shape Retrieval
   </strong>
  </a>
  , Ling Luo, Yulia Gryaditskaya, Yongxin Yang, Tao Xiang, Yi‑Zhe Song,
  <em>
   3DV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9274399/" rel="noopener noreferrer" target="_blank">
   <strong>
    On learning semantic representations for large-scale abstract sketches
   </strong>
  </a>
  , Peng Xu, Yongye Huang, Tongtong Yuan, Tao Xiang, Timothy Hospedales, Yi‑Zhe Song, Liang Wang,
  <em>
   TCSVT
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/9254098/" rel="noopener noreferrer" target="_blank">
   <strong>
    IEEE access special section editorial: AI-driven big data processing: Theory, methodology, and applications
   </strong>
  </a>
  , Zhanyu Ma, Sunwoo Kim, Pascual Martínez‑Gómez, Jalil Taghia, Yi‑Zhe Song, Huiji Gao,
  <em>
   IEEE
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2003.03787" rel="noopener noreferrer" target="_blank">
   <strong>
    Mind the gap: Enlarging the domain gap in open set domain adaptation
   </strong>
  </a>
  , Dongliang Chang, Aneeshan Sain, Zhanyu Ma, Yi‑Zhe Song, Jun Guo,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/2007.04101" rel="noopener noreferrer" target="_blank">
   <strong>
    On Learning Semantic Representations for Million-Scale Free-Hand Sketches
   </strong>
  </a>
  , Peng Xu, Yongye Huang, Tongtong Yuan, Tao Xiang, Timothy M Hospedales, Yi‑Zhe Song, Liang Wang,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=10431522207885335387&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Pixelor: a competitive sketching AI agent
   </strong>
  </a>
  , Ayan Kumar Bhunia, Ayan Das, Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yulia Gryaditskaya, Yi‑Zhe Song,
  <em>
   TOG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8949551/" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch fewer to recognize more by learning a co-regularized sparse representation
   </strong>
  </a>
  , Yonggang Qi, Yi‑Zhe Song,
  <em>
   TCSVT
  </em>
 </li>

</ol>

<h3>📚 2019</h3>
<ol style="padding-left: 1.2em;">
   <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Song_Generalizable_Person_Re-Identification_by_Domain-Invariant_Mapping_Network_CVPR_2019_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Generalizable person re-identification by domain-invariant mapping network
   </strong>
  </a>
  , Jifei Song, Yongxin Yang, Yi‑Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Dey_Doodle_to_Search_Practical_Zero-Shot_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Doodle to search: Practical zero-shot sketch-based image retrieval
   </strong>
  </a>
  , Sounak Dey, Pau Riba, Anjan Dutta, Josep Llados, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Pang_Generalising_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Generalising fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Kaiyue Pang, Ke Li, Yongxin Yang, Honggang Zhang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_CVPR_2019/html/Pang_Generalising_Fine-Grained_Sketch-Based_Image_Retrieval_CVPR_2019_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Generalising fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Kaiyue Pang, Ke Li, Yongxin Yang, Honggang Zhang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/3306618.3314233" rel="noopener noreferrer" target="_blank">
   <strong>
    AI+ art= human
   </strong>
  </a>
  , Antonio Daniele, Yi-Zhe Song,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8809264/" rel="noopener noreferrer" target="_blank">
   <strong>
    Semi-heterogeneous three-way joint embedding network for sketch-based image retrieval
   </strong>
  </a>
  , Jianjun Lei, Yuxin Song, Bo Peng, Zhanyu Ma, Ling Shao, Yi-Zhe Song,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8626530/" rel="noopener noreferrer" target="_blank">
   <strong>
    Toward deep universal sketch perceptual grouper
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8626530/" rel="noopener noreferrer" target="_blank">
   <strong>
    Toward deep universal sketch perceptual grouper
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=11059045185456022370&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Artistic Assemblage
   </strong>
  </a>
  , Yi-Zhe Song, Daniele Antonio,
  <em>
   xCoAx
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ui.adsabs.harvard.edu/abs/2019arXiv190712336R/abstract" rel="noopener noreferrer" target="_blank">
   <strong>
    Goal-Driven Sequential Data Abstraction
   </strong>
  </a>
  , Umar Riaz Muhammad, Yongxin Yang, Timothy M Hospedales, Tao Xiang, Yi-Zhe Song,
  <em>
   arXiv
  </em>
 </li>

</ol>

<h3>📚 2018</h3>
<ol style="padding-left: 1.2em;">
   <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ojs.aaai.org/index.php/AAAI/article/view/11596" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning to generalize: Meta-learning for domain generalization
   </strong>
  </a>
  , Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M Hospedales,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Xu_SketchMate_Deep_Hashing_CVPR_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchmate: Deep hashing for million-scale human sketch retrieval
   </strong>
  </a>
  , Peng Xu, Yongye Huang, Tongtong Yuan, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Zhanyu Ma, Jun Guo,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Song_Learning_to_Sketch_CVPR_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning to sketch with shortcut cycle consistency
   </strong>
  </a>
  , Jifei Song, Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8401709/" rel="noopener noreferrer" target="_blank">
   <strong>
    Variational Bayesian learning for Dirichlet process mixture of inverted Dirichlet distributions in non-Gaussian image feature modeling
   </strong>
  </a>
  , Zhanyu Ma, Yuping Lai, W Bastiaan Kleijn, Yi-Zhe Song, Liang Wang, Jun Guo,
  <em>
   TNNLS
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Muhammad_Learning_Deep_Sketch_CVPR_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning deep sketch abstraction
   </strong>
  </a>
  , Umar Riaz Muhammad, Yongxin Yang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Changqing_Zou_SketchyScene_Richly-Annotated_Scene_ECCV_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketchyscene: Richly-annotated scene sketches
   </strong>
  </a>
  , Changqing Zou, Qian Yu, Ruofei Du, Haoran Mo, Yi-Zhe Song, Tao Xiang, Chengying Gao, Baoquan Chen, Hao Zhang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/3240508.3240606" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-domain adversarial feature learning for sketch re-identification
   </strong>
  </a>
  , Lu Pang, Yaowei Wang, Yi-Zhe Song, Tiejun Huang, Yonghong Tian,
  <em>
   ACM
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Ke_LI_Universal_Sketch_Perceptual_ECCV_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Universal sketch perceptual grouping
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Ke_LI_Universal_Sketch_Perceptual_ECCV_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Universal sketch perceptual grouping
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales, Honggang Zhang,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.archive.org/work/i7rkm2e5abexnn7ekmbthedx2e/access/wayback/http://bmvc2018.org/contents/papers/0040.pdf" rel="noopener noreferrer" target="_blank">
   <strong>
    Semantic Embedding for Sketch-Based 3D Shape Retrieval
   </strong>
  </a>
  , Anran Qi, Yi-Zhe Song, Tao Xiang,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_cvpr_2018/html/Hu_Sketch-a-Classifier_Sketch-Based_Photo_CVPR_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-a-classifier: Sketch-based photo classifier generation
   </strong>
  </a>
  , Conghui Hu, Da Li, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_ECCV_2018/html/Kaiyue_Pang_Deep_Factorised_Inverse-Sketching_ECCV_2018_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep factorised inverse-sketching
   </strong>
  </a>
  , Kaiyue Pang, Da Li, Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=11748417708108091907&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Greedy hash: Towards fast optimization for accurate hash coding in CNN
   </strong>
  </a>
  , Jiun Tian Hoe, Kam Woh Ng, Tianyu Zhang, Chee Seng Chan, Yi-Zhe Song, Tao Xiang,
  <em>
   NIPS
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8395088/" rel="noopener noreferrer" target="_blank">
   <strong>
    IEEE Access special section editorial: Recent advantages of computer vision
   </strong>
  </a>
  , Zhanyu Ma, Haibin Ling, Yi-Zhe Song, Timothy Hospedales, Wei Jia, Yuxin Peng, Aili Han,
  <em>
   IEEE
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://openresearch.surrey.ac.uk/esploro/outputs/journalArticle/Recent-advances-in-machine-learning-for/99511114602346" rel="noopener noreferrer" target="_blank">
   <strong>
    Recent advances in machine learning for non-Gaussian data processing
   </strong>
  </a>
  , Zhanyu Ma, J-T Chien, Z-H Tan, Yi-Zhe Song, Jalil Taghia, Ming Xiao,
  <em>
   Neurocomputing
  </em>
 </li>

</ol>


<h3>📚 2017</h3>
<ol style="padding-left: 1.2em;">
   <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_iccv_2017/html/Li_Deeper_Broader_and_ICCV_2017_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Deeper, Broader and Artier Domain Generalization
   </strong>
  </a>
  , Da Li, Yongxin Yang, Yi-Zhe Song, Timothy M. Hospedales,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/article/10.1007/s11263-016-0932-3" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-a-net: A deep neural network that beats humans
   </strong>
  </a>
  , Qian Yu, Yongxin Yang, Feng Liu, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   IJCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_iccv_2017/html/Song_Deep_Spatial-Semantic_Attention_ICCV_2017_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep Spatial-Semantic Attention for Fine-Grained Sketch-Based Image Retrieval
   </strong>
  </a>
  , Jifei Song, Yu Qian, Yi-Zhe Song, Tao Xiang, Timothy Hospedales,
  <em>
   ICCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/1711.08106" rel="noopener noreferrer" target="_blank">
   <strong>
    The devil is in the middle: Exploiting mid-level representations for cross-domain instance matching
   </strong>
  </a>
  , Qian Yu, Xiaobin Chang, Yi-Zhe Song, Tao Xiang, Timothy M Hospedales,
  <em>
   arXiv
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.research.ed.ac.uk/en/publications/cross-domain-generative-learning-for-fine-grained-sketch-based-im" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-domain Generative Learning for Fine-Grained Sketch-Based Image Retrieval
   </strong>
  </a>
  , Kaiyue Pang, Yi-Zhe Song, Tao Xiang, Timothy M. Hospedales,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0925231217314364" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-modal Subspace Learning for Fine-grained Sketch-based Image Retrieval
   </strong>
  </a>
  , Peng Xu, Qiyue Yin, Yongye Huang, Yi-Zhe Song, Zhanyu Ma, Liang Wang, Tao Xiang, W Bastiaan Kleijn, Jun Guo,
  <em>
   Neurocomputing
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.research.ed.ac.uk/en/publications/fine-grained-image-retrieval-the-textsketch-input-dilemma" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-Grained Image Retrieval: the Text/Sketch Input Dilemma
   </strong>
  </a>
  , Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy M. Hospedales,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8016664/" rel="noopener noreferrer" target="_blank">
   <strong>
    Synergistic instance-level subspace alignment for fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy M Hospedales, Tao Xiang, Honggang Zhang,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/8016664/" rel="noopener noreferrer" target="_blank">
   <strong>
    Synergistic instance-level subspace alignment for fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy M Hospedales, Tao Xiang, Honggang Zhang,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=6337503410293765834&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-a-net that beats humans [OL]
   </strong>
  </a>
  , Q Yu, Y Yang, YZ Song, T Xiang, TM Hospedales,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.research.ed.ac.uk/en/publications/now-you-see-me-deep-face-hallucination-for-unviewed-sketches" rel="noopener noreferrer" target="_blank">
   <strong>
    Now You See Me: Deep Face Hallucination for Unviewed Sketches
   </strong>
  </a>
  , Conghui Hu, Da Li, Yi-Zhe Song, Timothy M. Hospedales,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=197706842303472179&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    „Deeper
   </strong>
  </a>
  , D Li, Y Yang, YZ Song, T Hospedales,
  <em>
   CVPR
  </em>
 </li>

</ol>


<h3>📚 2016</h3>
<ol style="padding-left: 1.2em;">
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7532801/" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-based image retrieval via siamese convolutional neural network
   </strong>
  </a>
  , Yonggang Qi, Yi-Zhe Song, Honggang Zhang, Jun Liu,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0262885616301524" rel="noopener noreferrer" target="_blank">
   <strong>
    A survey on heterogeneous face recognition: Sketch, infra-red, 3D and low-resolution
   </strong>
  </a>
  , Shuxin Ouyang, Timothy Hospedales, Yi-Zhe Song, Xueming Li, Chen Change Loy, Xiaogang Wang,
  <em>
   IVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="http://openaccess.thecvf.com/content_cvpr_2016/html/Ouyang_ForgetMeNot_Memory-Aware_Forensic_CVPR_2016_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Forgetmenot: Memory-aware forensic facial sketch matching
   </strong>
  </a>
  , Shuxin Ouyang, Timothy M Hospedales, Yi-Zhe Song, Xueming Li,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/article/10.1007/s11263-016-0963-9" rel="noopener noreferrer" target="_blank">
   <strong>
    Free-hand sketch synthesis with deformable stroke models
   </strong>
  </a>
  , Y. Li, Y-Z. Song, T. Hospedales, S. Gong,
  <em>
   IJCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.research.ed.ac.uk/en/publications/deep-multi-task-attribute-driven-ranking-for-fine-grained-sketch-" rel="noopener noreferrer" target="_blank">
   <strong>
    Deep multi-task attribute-driven ranking for fine-grained sketch-based image retrieval
   </strong>
  </a>
  , Jifei Song, Yi-Zhe Song, Tao Xiang, Timothy Hospedales, Xiang Ruan,
  <em>
   AAAI
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7477615/" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained sketch-based image retrieval: The role of part-aware attributes
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy Hospedales, Honggang Zhang, Yichuan Hu,
  <em>
   WACV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7477615/" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-grained sketch-based image retrieval: The role of part-aware attributes
   </strong>
  </a>
  , Ke Li, Kaiyue Pang, Yi-Zhe Song, Timothy Hospedales, Honggang Zhang, Yichuan Hu,
  <em>
   WACV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=13550880441023903228&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch me that shoe
   </strong>
  </a>
  , Yyu Qian, Liu Feng, Yi-Zhe Song, Xiang Tao, Change Loy Chen,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7974625/" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-modal subspace learning for sketch-based image retrieval: A comparative study
   </strong>
  </a>
  , Peng Xu, Ke Li, Zhanyu Ma, Yi-Zhe Song, Liang Wang, Jun Guo,
  <em>
   IC-NIDC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7974625/" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-modal subspace learning for sketch-based image retrieval: A comparative study
   </strong>
  </a>
  , Peng Xu, Ke Li, Zhanyu Ma, Yi-Zhe Song, Liang Wang, Jun Guo,
  <em>
   IC-NIDC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7805451/" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-modal face matching: Tackling visual abstraction using fine-grained attributes
   </strong>
  </a>
  , Yichuan Hu, Ke Li, Honggang Zhang,
  <em>
   VCIP
  </em>
 </li>


</ol>

<h3>📚 2015</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://arxiv.org/abs/1501.07873" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch-a-net that beats humans
   </strong>
  </a>
  , Qian Yu, Yongxin Yang, Yi-Zhe Song, Tao Xiang, Timothy Hospedales,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S1077314215000375" rel="noopener noreferrer" target="_blank">
   <strong>
    Free-hand sketch recognition by multi-kernel feature learning
   </strong>
  </a>
  , Yi Li, Timothy M Hospedales, Yi-Zhe Song, Shaogang Gong,
  <em>
   CVIU
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Qi_Making_Better_Use_2015_CVPR_paper.html" rel="noopener noreferrer" target="_blank">
   <strong>
    Making better use of edges via perceptual grouping
   </strong>
  </a>
  , Yonggang Qi, Yi-Zhe Song, Tao Xiang, Honggang Zhang, Timothy Hospedales, Yi Li, Jun Guo,
  <em>
   CVPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0925231215003082" rel="noopener noreferrer" target="_blank">
   <strong>
    Im2sketch: Sketch generation by unconflicted perceptual grouping
   </strong>
  </a>
  , Yonggang Qi, Jun Guo, Yi-Zhe Song, Tao Xiang, Honggang Zhang, Zheng-Hua Tan,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0925231215000260" rel="noopener noreferrer" target="_blank">
   <strong>
    Multi-label learning with prior knowledge for facial expression analysis
   </strong>
  </a>
  , Kaili Zhao, Honggang Zhang, Zhanyu Ma, Yi-Zhe Song, Jun Guo,
  <em>
   TIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7177409/" rel="noopener noreferrer" target="_blank">
   <strong>
    Refining graph matching using inherent structure information
   </strong>
  </a>
  , Wenzhao Li, Yi-Zhe Song, Andrea Cavallaro,
  <em>
   ICME
  </em>
 </li>

</ol>

<h3>📚 2014</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://qmro.qmul.ac.uk/jspui/handle/123456789/6440" rel="noopener noreferrer" target="_blank">
   <strong>
    Fine-Grained Sketch-Based Image Retrieval by Matching Deformable Part Models
   </strong>
  </a>
  , Yi Li, Timothy M Hospedales, Yi-Zhe Song, Shaogang Gong,
  <em>
   CVG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://journals.sagepub.com/doi/abs/10.1177/1475921714522841" rel="noopener noreferrer" target="_blank">
   <strong>
    Virtual visual sensors and their application in structural health monitoring
   </strong>
  </a>
  , Yi-Zhe Song, Chris R Bowen, Alicia H Kim, Aydin Nassehi, Julian Padget, Nick Gathercole,
  <em>
   SHM
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-319-16808-1_15" rel="noopener noreferrer" target="_blank">
   <strong>
    Cross-modal face matching: beyond viewed sketches
   </strong>
  </a>
  , Shuxin Ouyang, Timothy Hospedales, Yi-Zhe Song, Xueming Li,
  <em>
   ACCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0888327013006808" rel="noopener noreferrer" target="_blank">
   <strong>
    Non-invasive damage detection in beams using marker extraction and wavelets
   </strong>
  </a>
  , Yi-Zhe Song, Chris R Bowen, H Alicia Kim, Aydin Nassehi, Julian Padget, Nick Gathercole, Andrew Dent,
  <em>
   SPIE
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/7000322/" rel="noopener noreferrer" target="_blank">
   <strong>
    A Patch-based Sparse Representation for Sketch Recognition
   </strong>
  </a>
  , Yonggong Qi, Honggang Zhang, Yi-Zhe Song, Zheng-Hua Tan,
  <em>
   IEEE
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-319-14364-4_8" rel="noopener noreferrer" target="_blank">
   <strong>
    One-shot learning of sketch categories with co-regularized sparse coding
   </strong>
  </a>
  , Yonggang Qi, Wei-Shi Zheng, Tao Xiang, Yi-Zhe Song, Honggang Zhang, Jun Guo,
  <em>
   ISVC
  </em>
 </li>


</ol>

<h3>📚 2013</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0925231213006309" rel="noopener noreferrer" target="_blank">
   <strong>
    Text extraction from natural scene image: A survey
   </strong>
  </a>
  , Honggang Zhang, Kaili Zhao, Yi-Zhe Song, Jun Guo,
  <em>
   Neurocomputing
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.eecs.qmul.ac.uk/~sgg/papers/LiEtAl_BMVC2013.pdf" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketch recognition by ensemble matching of structured features.
   </strong>
  </a>
  , Yi Li, Yi-Zhe Song, Shaogang Gong,
  <em>
   BMVC
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/6738056/" rel="noopener noreferrer" target="_blank">
   <strong>
    Sketching by perceptual grouping
   </strong>
  </a>
  , Yonggang Qi, Jun Guo, Yi Li, Honggang Zhang, Tao Xiang, Yi-Zhe Song,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/6461879/" rel="noopener noreferrer" target="_blank">
   <strong>
    Abstract art by shape classification
   </strong>
  </a>
  , Yi-Zhe Song, David Pickup, Chuan Li, Paul Rosin, Peter Hall,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/2487276.2487288" rel="noopener noreferrer" target="_blank">
   <strong>
    Simple art as abstractions of photographs
   </strong>
  </a>
  , Peter Hall, Yi-Zhe Song,
  <em>
   CAE
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/6706384/" rel="noopener noreferrer" target="_blank">
   <strong>
    Perceptual grouping via untangling Gestalt principles
   </strong>
  </a>
  , Yonggang Qi, Jun Guo, Yi Li, Honggang Zhang, Tao Xiang, Yi-Zhe Song, Zheng-Hua Tan,
  <em>
   VCIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/6706330/" rel="noopener noreferrer" target="_blank">
   <strong>
    A multi-label classification approach for facial expression recognition
   </strong>
  </a>
  , Kaili Zhao, Honggang Zhang, Mingzhi Dong, Jun Guo, Yonggang Qi, Yi-Zhe Song,
  <em>
   VCIP
  </em>
 </li>


</ol>

<h3>📚 2012</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S0925231212001956" rel="noopener noreferrer" target="_blank">
   <strong>
    Robust visual tracking using structural region hierarchy and graph matching
   </strong>
  </a>
  , Yi-Zhe Song, Chuan Li, Liang Wang, Peter Hall, Peiyi Shen,
  <em>
   Neurocomputing
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/6418792/" rel="noopener noreferrer" target="_blank">
   <strong>
    A dataset for scene classification based on camera metadata
   </strong>
  </a>
  , Kaili Zhao, Can Cao, Honggang Zhang, Yizhe Song,
  <em>
   ICIP
  </em>
 </li>

</ol>

<h3>📚 2011</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://dl.acm.org/doi/abs/10.1145/2070781.2024161" rel="noopener noreferrer" target="_blank">
   <strong>
    Modeling and generating moving trees from video
   </strong>
  </a>
  , Chuan Li, Oliver Deussen, Yi-Zhe Song, Phil Willis, Peter Hall,
  <em>
   TOG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.sciencedirect.com/science/article/pii/S1077314211000841" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning invariant structure for object identification by using graph methods
   </strong>
  </a>
  , Bai Xiao, Song Yi-Zhe, Peter Hall,
  <em>
   CVIU
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.spiedigitallibrary.org/conference-proceedings-of-spie/7983/79830R/Non-invasive-damage-detection-in-composite-beams-using-marker-extraction/10.1117/12.880055.short" rel="noopener noreferrer" target="_blank">
   <strong>
    Non-invasive damage detection in composite beams using marker extraction and wavelets
   </strong>
  </a>
  , Yi-Zhe Song, Chris Bowen, H Alicia Kim, Aydin Nassehi, Julian Padget, Nick Gathercore, Andrew Dent,
  <em>
   SPIE
  </em>
 </li>


</ol>

<h3>📚 2010</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-642-15561-1_50" rel="noopener noreferrer" target="_blank">
   <strong>
    Finding semantic structures in image hierarchies using Laplacian graph energy
   </strong>
  </a>
  , Yi-Zhe Song, Pablo Arbelaez, Peter Hall, Chuan Li, Anupriya Balikai,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/5604693/" rel="noopener noreferrer" target="_blank">
   <strong>
    In search of perceptually salient groupings
   </strong>
  </a>
  , Yi-Zhe Song, Bai Xiao, Peter Hall, Liang Wang,
  <em>
   ICIP
  </em>
 </li>


</ol>

<h3>📚 2009</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/5336462/" rel="noopener noreferrer" target="_blank">
   <strong>
    Mobile augmented reality based 3D snapshots
   </strong>
  </a>
  , Peter Keitler, Frieder Pankratz, Bjorn Schwerdtfeger, Daniel Pustka, Wolf Rodiger, Gudrun Klinker, Christian Rauch, Anup Chathoth, John Collomosse, Yi-Zhe Song,
  <em>
   ISMAR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=1156167040563393860&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Hierarchical image descriptions for classification and painting
   </strong>
  </a>
  , Yi-Zhe Song,
  <em>
   University
  </em>
 </li>

</ol>

<h3>📚 2008</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://diglib.eg.org/bitstream/handle/10.2312/COMPAESTH.COMPAESTH08.065-072/065-072.pdf?sequence=1" rel="noopener noreferrer" target="_blank">
   <strong>
    Arty Shapes.
   </strong>
  </a>
  , Yi-Zhe Song, Paul L Rosin, Peter M Hall, John P Collomosse,
  <em>
   EG
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-540-89689-0_37" rel="noopener noreferrer" target="_blank">
   <strong>
    Structure is a visual class invariant
   </strong>
  </a>
  , Bai Xiao, Yi-Zhe Song, Anupriya Balika, Peter M Hall,
  <em>
   ECCV
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://link.springer.com/chapter/10.1007/978-3-540-89639-5_31" rel="noopener noreferrer" target="_blank">
   <strong>
    Stable image descriptions using Gestalt principles
   </strong>
  </a>
  , Yi-Zhe Song, Peter M Hall,
  <em>
   SSPR
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://www.researchgate.net/profile/Paul-Rosin/publication/221259874_Shapes_Fit_For_Purpose/links/0fcfd5107ee7911fef000000/Shapes-Fit-For-Purpose.pdf" rel="noopener noreferrer" target="_blank">
   <strong>
    Shapes Fit For Purpose.
   </strong>
  </a>
  , Anupriya Balikai, Paul L Rosin, Yi-Zhe Song, Peter M Hall,
  <em>
   BMVC
  </em>
 </li>


</ol>

<h3>📚 2007</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://ieeexplore.ieee.org/abstract/document/4276077/" rel="noopener noreferrer" target="_blank">
   <strong>
    RTcams: A new perspective on nonphotorealistic rendering from photographs
   </strong>
  </a>
  , Peter M Hall, John P Collomosse, Yi-Zhe Song, Peiyi Shen, Chuan Li,
  <em>
   ICIP
  </em>
 </li>
 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://scholar.google.com/scholar?cluster=3987824411733545783&amp;hl=en&amp;oi=scholarr" rel="noopener noreferrer" target="_blank">
   <strong>
    Learning Object Classes from Structure.
   </strong>
  </a>
  , Xiao Bai, Yi-Zhe Song, Peter M Hall,
  <em>
   BMVC
  </em>
 </li>


</ol>


<h3>📚 2005</h3>
<ol style="padding-left: 1.2em;">

 <li style="margin-bottom: 0.4em; line-height: 1.4;">
  <a href="https://diglib.eg.org/bitstreams/bd37c179-e25c-4076-ac93-6a9b0ccadfe6/download" rel="noopener noreferrer" target="_blank">
   <strong>
    Visual Recognition of Man-made Materials and Structures in an Office Environment.
   </strong>
  </a>
  , Yi-Zhe Song, Christopher P Town,
  <em>
   VVG
  </em>
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
    <li>📄59 x CVPR, 15 x ICCV, 17 x ECCV, 7 x AAAI, 5 x ICLR, 3 x NeurIPS, 1 x ICML </li>
  </ul>
</div>


<!-- Section: Downloads -->
<div class="section" id="downloads-section">
  <h2>📦 Downloads</h2>

  <h3 style="color: #ff6600; margin-top: 1.5em;">📁 Datasets</h3>

  <div class="dataset-gallery">
    <figure class="dataset-item">
      <a href="https://drive.google.com/u/0/uc?export=download&amp;confirm=tToE&amp;id=1mWEY7vFkOw790DwUtqcTX8fHzNBP_b1J" target="_blank">
        <img src="{{ '/images/SlowSketch.png' | relative_url }}" alt="SlowSketch Dataset">
      </a>
      <figcaption>
        <a href="https://drive.google.com/u/0/uc?export=download&amp;confirm=tToE&amp;id=1mWEY7vFkOw790DwUtqcTX8fHzNBP_b1J" target="_blank">SlowSketch</a>
        <span style="color: #ff6600;">(*NEW*)</span>
      </figcaption>
    </figure>

    <figure class="dataset-item">
      <a href="https://dali-dl.github.io/project_iccv2017.html" target="_blank">
        <img src="{{ '/images/project_img1-1.png' | relative_url }}" alt="PACS Dataset">
      </a>
      <figcaption>
        <a href="https://dali-dl.github.io/project_iccv2017.html" target="_blank">PACS (Deeper, Broader and Artier Domain Generalization)</a>
      </figcaption>
    </figure>

    <figure class="dataset-item">
      <a href="https://drive.google.com/u/0/uc?id=15s2BR-QwLgX_DObQBrYlUlZqUU90EL9G&amp;export=download" target="_blank">
        <img src="{{ '/images/dataset2-1024x600.jpg' | relative_url }}" alt="Fine-Grained SBIR Dataset v2">
      </a>
      <figcaption>
        <a href="https://drive.google.com/u/0/uc?id=15s2BR-QwLgX_DObQBrYlUlZqUU90EL9G&amp;export=download" target="_blank">Fine-Grained SBIR Datasets</a>
        <span style="color: #ff6600;">(v2 released!!)</span>
      </figcaption>
    </figure>

    <figure class="dataset-item">
      <a href="https://github.com/panly099/fine-graind-SBIR" target="_blank">
        <img src="{{ '/images/markings-1024x394.jpg' | relative_url }}" alt="Fine-Grained SBIR PASCAL VOC">
      </a>
      <figcaption>
        <a href="https://github.com/panly099/fine-graind-SBIR" target="_blank">Fine-Grained SBIR Dataset (PASCAL VOC)</a>
      </figcaption>
    </figure>
  </div>

  <h3 style="color: #ff6600; margin-top: 2em;">💻 Code</h3>
  <ul>
    <li>
      Free-hand sketch synthesis with deformable stroke models:
      <a href="https://github.com/panly099/sketchSynthesis" target="_blank">code</a> (Matlab)
    </li>
    <li>
      Fine-grained sketch-based image retrieval by matching DPM:
      <a href="https://github.com/panly099/fine-graind-SBIR" target="_blank">code</a> (Matlab)
    </li>
  </ul>
</div>



<!-- Section: Projects -->
<div class="section" id="projects-section" >
  <h2>🚀Projects</h2>
  projects
</div>

<!-- Section: News -->
<div class="section" id="news-section">
  <h2>🔥 Team News</h2>

  <h3>1 Paper in AAAI’25 !</h3>
  <ul style="padding-left: 1.2em;">
    <li>
      VersaGen: Unleashing Versatile Visual Control for Text-to-Image Synthesis  
      Zhipeng Chen, Lan Yang, Yonggang Qi, Honggang Zhang, Kaiyue Pang, Ke Li, Yi-Zhe Song, AAAI 2025
    </li>
  </ul>

  <h3>18 Papers in CVPR/ECCV/ICLR’24 ! </h3>
  <ul style="padding-left: 1.2em;">
    <li>Demofusion: Democratising high-resolution image generation with no $$$  
        Ruoyi Du, Dongliang Chang, Timothy Hospedales, Yi-Zhe Song, Zhanyu Ma, CVPR 2024</li>
    <li>It's All About Your Sketch: Democratising Sketch Control in Diffusion Models  
        Subhadeep Koley, Ayan Kumar Bhunia, Deeptanshu Sekhri, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>How to handle sketch-abstraction in sketch-based image retrieval?  
        Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>You'll Never Walk Alone: A Sketch and Text Duet for Fine-Grained Image Retrieval  
        Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>Doodle your 3d: From abstract freehand sketches to precise 3d shapes  
        Hmrishav Bandyopadhyay, Subhadeep Koley, Ayan Das, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>Sketchinr: A first look into sketches as implicit neural representations  
        Hmrishav Bandyopadhyay, Ayan Kumar Bhunia, Pinaki Nath Chowdhury, Aneeshan Sain, Tao Xiang, Timothy Hospedales, Yi-Zhe Song, CVPR 2024</li>
    <li>Text-to-image diffusion models are great sketch-photo matchmakers  
        Subhadeep Koley, Ayan Kumar Bhunia, Aneeshan Sain, Pinaki Nath Chowdhury, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>Wired perspectives: Multi-view wire art embraces generative ai  
        Zhiyu Qu, Lan Yang, Honggang Zhang, Tao Xiang, Kaiyue Pang, Yi-Zhe Song, CVPR 2024</li>
    <li>Democaricature: Democratising caricature generation with a rough sketch  
        Dar-Yen Chen, Ayan Kumar Bhunia, Subhadeep Koley, Aneeshan Sain, Pinaki Nath Chowdhury, Yi-Zhe Song, CVPR 2024</li>
    <li>ConceptHash: Interpretable Fine-Grained Hashing via Concept Discovery  
        Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang, CVPR 2024</li>
    <li>What Sketch Explainability Really Means for Downstream Tasks?  
        Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Ayan Kumar Bhunia, Aneeshan Sain, Tao Xiang, Yi-Zhe Song, CVPR 2024</li>
    <li>PartCraft: Crafting Creative Objects by Parts  
        Kam Woh Ng, Xiatian Zhu, Yi-Zhe Song, Tao Xiang, ECCV 2024</li>
    <li>Do Generalised Classifiers Really Work on Human Drawn Sketches?  
        Hmrishav Bandyopadhyay, Pinaki Nath Chowdhury, Aneeshan Sain, Subhadeep Koley, Tao Xiang, Ayan Kumar Bhunia, Yi-Zhe Song, ECCV 2024</li>
    <li>Freeview Sketching: View-Aware Fine-Grained Sketch-Based Image Retrieval  
        Aneeshan Sain, Pinaki Nath Chowdhury, Subhadeep Koley, Ayan Kumar Bhunia, Yi-Zhe Song, ECCV 2024</li>
    <li>Modelling complex vector drawings with stroke-clouds  
        Alexander Ashcroft, Ayan Das, Yulia Gryaditskaya, Zhiyu Qu, Yi-Zhe Song, ICLR 2024</li>
    <li>Ipr-nerf: Ownership verification meets neural radiance field  
        Win Kent Ong, Kam Woh Ng, Chee Seng Chan, Yi-Zhe Song, Tao Xiang, ICLR 2024</li>
    <li>Scale-Adaptive Diffusion Model for Complex Sketch Synthesis  
        Jijin Hu, Ke Li, Yonggang Qi, Yi-Zhe Song, ICLR 2024</li>
  </ul>
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

  const slider = document.querySelector('.bx-slider');
  const slides = document.querySelectorAll('.slides');
  const prev = document.getElementById('slider-prev');
  const next = document.getElementById('slider-next');

  let currentIndex = 0;

  function showSlide(index) {
    const offset = -index * 100;
    slider.style.transform = `translateX(${offset}%)`;
  }

  prev.addEventListener('click', () => {
    currentIndex = (currentIndex - 1 + slides.length) % slides.length;
    showSlide(currentIndex);
  });

  next.addEventListener('click', () => {
    currentIndex = (currentIndex + 1) % slides.length;
    showSlide(currentIndex);
  });

  // Optional: auto-play every 5 seconds
  setInterval(() => {
    currentIndex = (currentIndex + 1) % slides.length;
    showSlide(currentIndex);
  }, 5000);
</script>



