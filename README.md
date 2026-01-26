# DATA 4950: Data Science Capstone — Course Materials

**Spring 2026 | Middle Tennessee State University**

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Course](https://img.shields.io/badge/Course-DATA%204950-purple.svg)]()

## 📋 Course Overview

This repository contains all course materials, demonstration projects, templates, and resources for DATA 4950: Data Science Capstone.

**Instructor:** Dr. Yanfang Liu  
**Schedule:** Mondays 6:00 PM - 9:00 PM via Zoom  
**Office Hours:** T/R 2:00 PM - 3:30 PM via [Zoom](https://mtsu.zoom.us/j/81604724560)

---

## 🗂️ Repository Structure

```
course-materials/
├── demos/                              # Instructor-led demonstration projects
│   ├── california-housing-regression/  # Weeks 4-5
│   └── bank-marketing-classification/  # Weeks 6-7
│
├── templates/                          # Templates for deliverables
│   ├── project-charter-template.md
│   └── final-report-template.md
│
├── rubrics/                            # Grading rubrics
│   ├── project-charter-rubric.md
│   ├── eda-report-rubric.md
│   ├── modeling-report-rubric.md
│   ├── final-report-rubric.md
│   └── presentation-rubric.md
│
├── resources/                          # Additional learning resources
│   └── useful-links.md
│
└── syllabus/                           # Course syllabus
    └── DATA4950_Syllabus_Spring2026.pdf
```

---

## 🎯 Demo Projects

We will walk through two complete projects together in class. These follow the exact same 7-stage pipeline you will use for your team project.

| Demo | Type | Dataset | Weeks | Status |
|------|------|---------|-------|--------|
| [California Housing](demos/california-housing-regression/) | Regression | [sklearn.datasets](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html) | 4-5 | 📂 Available |
| [Bank Marketing](demos/bank-marketing-classification/) | Classification | [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing) | 6-7 | 📂 Available |

---

## 🚀 Getting Started

### For Students

1. **Bookmark this repository** — You'll reference it throughout the semester
2. **Clone it locally** (optional, for running demo notebooks):
   ```bash
   git clone https://github.com/MTSU-DATA4950-Capstone-Spring2026/course-materials.git
   ```
3. **Create your team repository** — Use the [capstone-project-template](https://github.com/MTSU-DATA4950-Capstone-Spring2026/capstone-project-template)

### Prerequisites (Complete Before Week 3)

- [ ] **GitHub account** — [Sign up here](https://github.com/join) (free)
- [ ] **Git installed** — [Download Git](https://git-scm.com/downloads)
- [ ] **Python 3.10+** — [Download Python](https://www.python.org/downloads/)
- [ ] **Jupyter Notebook** — `pip install notebook` or use VS Code

---

## 📅 Course Schedule & Deliverables

| Week | Date | Topic | Deliverable |
|------|------|-------|-------------|
| 1 | Jan 19 | *MLK Day - No Class* | — |
| 2 | Jan 26 | Course Introduction & Project Lifecycle | — |
| 3 | Feb 2 | Git/GitHub Fundamentals | GitHub setup |
| 4 | Feb 9 | Demo: Regression (EDA) | — |
| 5 | Feb 16 | Demo: Regression (Modeling) | **Project Charter (8%)** |
| 6 | Feb 23 | Demo: Classification (EDA) | **Quiz 1 (7.5%)** |
| 7 | Mar 2 | Demo: Classification (Modeling) | — |
| 8 | Mar 9 | *Spring Break - No Class* | — |
| 9 | Mar 16 | Feature Engineering & Pipelines | **EDA Report (12%)** |
| 10 | Mar 23 | Peer Review Workshop I | **Peer Review 1 (5%)** |
| 11 | Mar 30 | Model Selection & Tuning | — |
| 12 | Apr 6 | Deployment & MLOps | **Modeling Report (12%)** |
| 13 | Apr 13 | Peer Review Workshop II | **Peer Review 2 (5%)** |
| 14 | Apr 20 | LLMs in Data Science | **Quiz 2 (7.5%)** |
| 15 | Apr 27 | Final Presentations | **Presentation (10%)** |
| +5 days | May 2 | — | **Final Report (23%)** |

---

## 📁 Your Team Repository

Use our [capstone-project-template](https://github.com/MTSU-DATA4950-Capstone-Spring2026/capstone-project-template) to create your team repo. Your repository should follow this structure:

```
team-project-name/
├── README.md
├── .gitignore
├── requirements.txt
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── reports/
├── models/
└── presentations/
```

> ⚠️ **Important:** Do NOT commit large data files. Use `.gitignore` to exclude them.

---

## 🤖 LLM Policy

Large Language Models (ChatGPT, Claude, Copilot, etc.) are:

| ✅ Permitted | ❌ Not Permitted |
|-------------|-----------------|
| Debugging code errors | Generating analysis code |
| Understanding error messages | Writing reports |
| Clarifying documentation | Creating visualizations |
| | Answering quiz questions |

**All LLM usage must be documented.** Projects substantially generated by AI will receive a maximum grade of 30%.

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| Zoom Class | [Join](https://mtsu.zoom.us/j/81270840540) |
| Zoom Office Hours | [Join](https://mtsu.zoom.us/j/81604724560) |
| Project Template | [capstone-project-template](https://github.com/MTSU-DATA4950-Capstone-Spring2026/capstone-project-template) |
| Syllabus | [PDF](syllabus/DATA4950_Syllabus_Spring2026.pdf) |

---

## 📞 Getting Help

1. **During class:** Zoom chat or unmute
2. **Office hours:** T/R 2:00-3:30 PM via Zoom
3. **Email:** yanfang.liu@mtsu.edu
4. **GitHub issues:** Post questions in this repo's Issues tab

---

*Last updated: January 26, 2026*
