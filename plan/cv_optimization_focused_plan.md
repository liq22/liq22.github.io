# CV简历专项优化方案

## 📋 项目概述
专门针对李奇的中英文学术简历(LaTeX)进行优化，提升视觉效果和信息准确性。**主页保持原有头像`images/LQ.png`不变**，仅优化CV文档。

## 🎯 优化目标
1. **CV头像更新**: CV使用新头像 `cv/portait.jpg`（主页不变）
2. **二维码集成**: CV中添加个人主页二维码展示
3. **内容重构**: 合并研究经历和学习经历为统一部分
4. **视觉美化**: 为CV各部分添加FontAwesome图标
5. **信息修正**: 修正"陈亮"为"陈良"
6. **文献更新**: 更新最新一作文献列表

## 📄 CV文件专项修改

### 1. 中文简历 (`cv/cv_chinese.tex`) 详细修改

#### 1.1 头像路径更新（第107-113行）
```latex
% 更新头像引用，使用CV目录下的新头像
\IfFileExists{portait.jpg}{
\begin{center}
    \begin{tikzpicture}
    \clip (0,0) circle (3cm) node[anchor=center] {\includegraphics[width=6cm]{portait.jpg}}; 
    \end{tikzpicture}
\end{center}
}{}
```

#### 1.2 个人信息区域添加二维码（第116-128行后）
```latex
\vspace{.3cm}
% 添加个人主页二维码
\begin{center}
    \textbf{\small 个人主页}\\
    \vspace{.2cm}
    \IfFileExists{QRcode.png}{
        \includegraphics[width=2.5cm]{QRcode.png}
    }{}\\
    {\tiny 扫码访问主页}
\end{center}
\vspace{.3cm}
```

#### 1.3 研究领域部分图标化（第134-141行）
```latex
\section*{\large 🧠 研究领域}
\begin{tabular}{cl}
    \faAtom{}       & 可信人工智能 \\
    \faCogs{}       & 基础模型 \\
    \faWrench{}     & 智能监测诊断技术 \\
\end{tabular}
```

#### 1.4 核心技能部分图标化（第146-156行）
```latex
\section*{\large 💻 核心技能}
\begin{tabularx}{\textwidth}{cY}
    \faCode{}        & Python, MATLAB, PyTorch \\
    \faMicrochip{}   & TensorFlow, Scikit-learn \\
    \faFileAlt{}     & LaTeX, 英文学术写作 \\
    \faLanguage{}    & 中文(母语), 英文(优秀) \\
    \faDesktop{}     & Linux, Windows, HPC集群 \\
    \faLaptopCode{}  & Jupyter, VS Code, PyCharm \\
\end{tabularx}
```

#### 1.5 主要荣誉部分图标化（第161-171行）
```latex
\section*{\large 🏆 主要荣誉}
\begin{tabularx}{\textwidth}{cY}
    \faTrophy{} & 2024 首批科协青年托举人才（博士） \\
    \faAward{}  & 2024 振动工程协会科学技术二等奖 \\
    \faMedal{}  & 2023 清华大学社会实践奖学金 \\
    \faStar{}   & 2022 清华大学未来学者奖学金 \\
    \faCrown{}  & 2021 国家奖学金 \\
    \faCrown{}  & 2020 国家奖学金 \\
\end{tabularx}
```

#### 1.6 教育与研究经历合并重构（第181-225行）
```latex
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% 🎓 教育与研究经历
\phantomsection{}
\addcontentsline{toc}{section}{教育与研究经历}
\section*{\scshape\Large 🎓 教育与研究经历 \rule{\linewidth}{0.4pt}}

% 🔬 当前博士阶段（2022-至今）
{\large \textbf{🔬 博士研究阶段 (2022年9月-至今)}} \\
{{\fontseries{medium}\selectfont \faUniversity{} 清华大学 机械工程博士}} \\
{\scshape\fontseries{light}\selectfont\footnotesize 导师: 秦朝烨教授 | 研究方向: 可信AI、基础模型、故障诊断} \\
{\scshape\fontseries{light}\selectfont\footnotesize 学术成果: 8+篇JCR Q1论文，700+引用 | 未来学者奖学金} \\[1ex]

% 📚 访问学者经历
{\large \textbf{📚 访问学者经历}} \\
• \faGlobe{} \textbf{耶鲁大学统计与数据科学系} (2025年4月-2025年9月) \\
  导师：Lu Lu 教授 | 研究：物理信息神经网络、基础模型 \\[0.5ex]
• \faFlask{} \textbf{清华大学人工智能研究院} (2022年4月-2022年9月) \\
  导师：李远春 教授 | 研究：AI时间序列分析、工业机器学习 \\[1ex]

% 🎓 硕士研究阶段（2019-2022）
{\large \textbf{🎓 硕士研究阶段 (2019年9月-2022年6月)}} \\
{{\fontseries{medium}\selectfont \faUniversity{} 苏州大学 控制理论与控制工程硕士}} \\
{\scshape\fontseries{light}\selectfont\footnotesize 导师: 陈良教授、沈长青教授 | 研究重点: 故障诊断域适应方法} \\
{\scshape\fontseries{light}\selectfont\footnotesize 成果: 3篇ESI高被引论文 | 优秀毕业生 | 国家奖学金} \\[1ex]

% 🎓 本科学习阶段（2015-2019）
{\large \textbf{🎓 本科学习阶段 (2015年9月-2019年6月)}} \\
{{\fontseries{medium}\selectfont \faUniversity{} 苏州大学 电气工程及其自动化学士}} \\
{\scshape\fontseries{light}\selectfont\footnotesize 优秀毕业生 | 开学典礼新生代表发言人} \\[2ex]
```

