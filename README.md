# Chemometrics Web App — Data Handling (Part 1)

![Status](https://img.shields.io/badge/Status-Active-green)
![Version](https://img.shields.io/badge/Release-V3-orange)
![License](https://img.shields.io/badge/License-Proprietary%20%2F%20INPI%20Registered-red.svg)
![R](https://img.shields.io/badge/R%20Version-4.3.0%2B-blue.svg)

Developed by the **[Process Analytical Technology Laboratory (LTAP-UERJ)](https://www.ltapuerj.com.br/)**, this application is a comprehensive tool for data treatment, missing data imputation, spectral signal transformations, baseline and scatter corrections, variable normalization, and descriptive multivariate diagnostics in chemometric datasets.

---

## 🔗 Quick Links

* **Online Web App:** [Access on Shinyapps.io](https://ltap.shinyapps.io/data_handling/)
* **Desktop Executable Download:** [Download Executable (Google Drive)](https://drive.google.com/drive/folders/1l8dB4BGKVjqPMrvA5ZCLvafRNtTOCFew?usp=drive_link)
* **Scientific Article:** [Chemometrics Web App Part 1: Data Handling (Chemometrics and Intelligent Laboratory Systems)](https://doi.org/10.1016/j.chemolab.2022.104696)
* **Official Website:** [LTAP-UERJ Portal](https://www.ltapuerj.com.br/)
* **Software Registration (INPI):** [LTAP-UERJ CWA — Registros de Software](https://sites.google.com/view/ltap-uerj/cwa)
* **Support & Licensing:** [licarion@gmail.com](mailto:licarion@gmail.com) | [ltapuerj@gmail.com](mailto:ltapuerj@gmail.com)

---

## 👥 Developers & Authors

This module was developed by the chemometrics research team at **LTAP-UERJ**:

| Author | Affiliation | Profile / Contact |
| :--- | :--- | :--- |
| **[Bernardo Cardeal Darzé](http://lattes.cnpq.br/0590620499595344)** | LTAP — UERJ | [Lattes Profile](http://lattes.cnpq.br/0590620499595344) |
| **[José Licarion Pinto Segundo Neto](http://lattes.cnpq.br/5267552018296169)** | LTAP — UERJ | [Lattes Profile](http://lattes.cnpq.br/5267552018296169) |
| **[Aderval Severino Luna](http://lattes.cnpq.br/0294676847895948)** | UERJ | [Lattes Profile](http://lattes.cnpq.br/0294676847895948) |
| **I. C. A. Lima** | LTAP — UERJ | [Email](mailto:ltapuerj@gmail.com) |

---

## 🆕 Version History (Change Log)

### **V3 — Current Release**
* **Diagnostic Tools Module:** Upgraded the interactive comparison tab to a dedicated **Diagnostic Tools** engine featuring:
    * **Comparative PCA:** Streamlined tool for exploratory diagnostic analysis before and after pretreatment (fixed at 5 PCs, 95% confidence interval).
    * **Argument Safety Restrictions:** Simplified parameters for safer and easier pretreatment configuration.
* **Robust Variable Preprocessing:** Added **Median Centering** for non-parametric normalization workflows.
* **Data Transposition Tool:** Integrated one-click transpose toggle to flip orientation between samples in rows or columns.
* **CWA Workspace Serialization:** Save and restore workspace states in `.RData` format for seamless inter-module data transfer across the CWA platform.

### **V2 — Improved Compatibility & Refactoring**
* **Normality Test Guard:** Automatic omission of univariate/multivariate normality tests in sample classes with fewer than 5 observations to prevent execution crashes.
* **Spectral Diagnostic Engine:** Initial implementation of diagnostic tool logic for spectral signal inspection.

### **V1 — Initial Release**
* Fundamental implementation of descriptive statistics, missing data imputation (KNN, Random Forest, SVD, NIPALS), Savitzky-Golay derivatives, and basic variable scaling.

---

## 🚀 Key Features

### 📊 Descriptive Analysis & Normality Tests
| Tool | Description |
| :--- | :--- |
| **Summary Statistics** | Central tendency, dispersion, skewness, and kurtosis per variable and per sample class. |
| **Class Distribution** | Class frequencies, missing value proportions, interactive boxplots, and histograms. |
| **Multivariate Normality** | Henze-Zirkler, Royston, and Mardia multivariate normality diagnostic tests. |
| **Correlation Maps** | Interactive heatmaps displaying Pearson, Spearman, and Kendall correlation matrices. |

### 🧩 Data Imputation
| Method Type | Algorithms |
| :--- | :--- |
| **Simple Substitutions** | Mean, Median, and Minimum/Maximum substitution. |
| **ML & Statistical Imputation** | K-Nearest Neighbors (KNN), Random Forest (`missForest`), and Singular Value Decomposition (SVD). |
| **PCA Imputation** | NIPALS (Iterative PCA), Bayesian PCA, and Probabilistic PCA imputation methods. |

### 📈 Spectral Transformations & Signal Pretreatment
| Category | Algorithms |
| :--- | :--- |
| **Smoothing & Derivatives** | Savitzky-Golay smoothing, 1st/2nd order derivatives, and Moving Average filter. |
| **Scatter Correction** | Standard Normal Variate (SNV) and Multiplicative Scatter Correction (MSC). |
| **Baseline Correction** | Asymmetric Least Squares (ALS), Polynomial fitting, Low-Pass FFT, and Rolling Ball baseline estimation. |
| **Peak Alignment** | Parametric Time Warping (PTW) for spectral band alignment. |

### 🎛️ Variable Preprocessing & Normalization
| Technique | Description |
| :--- | :--- |
| **Scaling & Centering** | Mean Centering, Median Centering, Auto-scaling (Standardization), Range Scaling, and Pareto Scaling. |
| **Normality Transformations** | Box-Cox and Yeo-Johnson power transformations with automated lambda parameter estimation. |

---

## 🛠️ Technical Stack & Environment

### **Build & Compilation Environment**
* **Language Runtime:** `R (>= 4.3.0)`

### **Core R Dependencies & Libraries**
| Package | Version / Scope | Purpose |
| :--- | :--- | :--- |
| **`shiny`** | `^1.8.0` | Reactive application framework and web server architecture. |
| **`shinydashboard`** | `^0.7.2` | Dashboard layout structure and sidebar navigation UI. |
| **`plotly`** | `^4.10.0` | Interactive 2D/3D charts, spectral landscapes, and correlation maps. |
| **`DT`** | `^0.30` | DataTables interface for dataset preview and interactive tabular outputs. |
| **`mdatools`** | `^0.14.0` | Principal Component Analysis and chemometric modeling tools. |
| **`prospectr`** | `^0.2.7` | NIR/Raman spectral preprocessing (Savitzky-Golay, SNV, MSC). |
| **`baseline`** | `^1.3-4` | Baseline estimation and removal algorithms (ALS, Polynomial, Rolling Ball). |
| **`ptw`** | `^1.9-15` | Parametric Time Warping and spectral peak alignment. |
| **`missForest`** | `^1.5` | Non-parametric random forest missing value imputation. |
| **`pcaMethods`** | `^1.90.0` | NIPALS, Bayesian PCA, and Probabilistic PCA imputation. |
| **`VIM`** | `^6.2.2` | Visualization and imputation of missing values (KNN imputation). |
| **`MVN`** | `^5.9` | Multivariate normality tests (Mardia, Royston, Henze-Zirkler). |
| **`nortest`** | `^1.0-4` | Univariate normality tests (Anderson-Darling, Cramer-von Mises, Lilliefors). |
| **`corrplot`** | `^0.92` | Interactive visual correlation matrices. |
| **`GGally`** | `^2.1.2` | Extension of ggplot2 for scatterplot matrices. |
| **`rhandsontable`** | `^0.3.8` | Editable data grid for direct data manipulation in UI. |

---

## 💻 Access & Execution

This application is distributed under proprietary closed-source terms (the underlying `app.R` source code is not publicly distributed). Access is available through two distribution models:

1. **🌐 Online Web Version (Shinyapps.io):**
   * Access directly via web browser without installing R or any dependencies:
   * 🔗 **[https://ltap.shinyapps.io/data_handling/](https://ltap.shinyapps.io/data_handling/)**

2. **🖥️ Desktop Executable Version:**
   * Standalone Windows executable bundle (`.exe`) with an embedded runtime environment. No prior R installation required on the target computer.
   * Download the executable for Data Handling (Part 1) and other LTAP CWA modules here:
   * 🔗 **[LTAP CWA Executables Folder (Google Drive)](https://drive.google.com/drive/folders/1l8dB4BGKVjqPMrvA5ZCLvafRNtTOCFew?usp=drive_link)**

---

## ⚠️ Methodological Guidelines

> [!IMPORTANT]
> **Critical recommendations for data handling & preprocessing:**
> - Apply **Spectral Pretreatments** (SNV, MSC, Savitzky-Golay) *before* variable scaling or centering to ensure scatter corrections operate on raw intensity profiles.
> - Use **Comparative PCA** in the Diagnostic Tools tab to verify whether a given pretreatment reduces unwanted physical variance without eliminating chemical discrimination.
> - Remove **Zero-Variance Columns** and handle missing values before feeding datasets into downstream classification or multivariate calibration models.

---

## 📜 License & Intellectual Property Protection

> [!CAUTION]
> **All Rights Reserved — Intellectual Property Protection (INPI)**
> 
> This software, its interface designs, compiled binaries, and underlying analytical workflows are protected under Intellectual Property laws (Brazilian Software Law No. 9.609/98 and Industrial Property Law No. 9.279/96) and registered at the **National Institute of Industrial Property (INPI)**.

### **Terms of Use & Protection Clause:**
1. **Mandatory Attribution & Citation:** Any academic work, scientific article, technical report, software integration, or presentation utilizing or referencing this application **must explicitly credit** the authors (**Bernardo Cardeal Darzé, I. C. A. Lima, José Licarion Pinto Segundo Neto, Aderval Severino Luna**) and the **Process Analytical Technology Laboratory ([LTAP-UERJ](https://www.ltapuerj.com.br/))**, and cite the published scientific paper:
   > B.C. Darzé, I.C.A. Lima, L. Pinto, A.S. Luna, *Chemometrics web app part 1: data handling*, Chemometrics and Intelligent Laboratory Systems, 231 (2022) 104696. DOI: [10.1016/j.chemolab.2022.104696](https://doi.org/10.1016/j.chemolab.2022.104696)
2. **Prohibition of Unauthorized Reproduction & Redistribution:** Copying, modifying, decompiling, reverse engineering, re-licensing, sub-licensing, mirroring, or redistributing the binary executables or deployment packages without explicit prior written consent from LTAP-UERJ is strictly prohibited.
3. **Non-Commercial Use Only:** The application may only be used for personal, educational, or non-commercial academic research purposes unless a specific commercial license has been granted by LTAP-UERJ.
4. **Disclaimer of Liability:** LTAP-UERJ and the developers accept no responsibility or liability for damages, misinterpretation, or loss resulting from the use of this software or its generated datasets. The software is provided "as is", without warranties of any kind.

For licensing inquiries or commercial use permissions, please contact [licarion@gmail.com](mailto:licarion@gmail.com) or [ltapuerj@gmail.com](mailto:ltapuerj@gmail.com).

---

## 📧 Contact & Institutional Support

**[Process Analytical Technology Laboratory (LTAP/UERJ)](https://www.ltapuerj.com.br/)**

We acknowledge financial and institutional support from **UERJ**, **FAPERJ** (JCNE and CNE research scholarships), **CNPq** (Universal Grant), and **CAPES** (Finance Code 001).

---

<p align="center">
  <a href="https://www.ltapuerj.com.br/">LTAP-UERJ</a> •
  <a href="https://www.uerj.br/">UERJ</a> •
  <a href="https://www.faperj.br/">FAPERJ</a> •
  <a href="https://www.gov.br/cnpq/pt-br">CNPq</a> •
  <a href="https://www.gov.br/capes/pt-br">CAPES</a>
</p>
```
