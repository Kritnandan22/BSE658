# BSE658 — Statistics with R

A course repository for **BSE658**, covering fundamental and applied statistics using the R programming language. The course progresses from R basics to advanced statistical modelling, with hands-on R Markdown notebooks and real-world datasets.

---

## 📁 Repository Structure

```
BSE658/
├── Datasets/          # Shared datasets used across modules
├── Module 1/          # Introduction to R & R Notebooks
├── Module 2/          # Data Wrangling (Tidyverse) & Visualisation (ggplot2)
├── Module 3/          # Descriptive Statistics
├── Module 4/          # Inferential Statistics: Sampling, Estimation & Hypothesis Tests
├── Module 5/          # Hypothesis Testing: t-test & Chi-square Test
└── Module 6/          # Regression, ANOVA & Linear Mixed Models
```

---

## 📊 Datasets

Located in the `Datasets/` folder, three datasets are provided for class groups along with detailed description documents (`.docx`):

| File | Description |
|------|-------------|
| `Biological_Mouse_cortex.csv` | Biological dataset — mouse cortex measurements |
| `Covid_country_vaccinations.csv` | COVID-19 country-level vaccination data |
| `Psychological_DASS.csv` | Psychological dataset — Depression, Anxiety & Stress Scales (DASS) |

Each dataset has an accompanying `_info.docx` file that describes the variables and context.

---

## 📚 Modules

### Module 1 — Introduction to R & R Notebooks

**Folder:** `Module 1/`

An introductory module that familiarises students with R Markdown and R Notebooks as tools for reproducible data analysis.

| File | Description |
|------|-------------|
| `R notebook tutorial.Rmd` | Core tutorial: what is Markdown, what is an R Notebook, how to insert and run code chunks |
| `R notebook tutorial-2.Rmd` | Follow-up tutorial with additional exercises |
| `Notebook for chapter 1.Rmd` | Chapter 1 notebook — first steps in R |
| `*.nb.html` | Pre-rendered HTML outputs (open in a browser) |

**Key topics:**
- What is Markdown and R Markdown
- Creating and running R Notebooks in RStudio
- Literate programming and reproducible research

---

### Module 2 — Data Wrangling & Visualisation

**Folder:** `Module 2/`

Introduces the two pillars of modern R data science: **Tidyverse** for data manipulation and **ggplot2** for publication-quality graphics.

| File | Description |
|------|-------------|
| `Tidyverse.Rmd` | Installing and using Tidyverse packages (`dplyr`, `tidyr`, etc.) on a COVID testing dataset |
| `using ggplot.Rmd` | Building plots with `ggplot2` |
| `StatewiseTestingDetails.csv` | Statewise COVID-19 testing data (India) used in examples |
| `*.nb.html` / `*.html` | Pre-rendered HTML outputs |

**Key topics:**
- R packages: installation and loading (CRAN)
- Data frames and tibbles
- Data manipulation with `dplyr` and `tidyr`
- Data visualisation with `ggplot2` (aesthetics, geoms, layers)

---

### Module 3 — Descriptive Statistics

**Folder:** `Module 3/`

Covers the mathematical and conceptual foundations of describing data, including distributions, central tendency, and variability.

**Sub-folders:**
- `Datasets/` — Module-specific datasets (`.Rdata` files: `aflsmall`, `anscombesquartet`, `clinicaltrial`, `effort`, `parenthood`, `parenthood2`)
- `Notebooks/` — All R Markdown notebooks for this module

| Notebook | Description |
|----------|-------------|
| `Module3_Nb1.Rmd` | Descriptive statistics: central tendency and variability measures using the `lsr` package |
| `Module3_Nb2.Rmd` | Extended descriptive analysis |
| `Distributions.Rmd` / `Distributions_part2.Rmd` | Frequency distributions, histograms, and probability distributions |
| `Plotting.Rmd` | Visualising distributions and descriptive statistics |
| `SamplingDistribution.Rmd` | Introduction to sampling distributions |

**Key topics:**
- Frequency distributions and histograms
- Measures of central tendency: mean, median, mode
- Measures of variability: variance, standard deviation, range
- Introduction to probability distributions

---

### Module 4 — Inferential Statistics: Sampling, Estimation & Hypothesis Testing

**Folder:** `Module 4/`

Bridges descriptive and inferential statistics, focusing on how conclusions are drawn from samples about populations.

**Sub-folders:**

#### `Sampling_estimation/`
| File | Description |
|------|-------------|
| `Sampling_and_estimation.Rmd` | Sampling theory, point estimates, confidence intervals |
| Datasets (`.Rdata` / `.png`) | `afl24`, `aflsmall`, `fig1.png`, `fig2.png`, `fig3.png` |