#### 1.7 姓名修正
- **第220行**: 修正为 `导师: 陈良教授、沈长青教授`
- **第275行**: 修正为 `L. Chen (陈良), \textbf{Q. Li}, C. Shen et al.`

#### 1.8 最新文献列表更新（第269-282行）
```latex
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% 🔖 最新学术论文
\phantomsection
\addcontentsline{toc}{section}{最新学术论文}
\section*{\scshape\Large 📚 最新学术论文 \rule{\linewidth}{0.4pt}}
\begin{justify}
\setlength{\parindent}{0pt}
\footnotesize

% 2025年最新成果
[1] \textbf{Q. Li}, B. Chen, Q. Chen, X. Li, Z. Qin, and F. Chu, "HSE: A Plug-and-Play Module for Unified Fault Diagnosis Foundation Models," \textit{Information Fusion}, 2025. (中科院一区TOP，IF: 14.4) \\[0.5ex]

[2] \textbf{Q. Li}, L. Qin, H. Xu, Q. Lin, Z. Qin, and F. Chu, "Transparent information fusion network: An explainable network for multi-source bearing fault diagnosis via self-organized neural-symbolic nodes," \textit{Advanced Engineering Informatics}, 2025. (JCR Q1, IF: 8.0) \\[0.5ex]

% 2024年核心成果
[3] \textbf{Q. Li}, Y. Liu, S. Sun, Z. Qin, and F. Chu, "Deep expert network: A unified method toward knowledge-informed fault diagnosis via fully interpretable neuro-symbolic AI," \textit{J. Manuf. Syst.}, vol. 77, pp. 652–661, Dec. 2024. (中科院一区TOP，IF: 12.2) \\[0.5ex]

[4] \textbf{Q. Li}, H. Li, W. Hu, S. Sun, Z. Qin, and F. Chu, "Transparent Operator Network: A Fully Interpretable Network Incorporating Learnable Wavelet Operator for Intelligent Fault Diagnosis," \textit{IEEE Trans. Ind. Inf.}, 2024. (中科院一区TOP, IF: 12.3) \\[0.5ex]

% 高被引重点论文
[5] \textbf{Q. Li}, L. Chen, L. Kong, D. Wang, M. Xia, and C. Shen, "Cross-domain augmentation diagnosis: An adversarial domain-augmented generalization method for fault diagnosis under unseen working conditions," \textit{Reliab Eng Syst Saf}, vol. 234, p. 109171, 2023. (中科院一区TOP, IF: 9.4, ESI高被引🌟，被引51次) \\[0.5ex]

[6] 陈良 (导师), \textbf{Q. Li}, C. Shen et al. "Adversarial domain-invariant generalization: a generic domain-regressive framework for bearing fault diagnosis under unseen conditions," \textit{IEEE Trans. Ind. Informatics}, 2021. (中科院一区TOP, IF: 11.7, ESI高被引🌟，被引135次) \\[0.5ex]

[7] \textbf{Q. Li}, C. Shen, 陈良, et al. "Knowledge mapping-based adversarial domain adaptation: A novel fault diagnosis method with high generalizability under variable working conditions," \textit{Mech. Syst. Signal Process.}, vol. 147, 2021. (中科院一区TOP, IF: 8.6, ESI高被引🌟，被引130次) \\[0.5ex]
\end{justify}
```

