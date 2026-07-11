---
permalink: /
title: "Qi Li"
excerpt: ""
author_profile: false
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

<section class="hero" aria-labelledby="hero-title">
  <div class="hero__content">
    <p class="hero__eyebrow">Postdoctoral Researcher · Tsinghua University</p>
    <h1 id="hero-title" class="hero__title">Trustworthy AI for Industrial Intelligence</h1>
    <p class="hero__lead">I develop trustworthy and generalizable AI methods for industrial time-series understanding, fault diagnosis, and prognostics and health management.</p>
    <div class="hero__actions" aria-label="Profile links">
      <a class="hero__button hero__button--primary" href="https://scholar.google.com/citations?user=vCabh8oAAAAJ">Google Scholar</a>
      <a class="hero__button" href="https://github.com/liq22">GitHub</a>
      <a class="hero__button" href="mailto:liq22@tsinghua.org.cn">Email</a>
      <a class="hero__button" href="https://orcid.org/0000-0001-7105-2818">ORCID</a>
    </div>
    <ul class="hero__highlights" aria-label="Research highlights">
      <li><strong><span id="total_cit">1200+</span></strong><span>Google Scholar citations</span></li>
      <li><strong>3</strong><span>Core research themes</span></li>
      <li><strong>THU</strong><span>Department of Automation</span></li>
    </ul>
    <div class="hero__tags" aria-label="Research interests">
      <span>Trustworthy AI</span>
      <span>Foundation Models</span>
      <span>Reliable PHM</span>
    </div>
  </div>
  <div class="hero__portrait-frame">
    <img class="hero__portrait" src="{{ '/images/LQ.png' | relative_url }}" alt="Qi Li" decoding="async" fetchpriority="high">
  </div>
</section>

<span class='anchor' id='about-me'></span>
# 👋 About Me