#### `t-test/`
| File | Description |
|------|-------------|
| `ztest.Rmd` | One-sample z-test |
| `t-test.Rmd` | One-sample and independent-samples t-test |
| `Normality-check.Rmd` | Normality testing (Shapiro-Wilk, Q-Q plots) |
| `Diet_R.csv` | Diet study dataset used for z-test and t-test examples |
| Datasets (`.Rdata`) | `chico`, `zeppo` |

**Key topics:**
- Population vs. sample, sampling error
- Point estimation and interval estimation (confidence intervals)
- The Central Limit Theorem
- z-test and t-test for hypothesis testing
- Checking assumptions: normality tests

---

### Module 5 — Hypothesis Testing: t-test & Chi-square Test

**Folder:** `Module 5/`

Practical application of hypothesis testing with paired/independent t-tests and chi-square tests for categorical data.

| File | Description |
|------|-------------|
| `Ttest.Rmd` | Independent and paired-samples t-test using `lsr` and `psych` packages |
| `Chi_sq.Rmd` | Goodness-of-fit and test of independence using chi-square |
| Datasets (`.Rdata`) | `agpp`, `chapek9`, `chico`, `harpo`, `randomness`, `salem`, `zeppo` |
| `*.nb.html` | Pre-rendered HTML outputs |

**Key topics:**
- One-sample, independent, and paired-samples t-tests
- Effect size (Cohen's *d*)
- Chi-square goodness-of-fit test
- Chi-square test of independence
- Interpreting p-values and making decisions

---

### Module 6 — Regression, ANOVA & Linear Mixed Models

**Folder:** `Module 6/`

Advanced statistical modelling covering linear regression in multiple forms, analysis of variance, and mixed-effects models.

| File | Description |
|------|-------------|
| `Regression.Rmd` | Simple and multiple linear regression; model diagnostics |
| `CategoricalRegression.Rmd` | Regression with categorical predictors (dummy coding) |
| `Nonlinearity.Rmd` | Polynomial regression and non-linear relationships |
| `ANOVA.Rmd` | One-way ANOVA; comparing group means (Joyzepam drug study example) |
| `linearMixedModels.Rmd` | Linear mixed-effects models using `lme4` / `tidyverse` |
| `testcode.Rmd` | Additional test/exploratory code |
| Datasets (`.Rdata` / `.csv`) | `clinicaltrial`, `parenthood`, `winter_2016_senses_valence.csv` |
| `*.nb.html` | Pre-rendered HTML outputs |

**Key topics:**
- Simple linear regression: coefficients, R², model fit
- Multiple regression and predictor selection
- Categorical predictors and interaction terms
- One-way and factorial ANOVA; post-hoc tests
- Fixed effects vs. random effects
- Linear mixed-effects models for repeated measures / hierarchical data

---

## 🛠️ Prerequisites & Setup

### Software
- [R](https://cran.r-project.org/) (version ≥ 4.0 recommended)
- [RStudio](https://posit.co/download/rstudio-desktop/) (for running `.Rmd` notebooks interactively)

### R Packages

The notebooks use the following packages (install once in R):

```r
install.packages(c(
  "tidyverse",   # dplyr, tidyr, readr, stringr, ...
  "ggplot2",     # data visualisation
  "lsr",         # learning statistics with R helper functions
  "psych",       # psychological statistics utilities
  "magrittr",    # pipe operator
  "lme4"         # linear mixed-effects models
))
```

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/Kritnandan22/BSE658.git
   cd BSE658
   ```

2. **Open the R Project**
   Double-click `BSE658.Rproj` to open the project in RStudio. This sets the working directory correctly for all notebooks.

3. **Open a notebook**
   Navigate to any module folder, open an `.Rmd` file in RStudio, and click **Run All** (or run chunks individually with `Ctrl+Shift+Enter`).

4. **View pre-rendered outputs**
   Each module contains `.nb.html` or `.html` files — download and open them in any browser to read the notebooks without running R.

---

## 📖 Course Topics at a Glance

| Module | Topic |
|--------|-------|
| 1 | Introduction to R, RStudio & R Notebooks |
| 2 | Data Wrangling with Tidyverse; Visualisation with ggplot2 |
| 3 | Descriptive Statistics: Distributions, Central Tendency, Variability |
| 4 | Inferential Statistics: Sampling, Estimation, z-test, t-test |
| 5 | Hypothesis Testing: t-test, Chi-square Test |
| 6 | Regression, ANOVA, Linear Mixed Models |

---

## 📄 License

This repository is intended for educational purposes as part of the BSE658 course.
