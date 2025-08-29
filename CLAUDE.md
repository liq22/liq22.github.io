# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is Qi Li's personal academic homepage built with Jekyll and the AcadHomepage template. It's a static site hosted on GitHub Pages that showcases research in trustworthy AI, foundation models, and prognostic health management (PHM).

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Start local development server with live reload
bash run_server.sh
# OR manually:
bundle exec jekyll liveserve

# Access at http://127.0.0.1:4000
```

### Build Commands
```bash
# Build site for production
bundle exec jekyll build

# Serve without live reload
bundle exec jekyll serve
```

## Architecture

### Site Structure
- **_pages/about.md**: Main homepage content with research profile, publications, achievements
- **_config.yml**: Site configuration including author info, social links, and Jekyll settings  
- **_layouts/default.html**: Main page layout template
- **_includes/**: Reusable components (analytics, author profile, navigation, SEO)
- **_sass/**: Styling with modular SCSS files
- **assets/**: CSS, JavaScript, fonts (includes Font Awesome and Academicons)
- **images/**: Profile pictures, paper images, favicons

### Google Scholar Integration
- **google_scholar_crawler/**: Python crawler that fetches citation data
- **main.py**: Scholarly library integration to get citation counts
- **GitHub Action**: Runs daily at 08:00 UTC to update citation data
- **Environment variable**: `GOOGLE_SCHOLAR_ID` (vCabh8oAAAAJ for this site)
- **Output**: Creates `gs_data.json` and `gs_data_shieldsio.json` in `google-scholar-stats` branch

### Content Architecture
- **Single-page design**: All content in about.md with anchor-based navigation
- **Paper citations**: Use `<span class='show_paper_citations' data='PAPER_ID'></span>` for dynamic citation counts
- **Collapsible sections**: Research areas organized with HTML details/summary tags
- **Paper showcase**: Each paper has image, title, authors, description, and code links

### Navigation Structure
Navigation defined in `_data/navigation.yml`:
- About Me (#about-me)
- News (#-news) 
- Publications (#-publications)
- Honors and Awards (#-honors-and-awards)
- Educations (#-educations)
- Invited Talks (#-invited-talks)
- Internships (#-internships)
- Social Activities (#-social-activities)
- Contact (#-contact)

## Key Configuration

### Author Configuration (_config.yml)
- Repository: liq22/liq22.github.io
- Google Scholar ID: vCabh8oAAAAJ  
- ORCID: 0000-0001-7105-2818
- Social profiles: GitHub, ResearchGate, Bilibili, email
- Avatar: images/LQ.png
- Timezone: Asia/Shanghai

### Jekyll Settings
- Uses github-pages gem for GitHub Pages compatibility
- Markdown: kramdown with GFM input
- Plugins: jekyll-feed, jekyll-sitemap, hawkins (live reload)
- Excludes: docs, google_scholar_crawler from build

## File Editing Guidelines

### Adding Publications
1. Add paper image to `images/papers/`
2. Update `_pages/about.md` with new paper entry in appropriate research section
3. Use the established paper-box structure with image, title, authors, description
4. Include journal info with JCR quartile and impact factor
5. Add citation tracking span if desired

### Updating Profile
- Edit `_pages/about.md` for content changes
- Update `_config.yml` for author metadata and social links  
- Replace `images/LQ.png` for new profile photo

### Navigation Changes
- Edit `_data/navigation.yml` for menu items
- Ensure corresponding anchors exist in about.md