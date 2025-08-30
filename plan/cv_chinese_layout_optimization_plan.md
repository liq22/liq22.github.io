# 🎨 中文简历排版优化修改计划

基于当前cv_chinese.tex的问题分析和about.md的完整信息，制定以下全面的修改计划：

## 🚨 **当前问题分析**

### 技术问题
- **字体错误**: Fandol字体导致中文字符缺失警告，需要恢复Noto Sans CJK SC配置
- **排版问题**: 多处overfull/underfull hbox导致排版不美观
- **页面冗余**: 当前4页内容需要精简到2页
- **头像路径**: 需要使用cv/portrait_template.jpg替换当前头像

### 内容问题  
- **论文分类混乱**: 缺少主页式的三个清晰分类标识(🔖PHM foundation model, 🔖Neural-symbolic Diagnosis, 🔖Cross-domain Diagnosis) 从主页提炼一句话进行介绍
- **学习经历过详**: 本科硕士信息过于冗长，需要合并精简
- **重要内容缺失**: 缺少invited talks等关键学术活动
- **结构不够紧凑**: 信息分散，缺乏层次感

## 🛠️ **修改方案**

### **第一阶段：技术修复**

#### 1. 字体配置修复
```latex
% 恢复正确的中文字体配置，解决字符缺失问题
\setCJKmainfont{Noto Sans CJK SC}
\setCJKsansfont{Noto Sans CJK SC}  
\setCJKmonofont{Noto Sans Mono CJK SC}
```

#### 2. 头像更换
- **当前路径**: `../images/LQ.png`
- **更换为**: `cv/portrait_template.jpg`
- 调整圆形头像尺寸和位置以适应新图片

### **第二阶段：内容结构重组**

#### **论文分类重新设计** (按about.md的三个分类)

**🔖 PHM Foundation Model**
- HSE: 用于统一故障诊断的即插即用模块 *(Information Fusion 2025, IF=14.4)*

**🔖 Neural-Symbolic Diagnosis**  
- 透明信息融合网络：基于自组织神经符号节点的多源轴承故障诊断 *(ADVEI 2025, IF=8.0)*
- 深度专家网络：知识驱动故障诊断的神经符号AI统一方法 *(JMS 2024, IF=12.2)* 
- 透明算子网络：融合可学习小波算子的智能故障诊断 *(IEEE TII 2024, IF=12.3)*

**🔖 Cross-Domain Diagnosis**
- 跨域增强诊断：未见工况下故障诊断的对抗域增强泛化方法 *(RESS 2023, IF=9.4)*
- 对抗域不变泛化：轴承故障诊断的通用域回归框架 *(IEEE TII 2022, IF=11.7, 高被引🌟)*
- 知识映射对抗域适应：变工况故障诊断的高泛化性方法 *(MSSP 2021, IF=7.9, 高被引🌟)*

#### **学习经历精简合并**

**当前问题**: 清华大学、耶鲁大学、苏州大学硕士、苏州大学本科、瑞安十中分别占用大量篇幅

**精简方案**:
```
📚 博士研究 (2022-2026)
清华大学 机械工程博士 | 导师: 秦朝烨教授
• 研究方向: 可信AI、基础模型、故障诊断  
• 学术成果: 8+篇JCR Q1论文，700+引用
• 访问经历: 耶鲁大学统计与数据科学系 (2025.4-9) | 导师: Lu Lu教授

📚 硕士研究 (2019-2022)  
苏州大学 控制理论与控制工程硕士 | 导师: 陈亮、沈长青教授
• 研究重点: 故障诊断的域适应方法 | 3篇ESI高被引论文
• 荣誉: 优秀毕业生、国家奖学金、开学典礼研究生代表

📚 本科学习 (2015-2019)
苏州大学 电气工程及其自动化学士 | 优秀毕业生
```

### **第三阶段：新增重要内容**

#### **受邀学术报告** (添加到第2页侧边栏)
```
🎤 受邀学术报告
• 2024年4月：北京AI博士生论坛，北京（观众2万人）
• 2023年11月：PHM学术会议，杭州
• 2023年4月：清华大学机械工程系博士生论坛
• 2020年7月：IEEE INDIN 2020，英国华威（线上）
• 2018年7月：SDPC 2018，西安
```

#### **研究经历** (添加到第1页右侧)
基于about.md信息补充：
```
🔬 研究经历

耶鲁大学统计与数据科学系 | 访问学者 | 2025年4月-9月
• 导师：Lu Lu 教授 | 研究方向：物理信息神经网络、基础模型研究

清华大学人工智能研究院 | 研究实习生 | 2022年4月-9月  
• 导师：李远春 教授 | AI时间序列分析、工业应用机器学习算法

清华大学机械工程系 | 博士研究助理 | 2022年9月-至今
• 导师：秦朝烨 教授 | 可信AI与基础模型研究、主导8+篇JCR Q1期刊论文
```

### **第四阶段：页面布局优化**

#### **2页布局重新设计**

