<h1 align="center">
Qi Li - Personal Academic Homepage
</h1>

<div align="center">

[![](https://img.shields.io/github/stars/liq22/liq22.github.io)](https://github.com/liq22/liq22.github.io)
[![](https://img.shields.io/github/forks/liq22/liq22.github.io)](https://github.com/liq22/liq22.github.io)
[![](https://img.shields.io/github/issues/liq22/liq22.github.io)](https://github.com/liq22/liq22.github.io/issues)
[![](https://img.shields.io/github/license/liq22/liq22.github.io)](https://github.com/liq22/liq22.github.io/blob/main/LICENSE) | [中文文档](./docs/README-zh.md)

</div>

<p align="center">Postdoctoral Researcher in the Department of Automation at Tsinghua University<br>Research Focus: Trustworthy AI, Foundation Models, and Reliable PHM</p>

<p align="center">
  <br>
  <img src="docs/screenshot.png" width="100%" alt="Screenshot of Qi Li's academic homepage" loading="lazy">
  <br>
</p>

🏠 **Homepage**: [https://liq22.github.io](https://liq22.github.io)

📧 **Contact**: liq22@tsinghua.org.cn | 🎓 **Google Scholar**: [Profile](https://scholar.google.com/citations?user=vCabh8oAAAAJ)

## Research Highlights and Key Features

### 🔬 Research Profile

- **Research Areas**: Trustworthy AI, foundation models, and reliable prognostics and health management.
- **Research Output**: Publications in leading journals in industrial AI, reliability, and manufacturing systems.
- **Recognition**: CAST Youth Talent Support Program, national scholarships, and university honors.
- **International Experience**: Visiting scholar at Yale University in 2025.

### 💻 Homepage Features

- **Automatic Google Scholar updates**: A crawler and GitHub Actions workflow update author and publication citation counts.
- **Google Analytics support**: Optional analytics configuration for monitoring site traffic.
- **Responsive layout**: The site adapts to desktop, tablet, and mobile viewports.
- **Accessible visual system**: Full-width hero layout, system-aware dark mode, reduced-motion support, and visible keyboard focus states.
- **Image performance**: Lazy loading, asynchronous decoding, stable aspect ratios, and an optional image-compression workflow.
- **SEO support**: Metadata and sitemap integration help search engines discover and index the site.

## About This Repository

This repository contains the source code for Qi Li's academic homepage. It is based on the AcadHomepage template and presents research in trustworthy AI, foundation models, and PHM, together with publications, honors, and academic experience.

## Using This Repository as a Template

1. Fork this repository and rename it to `USERNAME.github.io`, where `USERNAME` is your GitHub username.
2. Configure the Google Scholar citation crawler:
   1. Find the Google Scholar ID in the URL of the relevant Scholar profile.
   2. Create a repository Actions secret named `GOOGLE_SCHOLAR_ID` with that ID as its value.
   3. Enable workflows in the repository's **Actions** tab.
3. Generate favicon assets and place them in `images/`.
4. Update `_config.yml` with the site's title, description, repository, and author information.
5. Update the homepage content in `_pages/about.md`.
6. The site will be published at `https://USERNAME.github.io`.

## Local Development

1. Clone the repository.
2. Install the Jekyll build environment, including Ruby, RubyGems, GCC, and Make, following the [Jekyll installation guide](https://jekyllrb.com/docs/installation/).
3. Run `bash run_server.sh` to start the development server with live reload.
4. Open `http://127.0.0.1:4000`.
5. Commit and push the changes when validation is complete.

## Acknowledgments

- AcadHomepage incorporates Font Awesome, distributed under the SIL OFL 1.1 and MIT licenses.
- AcadHomepage is influenced by [mmistakes/minimal-mistakes](https://github.com/mmistakes/minimal-mistakes), distributed under the MIT License.
- AcadHomepage is influenced by [academicpages/academicpages.github.io](https://github.com/academicpages/academicpages.github.io), distributed under the MIT License.
