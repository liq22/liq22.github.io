
<h1 align="center">
Qi Li - Personal Academic Homepage
</h1>

<div align="center">

[![](https://img.shields.io/github/stars/RayeRen/acad-homepage.github.io)](https://github.com/RayeRen/acad-homepage.github.io)
[![](https://img.shields.io/github/forks/RayeRen/acad-homepage.github.io)](https://github.com/RayeRen/acad-homepage.github.io)
[![](https://img.shields.io/github/issues/RayeRen/acad-homepage.github.io)](https://github.com/RayeRen/acad-homepage.github.io)
[![](https://img.shields.io/github/license/RayeRen/acad-homepage.github.io)](https://github.com/RayeRen/acad-homepage.github.io/blob/main/LICENSE)  | [中文文档](./docs/README-zh.md) 
</div>

<p align="center">Ph.D. Student in Mechanical Engineering at Tsinghua University<br>Research Focus: Trustworthy AI, Foundation Models, and Reliable PHM</p>

<p align="center">
    <br>
    <img src="docs/screenshot.png" width="100%"/>
    <br>
</p>

🏠 **Homepage**: [https://liq22.github.io](https://liq22.github.io)

📧 **Contact**: liq22@mails.tsinghua.edu.cn | 🎓 **Google Scholar**: [Citations 600+](https://scholar.google.com/citations?user=vCabh8oAAAAJ)

## Research Highlights & Key Features

### 🔬 Research Excellence
- **600+ Google Scholar Citations** with publications in top-tier journals (IF > 7.9)
- **3 Research Areas**: Trustworthy AI, Foundation Models, and Reliable PHM
- **Award Recognition**: 2024 CAST Youth Talent Support Program, Multiple National Scholarships
- **International Collaboration**: Visiting Scholar at Yale University (2025)

### 💻 Homepage Features  
- **Automatically update google scholar citations**: using the google scholar crawler and github action, this REPO can update the author citations and publication citations automatically.
- **Support Google analytics**: you can trace the traffics of your homepage by easy configuration.
- **Responsive**: this homepage automatically adjust for different screen sizes and viewports.
- **Beautiful and Simple Design**: this homepage is beautiful and simple, which is very suitable for academic personal homepage.
- **SEO**: search Engine Optimization (SEO) helps search engines find the information you publish on your homepage easily, then rank it against similar websites.

## About This Repository

This is the source code for Qi Li's personal academic homepage, built using the AcadHomepage template. The site showcases research in trustworthy AI, foundation models, and PHM, along with publications, awards, and academic activities.

## Using This as a Template

If you'd like to create your own academic homepage using this setup:

1. Fork this repository and rename to `USERNAME.github.io`, where `USERNAME` is your GitHub username.
1. Configure the Google Scholar citation crawler:
    1. Find your Google Scholar ID in the URL of your Google Scholar page (e.g., https://scholar.google.com/citations?user=SCHOLAR_ID).
    1. Set `GOOGLE_SCHOLAR_ID` variable in `Settings -> Secrets -> Actions -> New repository secret` with `name=GOOGLE_SCHOLAR_ID` and `value=SCHOLAR_ID`.
    1. Enable workflows in the `Actions` tab by clicking *"I understand my workflows, go ahead and enable them"*.
1. Generate favicon using [favicon-generator](https://redketchup.io/favicon-generator) and download files to `images/`.
1. Modify `_config.yml` configuration:
    1. Update `title`, `description`, `repository`, and `author` information
    1. Add optional `google_analytics_id` and SEO keys
1. Update your content in `_pages/about.md`:
    1. Use HTML+Markdown syntax
    1. Display paper citations with: `<span class='show_paper_citations' data='PAPER_ID'></span>`
1. Your page will be published at `https://USERNAME.github.io`

## Debug Locally

1. Clone your REPO to local using `git clone`.
1. Install Jekyll building environment, including `Ruby`, `RubyGems`, `GCC` and `Make` following [the installation guide](https://jekyllrb.com/docs/installation/#requirements).
1. Run `bash run_server.sh` to start Jekyll livereload server.
1. Open http://127.0.0.1:4000 in your browser.
1. If you change the source code of the website, the livereload server will automatically refresh.
1. When you finish the modification of your homepage, `commit` your changings and `push` to your remote REPO using `git` command.

# Acknowledges

- AcadHomepage incorporates Font Awesome, which is distributed under the terms of the SIL OFL 1.1 and MIT License.
- AcadHomepage is influenced by the github repo [mmistakes/minimal-mistakes](https://github.com/mmistakes/minimal-mistakes), which is distributed under the MIT License.
- AcadHomepage is influenced by the github repo [academicpages/academicpages.github.io](https://github.com/academicpages/academicpages.github.io), which is distributed under the MIT License.
