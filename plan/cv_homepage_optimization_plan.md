# CV简历优化方案

## 📋 项目概述
对李奇的中英文学术简历进行全面优化，提升视觉效果和信息准确性。主页保持原有头像，CV使用新头像。

## 🎯 优化目标
1. **CV头像更新**: 使用 `cv/portait.jpg` 作为CV专用头像（主页保持原头像不变）
2. **二维码集成**: 在CV中添加个人主页二维码 `cv/QRcode.png`
3. **内容重构**: 合并CV中的研究经历和学习经历部分
4. **视觉提升**: 为CV各段落添加相关图标
5. **信息修正**: 将"陈亮"更正为"陈良"
6. **文献更新**: 根据最新学术成果更新一作文献列表

## 📁 CV文件修改清单

### 1. 头像和二维码处理
- CV使用 `cv/portait.jpg`（无需复制，直接在CV目录使用）
- CV中集成 `cv/QRcode.png` 展示个人主页二维码
- **主页保持** `images/LQ.png` 不变

#### 2.2 教育与研究经历合并
将现有的第201-206行（教育背景）和第23-26行（研究经历）合并为：

```markdown
# 🎓 教育与研究经历

## 🔬 研究经历
- *2025.04 - 2025.09* 📚 **耶鲁大学统计与数据科学系** - 访问学者  
  导师：Lu Lu 教授 | 研究：物理信息神经网络、基础模型

- *2022.04 - 2022.09* 🔬 **清华大学人工智能研究院** - 研究实习生  
  导师：李远春 教授 | 研究：AI时间序列分析、工业机器学习

- *2022.09 - 至今* 🎯 **清华大学机械工程系** - 博士研究助理  
  导师：秦朝烨 教授 | 研究：可信AI与基础模型、8+篇JCR Q1论文

## 🎓 学历背景  
- *2022.09 - 至今* 🎓 **清华大学** 机械工程博士  
  导师：秦朝烨教授 | GPA: xx/xx | 研究方向：可信AI、基础模型、PHM

- *2019.09 - 2022.06* 🎓 **苏州大学** 控制理论与控制工程硕士  
  导师：陈良教授、沈长青教授 | 优秀毕业生、国家奖学金

- *2015.09 - 2019.06* 🎓 **苏州大学** 电气工程及其自动化学士  
  优秀毕业生、开学典礼研究生代表发言
```

#### 2.3 联系方式添加二维码
在第251-257行的联系方式部分添加：

```markdown
# 📫 Contact

## 🎈 Myself
- **Email**: liq22@mails.tsinghua.edu.cn  
- **ORCID**: [0000-0001-7105-2818](https://orcid.org/0000-0001-7105-2818)
- **个人主页**: 
  <div align="center">
    <img src="images/QRcode.png" alt="个人主页二维码" width="150"/>
    <br>
    <small>扫码访问个人主页</small>
  </div>
```

### 3. 中文简历优化 (`cv/cv_chinese.tex`)

#### 3.1 头像路径更新
修改第107-113行：
```latex
% 更新头像引用
\IfFileExists{portait.jpg}{
\begin{center}
    \begin{tikzpicture}
    \clip (0,0) circle (3cm) node[anchor=center] {\includegraphics[width=6cm]{portait.jpg}}; 
    \end{tikzpicture}
\end{center}
}{}
```

#### 3.2 研究与学习经历合并
将第181-225行重构为：

```latex
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% 教育与研究经历
\phantomsection{}
\addcontentsline{toc}{section}{教育与研究经历}
\section*{\scshape\Large 🎓 教育与研究经历 \rule{\linewidth}{0.4pt}}

% 博士阶段
{\large \textbf{🎓 博士研究 (2022-至今)}} \\
{{\fontseries{medium}\selectfont 清华大学 机械工程博士 | 导师: 秦朝烨教授}} \\
{\scshape\fontseries{light}\selectfont\footnotesize 研究方向: 可信AI、基础模型、故障诊断 | 学术成果: 8+篇JCR Q1论文，700+引用} \\[1ex]

% 研究经历
{\large \textbf{🔬 主要研究经历}} \\
• \textbf{耶鲁大学统计与数据科学系} (2025.04-2025.09) - 访问学者 \\
  导师：Lu Lu 教授 | 物理信息神经网络、基础模型研究 \\[0.5ex]
• \textbf{清华大学人工智能研究院} (2022.04-2022.09) - 研究实习生 \\
  导师：李远春 教授 | AI时间序列分析、工业应用机器学习算法 \\[1ex]

% 硕士阶段  
{\large \textbf{🎓 硕士研究 (2019-2022)}} \\
{{\fontseries{medium}\selectfont 苏州大学 控制理论与控制工程硕士 | 导师: 陈良、沈长青教授}} \\
{\scshape\fontseries{light}\selectfont\footnotesize 研究重点: 故障诊断域适应方法 | 3篇ESI高被引论文 | 优秀毕业生、国家奖学金} \\[1ex]

% 本科阶段
{\large \textbf{🎓 本科学习 (2015-2019)}} \\
{{\fontseries{medium}\selectfont 苏州大学 电气工程及其自动化学士 | 优秀毕业生、开学典礼研究生代表发言}} \\[2ex]
```