**第1页布局**:
```
左侧栏 (40%):
├── 个人信息 + 头像 (portrait_template.jpg)
├── 研究领域 (可信AI、基础模型、智能监测诊断)
├── 核心技能 (编程、工具、语言等)
└── 主要荣誉 (精选6-8项最重要的)

右侧栏 (60%):
├── 研究经历 (新增，3个主要研究经历)
└── 学习经历 (精简版，3个学历层次)
```

**第2页布局**:
```
左侧栏 (40%):
├── 姓名重复
├── 完整荣誉奖项 (按年份倒序)
├── 受邀学术报告 (新增，5场重要报告)
├── 学术服务 (期刊审稿人)
└── 项目应用 + 社会活动

右侧栏 (60%):
└── 代表性学术论文 (三分类，每类2-3篇代表作)
```

## 🎯 **排版美化细节**

### **视觉优化**
- **分类标识**: 增加emoji图标 (🔖, 📚, 🎤, 🔬)
- **间距调整**: 修复overfull/underfull hbox问题
- **字体层次**: 统一使用中文字体，避免字符缺失
- **颜色搭配**: 保持清华紫主题色彩

### **内容凝练原则**
- **50%压缩**: 学习经历篇幅减少一半
- **重点突出**: 强调最新成果和重要荣誉
- **信息完整**: 保留所有关键学术信息
- **逻辑清晰**: 按时间和重要性排序

## 📋 **具体执行步骤**

### **步骤1: 技术修复**
- [ ] 恢复setCJKmainfont等字体配置
- [ ] 更换头像为portrait_template.jpg
- [ ] 测试编译，确保中文显示正常

### **步骤2: 内容重构** 
- [ ] 重写论文部分，按三个分类重新组织
- [ ] 精简学习经历，合并相关信息
- [ ] 添加研究经历和受邀报告部分

### **步骤3: 布局调整**
- [ ] 重新设计2页布局结构
- [ ] 调整minipage尺寸和spacing
- [ ] 优化表格和列表格式

### **步骤4: 排版优化**
- [ ] 解决overfull/underfull hbox警告
- [ ] 统一字体大小和行距
- [ ] 测试最终PDF输出效果

## ⚡ **预期修改效果**

### **修改前问题**
- ❌ 字体错误导致中文字符缺失
- ❌ 4页冗长布局
- ❌ 论文分类不清晰
- ❌ 学习经历过于详细
- ❌ 缺少重要学术活动

### **修改后效果**  
- ✅ 完美的中文字体显示
- ✅ 精简的2页专业布局
- ✅ 清晰的三分类论文展示 (🔖标识)
- ✅ 凝练而完整的学术经历
- ✅ 全面的学术活动展示
- ✅ 与主页风格一致的专业简历
- ✅ 无编译错误的完美输出

## 🔄 **质量保证**

- **编译测试**: 确保0个LaTeX错误
- **字体验证**: 所有中文字符正确显示
- **内容核查**: 与about.md信息完全一致
- **排版检查**: 无overfull/underfull警告
- **视觉效果**: 专业美观的PDF输出



[1]	Q. Li, Y. Liu, S. Sun, Z. Qin, and F. Chu, “Deep expert network: A unified method toward knowledge-informed fault diagnosis via fully interpretable neuro-symbolic AI,” J. Manuf. Syst., vol. 77, pp. 652–661, Dec. 2024, doi: 10.1016/j.jmsy.2024.10.007. (中科院一区TOP，Impact Factor: 12.2)
[2]	Q. Li, H. Li, W. Hu, S. Sun, Z. Qin, and F. Chu, “Transparent Operator Network: A Fully Interpretable Network Incorporating Learnable Wavelet Operator for Intelligent Fault Diagnosis,” IEEE Trans. Ind. Inf., pp. 1–11, 2024, doi: 10.1109/TII.2024.3366993. (中科院一区TOP, Impact Factor: 11.7) 
[3]	Q. Li, L. Chen, L. Kong, D. Wang, M. Xia, and C. Shen, “Cross-domain augmentation diagnosis: An adversarial domain-augmented generalization method for fault diagnosis under unseen working conditions,” Reliab Eng Syst Saf, vol. 234, p. 109171, Jun. 2023, doi: 10.1016/j.ress.2023.109171. (中科院一区TOP, Impact Factor: 9.4, ESI 高被引论文,被引51次)
[4]	L. Chen (导师), Q. Li, C. Shen et al. “Adversarial domain-invariant generalization: a generic domain-regressive framework for bearing fault diagnosis under unseen conditions,” IEEE Trans. Ind. Informatics, 2021. (中科院一区TOP, Impact Factor: 11.7, ESI 高被引论文,被引135次)
[5]	Q. Li, C. Shen, L. Chen, et al. “Knowledge mapping-based adversarial domain adaptation: A novel fault diagnosis method with high generalizability under variable working conditions,” Mech. Syst. Signal Process., vol. 147, 2021. (中科院一区TOP, Impact Factor: 8.6, ESI 高被引论文,被引130次)


---
*计划创建时间：2025年8月*  
*状态：待用户确认*  
*预计修改时间：30-45分钟*