# SALSA Research Group Website

This is the official website for the SALSA (Scalable, Autonomous Learning for Sustainable Agents) research group.

## Overview

The SALSA research group focuses on developing autonomous learning systems that can scale to complex real-world problems while maintaining sustainability and responsible AI principles.

## Website Sections

The website is a single-page design containing:

- **Hero Section**: Introduction to the SALSA research group
- **About**: Brief overview of our research focus areas
- **Team**: Meet our researchers and collaborators
- **Publications**: Our latest research papers and publications
- **News**: Twitter feed with latest updates and news
- **Openings**: Career opportunities and positions available

## Development

This website is built with Jekyll, a static site generator.

### Prerequisites

- Ruby 3.0 or higher
- Bundler

### Local Development

1. Install dependencies:
```bash
bundle install
```

2. Build the site:
```bash
bundle exec jekyll build
```

3. Serve the site locally:
```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

### Project Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page layouts
│   └── default.html
├── _includes/           # Reusable components (empty for now)
├── _team/              # Team member profiles
├── _publications/      # Publication entries
├── assets/
│   ├── css/            # Stylesheets
│   ├── js/             # JavaScript files
│   └── images/         # Image assets
├── index.html          # Main page
└── Gemfile             # Ruby dependencies
```

### Adding Content

#### Adding Team Members

Create a new file in `_team/` directory with the following format:

```yaml
---
name: "Member Name"
role: "Position Title"
bio: "Short biography"
image: "/assets/images/member-photo.jpg"  # optional
github: "username"     # optional
twitter: "username"    # optional
website: "https://..."  # optional
scholar: "https://..."  # optional
---
```

#### Adding Publications

Create a new file in `_publications/` directory with the following format:

```yaml
---
title: "Publication Title"
authors: "Author 1, Author 2, et al."
venue: "Conference/Journal Name"
year: 2024
abstract: "Paper abstract..."  # optional
pdf: "https://..."     # optional
arxiv: "https://..."   # optional
code: "https://..."    # optional
doi: "10.xxxx/xxxxx"   # optional
---
```

## Deployment

This site is designed to be deployed on GitHub Pages. Simply push to the main branch and GitHub will automatically build and deploy the site.

## License

See LICENSE file for details.