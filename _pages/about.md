---
permalink: /
title: "Qi Li"
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
# 👋 About Me

I am a **Ph.D. student** in the Department of Mechanical Engineering at **Tsinghua University**, supervised by Prof. [Zhaoye Qin](https://www.me.tsinghua.edu.cn/info/1127/1763.htm). My previous experiences include:

- *Apr 2025 - Sep 2025*, Visiting scholar at **Yale University** working with [Lu Lu](https://lugroup.yale.edu).
- *Apr 2022 - Sep 2022*, Research intern at **AIR, Tsinghua University**, supervised by [Yuanchun Li](https://air.tsinghua.edu.cn/info/1046/1195.htm).
- *Sep 2019 - Jun 2022*, M.Eng. in **Control Theory and Control Engineering** at Soochow University (SUDA), supervised by [Prof. Liang Chen](http://jdxy.suda.edu.cn/d1/f2/c14011a446962/page.htm) and [Prof. Changqing Shen](http://web.suda.edu.cn/cqshen/).
- *Sep 2015 - Jun 2019*, B.Eng. in **Electrical Engineering** at SUDA.

My research interests including **trustworthy AI**, **foundation model** and **reliable prognostic and health management (PHM)**. I have published numerous papers in top-tier international journals with total <a href='https://scholar.google.com/citations?user=vCabh8oAAAAJ'>google scholar citations <strong><span id='total_cit'>600+</span></strong></a>. Feel free to reach out for collaboration opportunities!

# 🔥 News
- *2025.04*: A paper accepted by Information fusion
- *2025.01*: A paper accepted by ADVEI
- *2025.01*: The 2024 CAST Youth Talent Support Program - PhD Special Plan - CCF
- *2024.12*: Science and Technology Award of Chinese Society of Vibration Engineering.
- *2024.11*: A paper accepted by JMS.
- *2024.02*: A paper accepted by IEEE TII.
- *2022.05*: Received the Future Scholars Scholarship from THU.


# 📝 Publications

## 🔖Neural-symbolic Diagnosis

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">ADVIE 2025</div>
      <img src='images/papers/TIFN.png' alt="Transparent information fusion network" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Transparent information fusion network: An explainable network for multi-source bearing fault diagnosis via self-organized neural-symbolic nodes](https://doi.org/10.1016/j.aei.2025.103156)  
**Qi Li**, Lichang Qin, Haifeng Xu, Qijian Lin, Zhaoye Qin, Fulei Chu  

- Introduces a transparent information fusion network with self-organized neural-symbolic nodes, enabling fully explainable multi-source fault diagnosis through knowledge-informed decision-making. *(JCR Q1, Impact Factor: 8.0)*  

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">JMS 2024</div>
      <img src='images/papers/DEN.png' alt="Deep Expert Network" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Deep Expert Network: A Unified Method toward Knowledge-Informed Fault Diagnosis via Fully Interpretable Neuro-Symbolic AI](https://doi.org/10.1016/j.jmsy.2024.10.007)  
**Qi Li**, Yuekai Liu, Shilin Sun, Zhaoye Qin, Fulei Chu  

- Proposes a neuro-symbolic AI approach to fault diagnosis incorporating interpretable expert knowledge using a Deep Expert Network. *(JCR Q1, Impact Factor: 12.2)*  

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">IEEE TII 2024</div>
      <img src='images/papers/TON.png' alt="Transparent Operator Network" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Transparent Operator Network: A Fully Interpretable Network Incorporating Learnable Wavelet Operator for Intelligent Fault Diagnosis](https://doi.org/10.1109/TII.2024.3366993)  
**Qi Li**, Hua Li, Wenyang Hu, Shilin Sun, Zhaoye Qin, Fulei Chu  

- This work introduces an interpretable method for industrial time series classification by integrating learnable wavelet operators. *(JCR Q1, Impact Factor: 12.3)*  

</div>
</div>

## 🔖 Cross-domain Diagnosis

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">RESS 2023</div>
      <img src='images/papers/CADA.png' alt="Cross-Domain Augmentation Diagnosis" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Cross-Domain Augmentation Diagnosis: An Adversarial Domain-Augmented Generalization Method for Fault Diagnosis under Unseen Working Conditions](https://doi.org/10.1016/j.ress.2023.109171)  
**Qi Li**, Liang Chen, Lin Kong, Dong Wang, Min Xia, Changqing Shen  

- This paper presents a domain generalization approach employing adversarial learning and data augmentation for robust industrial time series classification. *(JCR Q1, Impact Factor: 9.4)*  

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">IEEE TII 2022</div>
      <img src='images/papers/ADIG.jpg' alt="Adversarial Domain-Invariant Generalization" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Adversarial Domain-Invariant Generalization: A Generic Domain-Regressive Framework for Bearing Fault Diagnosis under Unseen Conditions](https://ieeexplore.ieee.org/document/9428592/)  
**Chen Liang**, **Qi Li**, Changqing Shen, Jun Zhu, Dong Wang, Min Xia  

- A generic domain-regressive framework for fault diagnosis using adversarial learning between feature extractors and domain classifiers, achieving robust diagnosis performance. *(JCR Q1, Impact Factor: 11.7, highly cited🌟)*  

</div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">MSSP 2021</div>
      <img src='images/papers/KMADA.jpg' alt="Knowledge Mapping-Based Adversarial Domain Adaptation" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[Knowledge Mapping-Based Adversarial Domain Adaptation: A Novel Fault Diagnosis Method with High Generalizability under Variable Working Conditions](https://doi.org/10.1016/j.ymssp.2020.107095)  
**Qi Li**, Changqing Shen, Liang Chen, Zhongkui Zhu  

- Introduces a domain adaptation strategy using adversarial learning for improved generalizability in fault diagnosis across variable conditions. *(JCR Q1, Impact Factor: 7.9, highly cited🌟)*  

</div>
</div>




## 🔖PHM foundation model

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Information Fusion 2025</div>
      <img src='images/papers/HSE.png' alt="HSE: A Plug-and-Play Module for Unified Fault Diagnosis Foundation Models" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

[HSE: A Plug-and-Play Module for Unified Fault Diagnosis Foundation Models]  
**Qi Li**, Bojian Chen, Qitong Chen, Xuan Li, Zhaoye Qin, Fulei Chu  

- Propose a novel Heterogeneous Signal Embedding (HSE) module that projects heterogeneous signals into a unified signal space, offering seamless integration with existing IFD architectures as a plug-and-play solution. *(JCR Q1, Impact Factor: 14.4)*  

</div>
</div>

# 🎖 Honors and Awards

- *2025*: The 2024 CAST Youth Talent Support Program - PhD Special Plan - CCF
- *2024*: Science and Technology Award of Chinese Society of Vibration Engineering
- *2023*: Social Practice Scholarship of Tsinghua University
- *2022*: Future Scholars Scholarship of Tsinghua University
- *2021*: National Scholarship by Ministry of Education of China
- *2021*: Outstanding Student Cadre of Jiangsu Province
- *2021*: Outstanding postgraduate cadre of Soochow University
- *2020*: National Scholarship by Ministry of Education of China
- *2020*: Outstanding postgraduate of Soochow University
- *2019*: Special Award of Graduate Academic Scholarship
- *2019*: Delivered a speech at the opening ceremony of SUDA as a graduate student representative
- *2019*: Outstanding graduate of Soochow University

# 📖 Educations

- *2025.04 - 2025.09*, Visiting scholar in Statistics and Data Science, Yale University, advisor: Lu Lu.
- *2022.09 - Present*, Ph.D. in Mechanical Engineering, Tsinghua University (THU), Supervisor: Prof. Zhaoye Qin
- *2019.09 - 2022.06*, M.E. in Control Theory and Control Engineering, Soochow University (SUDA), Supervisors: Prof. Liang Chen, Prof. Changqing Shen
- *2015.09 - 2019.06*, B.E. in Electrical Engineering, Soochow University (SUDA)

# 💬 Invited Talks

- *2024.04*, Beijing AI PhD Student Forum, Beijing, China (2w viewers)
- *2023.11*, PHM Conference, Hangzhou, Hangzhou, China
- *2023.04*, Tsinghua University Department of Mechanical Engineering PhD Student Forum
- *2020.07*, IEEE INDIN 2020, Warwick, UK
- *2018.07*, SDPC 2018, Xi'an, China

# 💻 Internships

- *Mar 2022 - Aug 2022*, Research Intern at Institute for AI Industry Research, Tsinghua University
  - Conducted a research project focused on AI-enabled time series analysis for battery monitoring.

# 🔧 Skills

- Language: CSC English test (104/130)
- Programming: Python, MATLAB, PyTorch, TensorFlow
- Hobby: Marathon, Positive Psychology, Workout

# 🖥 Journal Reviews

- *Information Fusion (IF)*
- *Advanced Engineering Informatics (AEI)*
- *IEEE Transactions on Industrial Informatics (TII)*
- *Mechanical Systems and Signal Processing (MSSP)*
- *IEEE Transactions on Industrial Electronics (TIE)*
- *IEEE Transactions on Instrumentation and Measurement (TIM)*
- *IEEE Transactions on Industrial Informatics (TII)*
- *Measurement*
- *Measurement Science and Technology (MST)*

# 💴 Horizontal project

- TODO after graduation.

# 🎙 Social Activities

- *2023*：Volunteer at the IFToMM International Conference on Rotordynamics
- *2019 - 2022*: Graduate monitor of the University of Mechanical and Electric Engineering, SUDA
- *2021*: Interview by Student Union of Soochow University [Link](https://mp.weixin.qq.com/s/zW07Tp2uh0CkHzmfCAVnqw)
- *2019*: Delivered a speech at the opening ceremony of SUDA as a graduate student representative [Link](https://mp.weixin.qq.com/s/HQSOWfekFaz2hYdh-4hvwA)

# 📫 Contact

## 🎈 Myself

- **Email**: liq22@mails.tsinghua.edu.cn
- **ORCID**: [https://orcid.org/0000-0001-7105-2818](https://orcid.org/0000-0001-7105-2818)
- **wechat**: 17777777
<!-- - [**Curriculum Vitae**] -->

## 👻 Friend Links
- [Haifeng Xu](https://xyyxhf.github.io)

# 👓 Qi Li | Last updated: 2025.4
