# NHL Shots vs Goals Regression

**Author:** Hemangi Vij  
**Course:** MATH 261A – Fall 2025, San José State University  
**Date of submission:** September 2025  

---

## Project Overview
This repository contains my Math 261A Paper 1 project.  
The goal of this analysis is to evaluate whether **shots on goal predict goals scored in NHL games** at the team–game level for the 2021–22 season.  

The paper (`MathProject.qmd`) is written in Quarto and organized into the following sections:  
- **Introduction:** motivation and research question.  
- **Data:** NHL play-by-play dataset description, variables, sample size, and visualizations.  
- **Methods:** linear regression model, assumptions, and software.  
- **Results:** estimated slope, intercept, $R^2$, hypothesis test, residual diagnostics.  
- **Discussion:** interpretation, strengths/limitations, and directions for future work.  

---

## Files
- `MathProject.qmd` – Quarto source file for the paper.  
- `references.bib` – Bibliography file with citations for R, tidyverse, ggplot2, and NHL data.  
- `.gitignore` – Excludes large/raw files and system artifacts from the repo.  
- `README.md` – This file, describing the project.  

---

## Data
The analysis uses official **NHL play-by-play event data** from the 2021–22 season [@nhl_data].  
Each row in the raw dataset represents an event (e.g., shot or goal). For this project, data are aggregated to the **team–game level** to create two variables:  
- **Shots on goal** – all events recorded as shots on goal (including those that became goals).  
- **Goals** – number of goals scored by the team in the game.  

**Dataset license:** The NHL play-by-play data is publicly available from [NHL.com](https://www.nhl.com/stats/). It is used here for educational purposes and is not redistributed in this repository.  

---

## Reproducibility
- Implemented in **R** [@R_language] using the **tidyverse** [@tidyverse2019], **ggplot2** [@ggplot2], **ggpubr** [@ggpubr], **patchwork** [@patchwork], and **stringr** [@stringr].  
- Written in Quarto; output is a PDF document.  
- Repository follows reproducible workflow guidelines with commits, clean structure, and explanatory comments.  

---

## Statement on AI/LLM Use
This project received assistance from an **LLM (ChatGPT)** for:  
- Formatting Quarto `.qmd` chunks.  
- Workflow guidance (Git/GitHub setup, bibliography formatting, README drafting).  
- Clarifying rubric requirements.  

All **analysis, interpretation, and final writing choices** were reviewed and verified by the author.  

---

## License
This repository is for **educational purposes only**.  
- Code and text are available for reuse with attribution.  
- NHL play-by-play data remains © National Hockey League, accessed via NHL.com.  

---

## How to Render
To knit the paper to PDF:  
```bash
quarto render MathProject.qmd --to pdf
