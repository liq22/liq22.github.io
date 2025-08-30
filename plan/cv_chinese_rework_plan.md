# 中文学术简历改版计划（cv/cv_chinese.tex）

> 目标：精简为优雅的 2 页版式，突出三大研究「package」，合并本硕教育经历，加入 Invited Talks，更新头像为 `cv/portait_template.jpg`。

## 成果目标
- 页面控制：不超过 2 页；移除冗余或重复侧栏/空白页。
- 头像更新：替换为 `cv/portait_template.jpg`，圆形裁剪、与侧栏对齐。
- 学习经历：合并苏州大学本硕为一条目，表述更凝练；保留清华博士、耶鲁访问。
- 代表性学术论文：按三大 package 分组展示，并在每组前加入「🔖」标签：
  - 🔖 PHM Foundation Model（基础模型）
  - 🔖 Neural‑symbolic Diagnosis（可解释/神经符号）
  - 🔖 Cross‑domain Diagnosis（跨域/泛化）
- 新增「受邀报告」区块（Invited Talks），内容精炼为 3–5 条。

## 版式与技术改动
- 侧栏策略：仅在第 1 页保留紫色侧栏；第 2 页使用全宽主内容，删除重复的侧栏与姓名块。
- 段落/列表收紧：引入 `enumitem`，统一 `itemsep=1pt, topsep=1pt, parsep=0pt`；标题与段前后距用 `titlesec` 进一步压缩。
- Package 标签：实现一个轻量标签命令 `\packagetag{...}`，默认渲染为 `\faBookmark` 或直接字符 `🔖`（以 XeLaTeX/Noto 渲染为准，若emoji不稳定则回退到 FontAwesome 书签图标）。
- 论文分组呈现：采用三行卡片式布局（`tabularx`/`minipage`），每组 3 行主代表作 。
- 清理空白页：移除强制分页与重复 `minipage` 侧栏；检查 `\vfill` 与固定高度设置，避免撑出多余页。

## 内容调整草案（供确认）
- 学习经历（精简）
  - 清华大学｜机械工程博士（2022–今）— 导师：秦朝烨；方向：智能监测诊断/可信AI；代表成果与奖项保留 2–3 点。
  - 耶鲁大学｜访问学者（2025.04–2025.09）— 导师：Lu Lu；方向：PINN/统计与数据科学（1–2 点）。
  - 苏州大学｜本硕（2015–2022）— 硕士：控制理论与控制工程；学士：电气工程及其自动化；获江苏省优毕、国家奖学金（合并为 2–3 点）。

- 代表性论文（建议分配）
  - 🔖 Neural‑symbolic Diagnosis：DEN（JMS 2024）、TON（IEEE TII 2024）
  - 🔖 Cross‑domain Diagnosis：CADA（RESS 2023）、ADIG（IEEE TII 2022）、KMADA（MSSP 2021）
  - 🔖 PHM Foundation Model：HSE / 透明算子/其他基础模块类工作（如有，选 1–2 篇放此组）

- 受邀报告（示例占位，待您最终确认）
  - Beijing AI PhD Forum（2024）
  - PHM Conference, Hangzhou（2023）
  - IEEE INDIN（2020, Warwick）
  - SDPC（2018, Xi’an）

## 实施步骤（待您确认后执行）
1) 更新头像路径与裁剪；只保留第 1 页侧栏。
2) 合并本硕教育经历，精简要点与行距。
3) 新增 `\packagetag` 并重构「代表性学术论文」为三组包。
4) 加入「受邀报告」区块，统一列表样式与间距。
5) 收紧全局标题/列表间距，去除多余 `\newpage`/`\vfill`/重复侧栏。
6) 编译验证页数≤2，微调字距与断行，确保观感整洁。

## 需要您确认的点
- 论文分组是否按上面三类归并；是否需要调整代表作顺序。
- 受邀报告最终清单（可直接在此文件补充/修改）。
- 是否保留高中经历；若压缩空间，建议删除。
- 页数上限为 2 页是否合适（或希望 1 页版/2 页精排版）。

—— 确认后，我将按以上步骤修改 `cv/cv_chinese.tex` 并提交变更。
