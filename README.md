# AWS Internship Report Site

A personal internship report website built with **Hugo** and the **FCJ Workshop template**, documenting my internship experience at **Amazon Web Services Vietnam Co., Ltd.** The site is automatically deployed to **GitHub Pages** via GitHub Actions CI/CD.

🌐 **Live Site:** [https://tmh-1234.github.io/aws-internship-report-site/](https://tmh-1234.github.io/aws-internship-report-site/)

---

## 👤 Author

| Field | Info |
|---|---|
| **Full Name** | Tong Minh Hieu |
| **Email** | minhieutdg@gmail.com |
| **Phone** | 0907270350 |
| **University** | Ho Chi Minh City University of Technology |
| **Major** | Information Technology |
| **Class** | 22DTHJA2 |
| **Company** | Amazon Web Services Vietnam Co., Ltd. |
| **Position** | FCJ Cloud Engineer |
| **Duration** | 17/04/2026 – 30/07/2026 |

---

## 🛠️ Tech Stack

| Tool | Version / Details |
|---|---|
| **Static Site Generator** | [Hugo Extended](https://gohugo.io/) v0.137.1 |
| **Theme** | [hugo-theme-learn](https://github.com/matcornic/hugo-theme-learn) (Git submodule) |
| **Hosting** | GitHub Pages |
| **CI/CD** | GitHub Actions |
| **Languages** | English 🇺🇸 / Vietnamese 🇻🇳 (bilingual) |

---

## 📁 Project Structure

```
aws-internship-report-site/
│
├── .github/
│   └── workflows/
│       └── hugo.yml              # CI/CD: auto-build & deploy to GitHub Pages
│
├── archetypes/
│   └── default.md                # Default front-matter template for new pages
│
├── content/                      # All site content (bilingual: .md & .vi.md)
│   ├── _index.md                 # Homepage (English)
│   ├── _index.vi.md              # Homepage (Vietnamese)
│   │
│   ├── 1-Worklog/                # Weekly activity log (12 weeks)
│   │   ├── 1.1-Week1/            #
│   │   ├── 1.2-Week2/            #
│   │   ├── 1.3-Week3/            #
│   │   ├── 1.4-Week4/            #
│   │   ├── 1.5-Week5/            #
│   │   ├── 1.6-Week6/            #
│   │   ├── 1.7-Week7/            #
│   │   ├── 1.8-Week8/            #
│   │   ├── 1.9-Week9/            #
│   │   ├── 1.10-Week10/          #
│   │   ├── 1.11-Week11/          #
│   │   ├── 1.12-Week12/          #
│   │
│   ├── 2-Proposal/               # Internship proposal document
│   │
│   ├── 3-Blogs-Posted/        # 3 AWS blogs
│   │   ├── 3.1-Blog1/            # Blog 1: Refining the Serverless Architecture for GreenLens Kids through Practical Experience
│   │   ├── 3.2-Blog2/            # Blog 2: Building the Cloud Application Layer with First Cloud AI Journey
│   │   ├── 3.3-Blog3/            # Blog 3: Summarizing the Journey of Building GreenLens Kids with First Cloud AI Journey
│   │
│   ├── 4-EventParticipated/      # Events attended during internship
│   │   ├── 4.1-Event1/           # GenAI-powered App-DB Modernization Workshop
│   │   └── 4.2-Event2/
│   │
│   ├── 5-Workshop/               # Technical workshop documentation
│   │   ├── 5.1-Workshop-overview/
│   │   ├── 5.2-Prerequiste/
│   │   ├── 5.3-S3-vpc/           # Access S3 from VPC (Gateway Endpoint)
│   │   ├── 5.4-S3-onprem/        # Access S3 from On-premises (Interface Endpoint)
│   │   ├── 5.5-Policy/           # VPC Endpoint Policies (Bonus)
│   │   └── 5.6-Cleanup/          # Resource cleanup steps
│   │
│   ├── 6-Self-evaluation/        # Intern self-assessment criteria table
│   └── 7-Feedback/               # Sharing and feedback section
│
├── layouts/
│   ├── partials/
│   │   ├── custom-footer.html    # Custom footer override
│   │   ├── logo.html             # Custom logo partial
│   │   └── menu-footer.html      # Menu footer partial
│   └── shortcodes/
│       ├── ghcontributors.html   # GitHub contributors shortcode
│       ├── tab.html              # Tab shortcode
│       └── tabs.html             # Tabs container shortcode
│
├── static/
│   ├── AWS_Logo.svg              # AWS logo asset
│   ├── css/
│   │   ├── theme-mine.css        # Custom theme CSS
│   │   └── theme-workshop.css    # Workshop theme CSS variant
│   ├── fonts/                    # Custom fonts
│   └── images/
│       ├── Avatar.JPG            # Author profile picture
│       ├── favicon.png           # Site favicon
│       ├── favicon-16x16.png
│       ├── 2-Proposal/           # Images for Proposal section
│       └── 5-Workshop/           # Images for Workshop section
│
├── themes/
│   └── hugo-theme-learn/         # Git submodule: FCJ Learn theme
│
├── config.toml                   # Main Hugo site configuration
├── .gitmodules                   # Git submodule reference (theme)
├── .gitignore                    # Ignores public/, logs, editor files
└── README.md                     # This file
```

---

## 📋 Report Contents

The site is organized into 7 main sections:

| # | Section | Description |
|---|---|---|
| 1 | **Worklog** | Weekly activity logs covering 12 weeks of internship |
| 2 | **Proposal** | Internship plan and project proposal submitted to AWS |
| 3 | **Blogs Posted** | 3 AWS official blogs translated from English to Vietnamese |
| 4 | **Events Participated** | Events and workshops attended during the internship period |
| 5 | **Workshop** | Step-by-step technical lab: *Secure Hybrid Access to S3 using VPC Endpoints* |
| 6 | **Self-evaluation** | Self-assessment across 12 professional criteria |
| 7 | **Sharing & Feedback** | Personal reflections, lessons learned, and feedback |

### 🔬 Workshop: Secure Hybrid Access to S3 using VPC Endpoints

The workshop section documents a hands-on AWS lab covering **AWS PrivateLink** and **VPC Endpoints** to provide secure, private connectivity to Amazon S3 — without traversing the public internet.

- **Gateway VPC Endpoint** – Routes S3/DynamoDB traffic via route tables from within a VPC
- **Interface VPC Endpoint** – Uses DNS resolution and Network Load Balancer for on-premises access
- Includes prerequisite setup, testing, endpoint policies, and resource cleanup

---

## 🚀 Getting Started (Local Development)

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) v0.137.1+
- Git

### Clone & Run

```bash
# Clone with submodules (required for the theme)
git clone --recurse-submodules https://github.com/tmh-1234/aws-internship-report-site.git
cd aws-internship-report-site

# Start local dev server
hugo server -D
```

The site will be available at: `http://localhost:1313/aws-internship-report-site/`

> If you already cloned without `--recurse-submodules`, run:
> ```bash
> git submodule update --init --recursive
> ```

---

## ⚙️ Configuration

The main configuration is in [`config.toml`](./config.toml):

- **`baseURL`** – Set to the GitHub Pages URL
- **`theme`** – `hugo-theme-learn` (FCJ Workshop variant)
- **`themeVariant`** – `workshop` (custom AWS-styled color scheme)
- **`defaultContentLanguage`** – `en` (English default, with Vietnamese available)
- **Multilingual** – Configured under `[Languages.en]` and `[Languages.vi]`
- **Menu shortcuts** – Links to GitHub repo and AWS FCJ Study Group Facebook

---

## 🔄 CI/CD Deployment

Deployments are automated via **GitHub Actions** (`.github/workflows/hugo.yml`):

1. **Trigger:** Push to `main` branch (or manual `workflow_dispatch`)
2. **Build job:**
   - Checks out source with submodules
   - Installs Hugo Extended v0.137.1
   - Builds site with `--minify` flag
   - Uploads build artifact
3. **Deploy job:**
   - Deploys the built artifact to GitHub Pages
   - Timezone: `Asia/Ho_Chi_Minh`

---

## 🌏 Multilingual Support

All content pages are available in both **English** and **Vietnamese**:

- English pages: `_index.md`
- Vietnamese pages: `_index.vi.md`

Language switching is available in the site navigation.

---

## 🔗 Links

- 📁 [GitHub Repository](https://github.com/tmh-1234/aws-internship-report-site)
- 👥 [AWS FCJ Study Group (Facebook)](https://www.facebook.com/groups/awsstudygroupfcj/)
- 🎨 [Hugo Theme Learn](https://github.com/matcornic/hugo-theme-learn)
- Linkedin: https://www.linkedin.com/in/tong-minh-hieu-8979a6403/