#### 1.9 侧边栏优化（第294-378行）
为受邀学术报告、学术服务、项目应用、社会活动等部分添加相应图标：

```latex
% 🎤 受邀学术报告
\section*{\large 🎤 受邀学术报告}
\begin{tabularx}{\textwidth}{cY}
    \faMicrophone{} & 2024.04 北京AI博士生论坛，北京（观众2万人） \\
    \faChalkboardTeacher{} & 2023.11 PHM学术会议，杭州 \\
    \faUniversity{} & 2023.04 清华大学机械工程系博士生论坛 \\
    \faGlobe{} & 2020.07 IEEE INDIN 2020，英国华威（线上） \\
    \faMapMarkerAlt{} & 2018.07 SDPC 2018，西安 \\
\end{tabularx}

% 📝 学术服务  
\section*{\large 📝 学术服务}
\begin{tabularx}{\textwidth}{cY}
    \faJournalWhills{} & Information Fusion (IF: 14.4) \\
    \faJournalWhills{} & IEEE TII, MSSP \\
    \faJournalWhills{} & Advanced Engineering Informatics \\
    \faJournalWhills{} & IEEE TIE, IEEE TIM \\
    \faJournalWhills{} & Measurement, MST \\
\end{tabularx}

% 🚀 项目应用
\section*{\large 🚀 项目应用}
\begin{tabularx}{\textwidth}{cY}
    \faPlane{}      & 某型号飞机减振降噪分析 \\
    \faBolt{}       & 水电站智能运维技术 \\
    \faGithub{}     & PHMBench开源项目组负责人 \\
\end{tabularx}

% 🤝 社会活动
\section*{\large 🤝 社会活动}
\begin{tabularx}{\textwidth}{cY}
    \faMicrophone{}  & 苏大开学典礼新生代表发言 \\
    \faUserTie{}     & 苏大机电学院研究生班长 \\
    \faHandsHelping{} & IFToMM会议志愿者 \\
\end{tabularx}
```

### 2. 英文简历 (`cv/cv_english.tex`) 对应修改

#### 2.1 头像路径更新（第120-126行）
```latex
% 使用CV目录下的新头像，注意相对路径
\IfFileExists{portait.jpg}{
\begin{center}
    \begin{tikzpicture}
    \clip (0,0) circle (3cm) node[anchor=center] {\includegraphics[width=6cm]{portait.jpg}}; 
    \end{tikzpicture}
\end{center}
}{}
```

#### 2.2 个人信息区域添加二维码
在个人信息部分后添加二维码展示区域。

#### 2.3 教育与研究经历合并
将Research Experience（第186-231行）和Education（第234-257行）合并为统一的"Education & Research Experience"部分。

#### 2.4 姓名修正
确保所有"Liang Chen"的引用统一为"Chen Liang"或保持一致性。

## 📋 实施步骤

### Phase 1: 文件备份与准备
1. 备份原始CV文件
2. 验证图片文件存在性
3. 准备LaTeX编译环境

### Phase 2: 中文简历优化
1. 更新头像引用路径
2. 添加个人主页二维码
3. 为各部分添加图标装饰  
4. 合并教育与研究经历
5. 修正姓名错误
6. 更新最新文献列表

### Phase 3: 英文简历同步优化
1. 应用与中文简历相同的修改
2. 确保英文表述准确
3. 保持两版本内容一致性

### Phase 4: 编译与测试
1. XeLaTeX编译中文简历
2. LaTeX编译英文简历
3. 检查PDF生成效果
4. 验证图标和图片显示

### Phase 5: 质量检查
1. 检查所有姓名修正
2. 验证文献引用准确性
3. 确认图标显示正常
4. 对比原版确认改进效果

## ⚠️ 重要说明
- **主页不变**: Jekyll网站保持使用 `images/LQ.png` 作为头像
- **CV专用**: 仅CV文档使用 `cv/portait.jpg` 新头像
- **字体依赖**: 确保系统安装FontAwesome字体以正确显示图标
- **编译环境**: 推荐使用XeLaTeX编译中文简历以支持中文字体

## 🎯 预期效果
- ✅ CV使用新头像，视觉更加专业
- ✅ 二维码方便访问个人主页
- ✅ 图标装饰提升整体美观度
- ✅ 内容结构更加清晰合理
- ✅ 信息准确性大幅提升
- ✅ 展示最新学术成果

---
**创建时间**: 2025-08-30  
**专项范围**: CV简历文档优化  
**预计时间**: 30-40分钟  
**主页影响**: 无（保持原状）