# 📊 CodeSummary
> **A general-purpose RMarkdown template for structured, reproducible data analysis.**  
> Load → Clean → Analyze → Visualize → Export — all in one polished document.

<br>

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Language](https://img.shields.io/badge/Language-R%20%7C%20RMarkdown-276DC3?logo=r)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Themes](https://img.shields.io/badge/Themes-Light%20%7C%20Dark-F2EFE9?logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48Y2lyY2xlIGN4PSI4IiBjeT0iOCIgcj0iOCIgZmlsbD0iIzEyMTMxNyIvPjwvc3ZnPg==)

---

## 🎨 Two themes, one workflow

<table>
<tr>
<td align="center" width="50%">

### ☀️ Light — Bone
Formal academic style with bone background (`#F2EFE9`), Georgia serif typography and restrained institutional palette.

</td>
<td align="center" width="50%">

### 🌙 Dark — Soft Neon
Midnight UI background (`#121317`) with Soft Neon Overlay palette: Blush Pink, Mint Glow and Highlight Yellow syntax highlighting.

</td>
</tr>
<tr>
<td align="center">

<a href="https://dotstefano.github.io/Code_summary/">
  <img src="assets/CODE_SUMMARY.png" width="400" alt="Light theme preview"/>
</a>

</td>
<td align="center">

<a href="https://dotstefano.github.io/Code_summary/">
  <img src="assets/CODE_SUMMARY_DARK.png" width="400" alt="Dark theme preview"/>
</a>

</td>
</tr>
<tr>
<td align="center"><sub>Click to open the live interactive document</sub></td>
<td align="center"><sub>Click to open the live interactive document</sub></td>
</tr>
</table>

---

## ✨ What is this?

`CodeSummary` is a ready-to-use **RMarkdown template** designed to bring structure and clarity to your data analysis workflow. Instead of starting from a blank `.Rmd` every time, this template gives you a clean, consistent scaffold with all the sections you need — from data loading to final export.

Each analysis chunk comes with a **collapsible interpretation block**, so you can annotate findings inline without cluttering the code. A final **interactive progress checklist** ties everything together.

---

## 🗂️ Template Structure

```
📄 skeleton.Rmd
│
├── 📥  1. Setup & Libraries
├── 📂  2. Data Loading
├── 🧹  3. Data Cleaning
├── 📊  4. Descriptive Statistics
├── 🔬  5. Statistical Tests
├── 📈  6. Visualization
├── 📤  7. Export (Excel / CSV)
└── ✅  8. Progress Checklist
```

Each section includes:
- Annotated, ready-to-modify code
- A `<details>` collapsible block for interpretations
- Consistent chunk naming for easy navigation

---

## 🚀 Quick Start

**1. Install the package**

```r
remotes::install_github("DotStefano/Code_summary")
```

**2. Open the template in RStudio**

File → New File → R Markdown → From Template → choose your theme:
- **Data Analysis template - Light**
- **Data Analysis template - Dark**

**3. Or download directly**

```r
# Light theme
download.file(
  url = "https://raw.githubusercontent.com/DotStefano/Code_summary/main/inst/rmarkdown/templates/doctorado/skeleton/skeleton.Rmd",
  destfile = "my_analysis.Rmd"
)

# Dark theme
download.file(
  url = "https://raw.githubusercontent.com/DotStefano/Code_summary/main/inst/rmarkdown/templates/doctorado_dark/skeleton/skeleton.Rmd",
  destfile = "my_analysis_dark.Rmd"
)
```

**4. Render**

```r
rmarkdown::render("my_analysis.Rmd")
```

---

## 📦 Dependencies

```r
install.packages(c(
  "tidyverse",   # Data wrangling and visualization
  "openxlsx",    # Excel export
  "knitr",       # Report rendering
  "kableExtra"   # Table formatting
))
```

---

## 💡 Key Features

| Feature | Description |
|---|---|
| 🎨 **Two themes** | Light (bone) and Dark (soft neon) — pick your style |
| 🔁 **Reproducible** | Self-contained structure, clear session info block |
| 💬 **Annotatable** | Collapsible `<details>` blocks per chunk for inline notes |
| ✅ **Progress checklist** | Interactive checklist with progress bar at the end |
| 📤 **Export-ready** | Built-in multi-sheet Excel export section |
| 🔬 **Analysis-focused** | Covers the full pipeline from raw data to final output |
| 🧩 **Modular** | Each section is independent — add, remove, or reorder freely |

---

## 📁 Repository Structure

```
Code_summary/
├── assets/
│   ├── CODE_SUMMARY.png          # Light theme preview
│   └── CODE_SUMMARY_DARK.png     # Dark theme preview
├── inst/rmarkdown/templates/
│   ├── doctorado/                # Light theme
│   │   ├── template.yaml
│   │   └── skeleton/
│   │       └── skeleton.Rmd
│   └── doctorado_dark/           # Dark theme
│       ├── template.yaml
│       └── skeleton/
│           └── skeleton.Rmd
├── index.html                    # Live preview (GitHub Pages)
├── DESCRIPTION
├── LICENSE
└── README.md
```

---

## 🤝 Contributing

Suggestions and improvements are welcome. Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
  <sub>Built for reproducible research · Made with ❤️ and R</sub>
</div>