I am a **postdoctoral researcher** in the Department of Automation at **Tsinghua University**, working with Prof. [Xiao He](https://www.au.tsinghua.edu.cn/info/1092/1527.htm). My previous academic experience includes:

- *Sep 2022 - Jun 2026*: Ph.D. in **Mechanical Engineering** at **Tsinghua University**, supervised by Prof. [Zhaoye Qin](https://www.me.tsinghua.edu.cn/info/1127/1763.htm) in the group of Prof. [Fulei Chu](https://www.researchgate.net/profile/Fulei-Chu-3).
- *Apr 2025 - Sep 2025*: Visiting scholar at **Yale University**, working with Prof. [Lu Lu](https://lugroup.yale.edu).
- *Apr 2022 - Sep 2022*: Research intern at **AIR, Tsinghua University**, supervised by [Yuanchun Li](https://air.tsinghua.edu.cn/info/1046/1195.htm).
- *Sep 2019 - Jun 2022*: M.Eng. in **Control Theory and Control Engineering** at Soochow University (SUDA), supervised by [Prof. Liang Chen](http://jdxy.suda.edu.cn/d1/f2/c14011a446962/page.htm) and [Prof. Changqing Shen](http://web.suda.edu.cn/cqshen/).
- *Sep 2015 - Jun 2019*: B.Eng. in **Electrical Engineering** at SUDA.

My research interests include **trustworthy AI**, **foundation models**, and **reliable prognostics and health management (PHM)**. My work focuses on developing interpretable, generalizable, and reliable learning systems for industrial applications. Please feel free to contact me regarding research collaboration.

# 🔥 News

- *2026.07*: Joined the Department of Automation at Tsinghua University as a postdoctoral researcher.
- *2026.06*: Received the Distinguished Graduate honor from Tsinghua University.
- *2026.04*: Named an Academic Rising Star of Tsinghua Mechanical Engineering.
- *2026*: VSLLaVA was published in *Advanced Engineering Informatics*.
- *2026*: Received the Merit Student Award from Tsinghua University.
- *2025.12*: Received the Shuimu Scholar Fellowship.
- *2025.11*: Served as a session chair at PHMAP.
- *2025.09*: Received the National Scholarship.
- *2025.04*: A paper was accepted by *Information Fusion*.
- *2025.01*: A paper was accepted by *Advanced Engineering Informatics*.
- *2025.01*: Selected for the 2024 CAST Youth Talent Support Program - Ph.D. Special Plan - CCF.
- *2024.12*: Received the Science and Technology Award of the Chinese Society of Vibration Engineering.
- *2024.11*: A paper was accepted by the *Journal of Manufacturing Systems*.
- *2024.02*: A paper was accepted by *IEEE Transactions on Industrial Informatics*.
- *2023.02*: A paper was accepted by *Reliability Engineering & System Safety*.
- *2022.05*: Received the Future Scholars Scholarship from Tsinghua University.

# 📝 Publications

<details>
<summary><h2>🔖 PHM Foundation Models</h2></summary>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Advanced Engineering Informatics 2026</div>
      <img src="{{ '/images/papers/VSLLAVA.png' | relative_url }}" alt="VSLLaVA pipeline for industrial vibration signal analysis" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

VSLLaVA: a pipeline of large multimodal foundation model for industrial vibration signal analysis

**Qi Li**, Xinran Zhang, Jinfeng Huang, Hongliang He, Feibin Zhang\*, Zhaoye Qin\*, Fulei Chu

- Published in *Advanced Engineering Informatics*, 2026. *(SCI, CAS Q1 Top; Impact Factor: 11.5)*

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Information Fusion 2025</div>
      <img src="{{ '/images/papers/HSE.png' | relative_url }}" alt="Heterogeneous Signal Embedding framework" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[HSE: A Plug-and-Play Module for Unified Fault Diagnosis Foundation Models](https://doi.org/10.1016/j.inffus.2025.103277)

**Qi Li**, Bojian Chen, Qitong Chen, Xuan Li, Zhaoye Qin, Fulei Chu

- Proposes a Heterogeneous Signal Embedding (HSE) module that projects heterogeneous signals into a unified signal space and integrates with existing intelligent fault-diagnosis architectures as a plug-and-play component. *(JCR Q1; Impact Factor: 14.4)*
- [Code](https://github.com/liq22/ISFM_HSE)

</div>
</div>

</details>

<details>
<summary><h2>🔖 Neuro-symbolic Diagnosis</h2></summary>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">ADVEI 2025</div>
      <img src="{{ '/images/papers/TIFN.png' | relative_url }}" alt="Transparent information fusion network" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Transparent information fusion network: An explainable network for multi-source bearing fault diagnosis via self-organized neural-symbolic nodes](https://doi.org/10.1016/j.aei.2025.103156)

**Qi Li**, Lichang Qin, Haifeng Xu, Qijian Lin, Zhaoye Qin, Fulei Chu

- Introduces a transparent information fusion network with self-organized neural-symbolic nodes, enabling explainable multi-source fault diagnosis through knowledge-informed decision-making. *(JCR Q1; Impact Factor: 8.0)*

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">JMS 2024</div>
      <img src="{{ '/images/papers/DEN.png' | relative_url }}" alt="Deep Expert Network architecture" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Deep Expert Network: A Unified Method toward Knowledge-Informed Fault Diagnosis via Fully Interpretable Neuro-Symbolic AI](https://doi.org/10.1016/j.jmsy.2024.10.007)

**Qi Li**, Yuekai Liu, Shilin Sun, Zhaoye Qin, Fulei Chu

- Proposes a neuro-symbolic approach to fault diagnosis that incorporates interpretable expert knowledge through a Deep Expert Network. *(JCR Q1; Impact Factor: 12.2)*

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">IEEE TII 2024</div>
      <img src="{{ '/images/papers/TON.png' | relative_url }}" alt="Transparent Operator Network architecture" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Transparent Operator Network: A Fully Interpretable Network Incorporating Learnable Wavelet Operator for Intelligent Fault Diagnosis](https://doi.org/10.1109/TII.2024.3366993)

**Qi Li**, Hua Li, Wenyang Hu, Shilin Sun, Zhaoye Qin, Fulei Chu

- Introduces an interpretable method for industrial time-series classification by integrating learnable wavelet operators. *(JCR Q1; Impact Factor: 12.3)*

</div>
</div>

</details>

<details>
<summary><h2>🔖 Cross-domain Diagnosis</h2></summary>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">RESS 2023</div>
      <img src="{{ '/images/papers/CADA.png' | relative_url }}" alt="Cross-domain augmentation diagnosis framework" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Cross-Domain Augmentation Diagnosis: An Adversarial Domain-Augmented Generalization Method for Fault Diagnosis under Unseen Working Conditions](https://doi.org/10.1016/j.ress.2023.109171)

**Qi Li**, Liang Chen, Lin Kong, Dong Wang, Min Xia, Changqing Shen

- Presents a domain-generalization approach that combines adversarial learning and data augmentation for robust industrial time-series classification. *(JCR Q1; Impact Factor: 9.4)*

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">IEEE TII 2022</div>
      <img src="{{ '/images/papers/ADIG.jpg' | relative_url }}" alt="Adversarial domain-invariant generalization framework" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Adversarial Domain-Invariant Generalization: A Generic Domain-Regressive Framework for Bearing Fault Diagnosis under Unseen Conditions](https://ieeexplore.ieee.org/document/9428592/)

**Chen Liang**, **Qi Li**, Changqing Shen, Jun Zhu, Dong Wang, Min Xia

- Introduces a domain-regressive framework that uses adversarial learning between feature extractors and domain classifiers to improve diagnosis under unseen conditions. *(JCR Q1; Impact Factor: 11.7; highly cited)*

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">MSSP 2021</div>
      <img src="{{ '/images/papers/KMADA.jpg' | relative_url }}" alt="Knowledge mapping-based adversarial domain adaptation framework" loading="lazy" decoding="async" fetchpriority="low">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Knowledge Mapping-Based Adversarial Domain Adaptation: A Novel Fault Diagnosis Method with High Generalizability under Variable Working Conditions](https://doi.org/10.1016/j.ymssp.2020.107095)

**Qi Li**, Changqing Shen, Liang Chen, Zhongkui Zhu

- Introduces a knowledge-mapping and adversarial-learning strategy that improves generalizability across variable operating conditions. *(JCR Q1; Impact Factor: 7.9; highly cited)*

</div>
</div>
</details>

# 🎖 Honors and Awards

- *2026*: Distinguished Graduate, Tsinghua University.
- *2026*: Merit Student Award, Tsinghua University.
- *2026*: Academic Rising Star of Tsinghua Mechanical Engineering.
- *2025*: Shuimu Scholar Fellowship.
- *2025*: National Scholarship, Ministry of Education of China.
- *2025*: The 2024 CAST Youth Talent Support Program - Ph.D. Special Plan - CCF.
- *2024*: Tsinghua Scholarship for Overseas Graduate Studies.
- *2024*: Science and Technology Award of the Chinese Society of Vibration Engineering.
- *2023*: Social Practice Scholarship, Tsinghua University.
- *2022*: Future Scholars Scholarship, Tsinghua University.
- *2021*: National Scholarship, Ministry of Education of China.
- *2021*: Outstanding Student Cadre of Jiangsu Province.
- *2021*: Outstanding Postgraduate Cadre, Soochow University.
- *2020*: National Scholarship, Ministry of Education of China.
- *2020*: Outstanding Postgraduate, Soochow University.
- *2019*: Special Award of the Graduate Academic Scholarship.
- *2019*: Delivered the graduate student representative address at the opening ceremony of Soochow University.
- *2019*: Outstanding Graduate, Soochow University.

# 📖 Education

- *2026.07 - Present*: Postdoctoral researcher in the Department of Automation at Tsinghua University, working with Prof. [Xiao He](https://www.au.tsinghua.edu.cn/info/1092/1527.htm).
- *2025.04 - 2025.09*: Visiting scholar in Statistics and Data Science at Yale University, working with Prof. [Lu Lu](https://lugroup.yale.edu).
- *2022.09 - 2026.06*: Ph.D. in Mechanical Engineering, Tsinghua University; supervisor: Prof. Zhaoye Qin.
- *2019.09 - 2022.06*: M.Eng. in Control Theory and Control Engineering, Soochow University; supervisors: Prof. Liang Chen and Prof. Changqing Shen.
- *2015.09 - 2019.06*: B.Eng. in Electrical Engineering, Soochow University.

# 💬 Invited Talks

- *2024.04*: Beijing AI Ph.D. Student Forum, Beijing, China (approximately 20,000 viewers).
- *2023.11*: PHM Conference, Hangzhou, China.
- *2023.04*: Tsinghua University Mechanical Engineering Ph.D. Student Forum.
- *2020.07*: IEEE INDIN 2020, Warwick, United Kingdom.
- *2018.07*: SDPC 2018, Xi'an, China.

# 💻 Internships

- *Mar 2022 - Aug 2022*: Research Intern at the Institute for AI Industry Research (AIR), Tsinghua University.
  - Conducted research on AI-enabled time-series analysis for battery monitoring.

# 🔧 Skills

- **English**: CSC English Test, 104/130.
- **Programming**: Python, MATLAB, PyTorch, and TensorFlow.
- **Interests**: Marathon running, positive psychology, and strength training.

# 🖥 Peer Review Service

- *Information Fusion*
- *Advanced Engineering Informatics*
- *IEEE Transactions on Industrial Informatics*
- *Mechanical Systems and Signal Processing*
- *IEEE Transactions on Industrial Electronics*
- *IEEE Transactions on Instrumentation and Measurement*
- *Measurement*
- *Measurement Science and Technology*
- *IEEE Transactions on Systems, Man, and Cybernetics: Systems*
- *IEEE Transactions on Cybernetics*
- *IEEE Transactions on Reliability*
- *Engineering*
- *Applied Soft Computing*
- *Reliability Engineering & System Safety*

# 🤔 Projects

- Vibration and noise reduction for aerospace systems (key contributor).
- Parameter measurement for aerospace systems (key contributor).
- Lead the open-source [PHMBench](https://github.com/PHMBench) project group and contribute to broader PHM research initiatives.
- [Self-Distillation During My Ph.D.](https://github.com/liq22/THU_Self-Distillation)

# 🎙 Social Activities

- *2025*: Interviewed by Tsinghua University ([link](https://mp.weixin.qq.com/s/dPp1mKACXWI0FLqtREoPPA)).
- *2023*: Volunteer at the IFToMM International Conference on Rotordynamics.
- *2019 - 2022*: Graduate student class representative in the School of Mechanical and Electric Engineering, Soochow University.
- *2021*: Interviewed by the Student Union of Soochow University ([link](https://mp.weixin.qq.com/s/zW07Tp2uh0CkHzmfCAVnqw)).
- *2019*: Delivered the graduate student representative address at the opening ceremony of Soochow University ([link](https://mp.weixin.qq.com/s/HQSOWfekFaz2hYdh-4hvwA)).

# 📫 Contact

- **Email**: [liq22@tsinghua.org.cn](mailto:liq22@tsinghua.org.cn)
- **Google Scholar**: [Qi Li](https://scholar.google.com/citations?user=vCabh8oAAAAJ)
- **GitHub**: [liq22](https://github.com/liq22)
- **ORCID**: [0000-0001-7105-2818](https://orcid.org/0000-0001-7105-2818)

<p class="page-updated">Last updated: July 2026</p>
