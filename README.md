# Workflow for Contributing & Publishing 

Use RStudio to branch, edit, preview, render, and publish our Quarto site (served from `docs/`) on GitHub Pages.

---

## 1. Open the Project in RStudio

1. Go to **File ▶ New Project ▶ Version Control ▶ Git**  
2. Enter the repo URL (e.g. `git@github.com:your-org/your-quarto-site.git`)  
3. Choose a local folder, then **Create Project**  
4. RStudio will clone the repo and open it as a project  

---

## 2. Create a Feature Branch

1. In the **Git** pane, click **Branch ▶ New Branch**  
2. Name it `feat/your-topic` and click **Create**  
3. Verify you’re on your new branch  

---

## 3. Make Your Changes

- Edit `.qmd` files in the **Source** pane  
- Update `_quarto.yml` or `styles/style.css`  
- Add new images or data under `images/`, `data/`, etc.

---

## 4. Preview Locally

Either option A or B: 
### A. Using the Addin  
- **Addins ▶ Quarto ▶ Preview Website**  
- Browser auto-reloads at `http://localhost:4200`

### B. Using the R Console  
```r
quarto::quarto_preview()
```

---

## 6. Render the Site
Either option A or B: 
### A. Using R  
```r
quarto::quarto_render()
```
This regenerates the HTML into `docs/`.

### B. Using Terminal (optional)  
```bash
quarto render --to html
```

---

## 7. Commit & Push via RStudio

1. In the **Git** pane, stage your changes:
   - Include both source files (`.qmd`, CSS) **and** updated `docs/**`  
2. Click **Commit**, write a clear message (e.g. `feat: add fall workshop page`), then **Commit**  
3. Click **Push** to send your branch to GitHub  

---

## 8. Open a Pull Request

1. On GitHub, click **Compare & pull request** for your branch  
2. Fill in title/description and assign reviewers/labels  
3. Click **Create pull request**  

---

## 9. Review, Merge & Publish

- Once merged into `main`, GitHub Pages (serving `docs/`) will auto-deploy within minutes  
- Verify your live site at  
  `https://your-org.github.io/your-quarto-site/`

---

Verify your live site at
https://your-org.github.io/your-quarto-site/