#### 3.3 名称修正
- 第220行：`导师: 陈良、沈长青教授` (修正"陈亮"→"陈良")
- 第275行：`L. Chen (陈良)` (修正导师姓名)

#### 3.4 侧边栏增加图标
为第135-171行的各个部分添加图标：

```latex
% 研究领域
\section*{\large 🧠 研究领域}
\begin{tabular}{cl}
    \faBrain{}      & 可信人工智能 \\
    \faCogs{}       & 基础模型 \\
    \faTools{}      & 智能监测诊断技术 \\
\end{tabular}

% 核心技能  
\section*{\large 💻 核心技能}
\begin{tabularx}{\textwidth}{cY}
    \faCode{}        & Python, MATLAB, PyTorch \\
    \faPen*{}        & TensorFlow, Scikit-learn \\
    \faFont{}        & LaTeX, 英文学术写作 \\
    \faLanguage{}    & 中文(母语), 英文(优秀) \\
    \faDesktop{}     & Linux, Windows, HPC集群 \\
    \faLaptopCode{}  & Jupyter, VS Code, PyCharm \\
\end{tabularx}

% 主要荣誉
\section*{\large 🏆 主要荣誉}
```

### 4. 英文简历优化 (`cv/cv_english.tex`)

#### 4.1 头像路径更新
修改第120-126行：
```latex
\IfFileExists{../images/portait.jpg}{
\begin{center}
    \begin{tikzpicture}
    \clip (0,0) circle (3cm) node[anchor=center] {\includegraphics[width=6cm]{../images/portait.jpg}}; 
    \end{tikzpicture}
\end{center}
}{}
```

#### 4.2 教育与研究经历整合
将第186-257行重构，合并Research Experience和Education部分。

#### 4.3 名称修正
修正所有"Liang Chen"的引用，确保一致性。

### 5. 最新文献列表更新

#### 5.1 一作文献（按时间倒序）
```latex
% 2025年文献
[1] \textbf{Q. Li}, B. Chen, Q. Chen, X. Li, Z. Qin, and F. Chu, "HSE: A Plug-and-Play Module for Unified Fault Diagnosis Foundation Models," \textit{Information Fusion}, 2025. (JCR Q1, IF: 14.4)

[2] \textbf{Q. Li}, L. Qin, H. Xu, Q. Lin, Z. Qin, and F. Chu, "Transparent information fusion network: An explainable network for multi-source bearing fault diagnosis via self-organized neural-symbolic nodes," \textit{Advanced Engineering Informatics}, 2025. (JCR Q1, IF: 8.0)

% 2024年文献
[3] \textbf{Q. Li}, Y. Liu, S. Sun, Z. Qin, and F. Chu, "Deep expert network: A unified method toward knowledge-informed fault diagnosis via fully interpretable neuro-symbolic AI," \textit{J. Manuf. Syst.}, vol. 77, pp. 652–661, Dec. 2024. (JCR Q1, IF: 12.2)

[4] \textbf{Q. Li}, H. Li, W. Hu, S. Sun, Z. Qin, and F. Chu, "Transparent Operator Network: A Fully Interpretable Network Incorporating Learnable Wavelet Operator for Intelligent Fault Diagnosis," \textit{IEEE Trans. Ind. Inf.}, 2024. (JCR Q1, IF: 12.3)

% 2023年文献
[5] \textbf{Q. Li}, L. Chen, L. Kong, D. Wang, M. Xia, and C. Shen, "Cross-domain augmentation diagnosis: An adversarial domain-augmented generalization method for fault diagnosis under unseen working conditions," \textit{Reliab Eng Syst Saf}, vol. 234, p. 109171, 2023. (JCR Q1, IF: 9.4, 高被引🌟)

% 早期重要文献
[6] \textbf{Q. Li}, C. Shen, L. Chen, et al. "Knowledge mapping-based adversarial domain adaptation: A novel fault diagnosis method with high generalizability under variable working conditions," \textit{Mech. Syst. Signal Process.}, vol. 147, 2021. (JCR Q1, IF: 8.6, 高被引🌟)
```

## 📋 实施步骤

### Phase 1: 文件准备
1. 备份原始文件
2. 复制图片文件到正确位置
3. 验证文件路径

### Phase 2: Jekyll网站更新
1. 更新配置文件
2. 修改about.md页面
3. 测试本地构建

### Phase 3: 简历文档更新
1. 修改中文简历模板
2. 修改英文简历模板  
3. 编译测试PDF生成

### Phase 4: 内容验证
1. 检查所有名称修正
2. 验证文献引用准确性
3. 确认图标显示正常

### Phase 5: 最终测试
1. Jekyll网站构建测试
2. LaTeX编译测试
3. 跨平台显示验证

## ⚠️ 注意事项
- 保持所有平台信息的一致性
- 确保图片文件路径正确
- 验证LaTeX编译无错误
- 检查Jekyll构建成功

## 🎯 预期效果
- 统一美观的视觉形象
- 更直观的联系方式展示
- 清晰的学术经历展示
- 准确的个人信息
- 最新的学术成果展示

---
*创建时间: 2025-08-30*  
*预计完成时间: 45-60分钟*