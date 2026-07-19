# Chemometrics Web App — Data Handling (Part 1)

![Status](https://img.shields.io/badge/Status-Active-green)
![Version](https://img.shields.io/badge/Release-V3-orange)
![License](https://img.shields.io/badge/License-Proprietary%20%2F%20INPI%20Registered-red.svg)
![R](https://img.shields.io/badge/Language-R-blue.svg)

Developed by the **Process Analytical Technology Laboratory (LTAP-UERJ)**, this application is a comprehensive tool for the treatment, preprocessing, imputation, spectral transformation, and visualization of chemometric data.

---

## 🔗 Quick Links

* **Online Version:** [Access the Web App](https://ltap.shinyapps.io/data_handling/)
* **Scientific Article:** [ScienceDirect — Chemometrics Web App Part 1: Data Handling](https://doi.org/10.1016/j.chemolab.2022.104696)
* **Software Registration (INPI):** [LTAP-UERJ CWA — Registros de Software](https://sites.google.com/view/ltap-uerj/cwa)
* **Support/Feedback:** [ltapuerj@gmail.com](mailto:ltapuerj@gmail.com)

---

## 🆕 Version History (Change Log)

### **V3 — Current Release**
* **Diagnostic Tools:** Upgraded "Interactive Plots" to a comprehensive "Diagnostic Tools" section, integrating:
    * **Comparative PCA:** Streamlined tool for exploratory diagnostic analysis before and after pretreatment.
    * **Argument Restrictions:** Simplified parameters for safer and easier pretreatment configuration.
* **Variable Preprocessing:** Added **Median Centering** for robust normalization workflows.
* **Data Transposition Tool:** Integrated functionality to easily toggle between samples in rows or columns.
* **Session Management:** Save and restore workspace states in `.RData` format for seamless inter-module data transfer.

### **V2 — Improved Compatibility & Refactoring**
* **Normality Test Guard:** Automatic omission of normality tests in classes with fewer than 5 samples to prevent execution crashes.
* **Spectral Diagnostic Engine:** Initial implementation of diagnostic tool logic for spectral signal inspection.

### **V1 — Initial Release**
* Fundamental implementation of descriptive statistics, missing data imputation, Savitzky-Golay derivatives, and basic variable scaling.

---

## 🚀 Key Features

### 📊 Descriptive Analysis & Normality Tests
* **Summary Statistics:** Central tendency, dispersion, skewness, and kurtosis per variable and per sample class.
* **Class & Variable Distribution:** Class frequencies, missing value proportions, and boxplot visualizations.
* **Multivariate Normality:** Henze-Zirkler, Royston, and Mardia multivariate normality tests.

### 🧩 Data Imputation
* **Simple Substitutions:** Mean, Median, and Minimum/Maximum substitution.
* **Machine Learning & Statistical Imputation:** K-Nearest Neighbors (KNN), Random Forest (`missForest`), and Singular Value Decomposition (SVD).
* **PCA Imputation:** NIPALS, Bayesian PCA, and Probabilistic PCA imputation methods.

### 📈 Spectral Transformations & Signal Pretreatment
* **Smoothing & Derivatives:** Savitzky-Golay smoothing and derivatives (1st and 2nd order), Moving Average.
* **Scatter Correction:** Standard Normal Variate (SNV) and Multiplicative Scatter Correction (MSC).
* **Baseline Correction:** Asymmetric Least Squares (ALS), Polynomial fitting, Low-Pass FFT, and Rolling Ball baseline estimation.
* **Peak Alignment:** Parametric Time Warping (PTW) for spectral band alignment.

### 🎛️ Variable Preprocessing & Normalization
* **Scaling & Centering:** Mean Centering, Median Centering, Auto-scaling (Standardization), Range Scaling, and Pareto Scaling.
* **Normality-Inducing Transformations:** Box-Cox and Yeo-Johnson transformations with automatic lambda estimation.

---

## 💾 Installation & Usage

### **How to Run (R/RStudio)**
After downloading or cloning the unencrypted source files, open the application in RStudio and click the **"Run App"** button at the top right of the editor.

### **Distribution Models**
* **Shinyapps Version 01:** Open source and free online access.
* **Desktop Version 01:** Available as an offline standalone executable.

---

## 📜 License & Intellectual Property Protection

> [!CAUTION]
> **All Rights Reserved — Intellectual Property Protection (INPI)**
> 
> This software, its source code, interface designs, visual assets, and underlying analytical workflows are protected under Intellectual Property laws (Brazilian Software Law No. 9.609/98 and Industrial Property Law No. 9.279/96) and registered at the **National Institute of Industrial Property (INPI)**.

### **Terms of Use & Protection Clause:**
1. **Mandatory Attribution & Citation:** Any academic work, scientific article, technical report, software integration, or presentation utilizing or referencing this application **must explicitly credit** the authors (**Paulo Henrique Couto Simões, Julio Cesar Siqueira, Licarion Pinto, Aderval Luna**) and the **Process Analytical Technology Laboratory (LTAP-UERJ)**, and cite the published scientific paper:
   > B.C. Darz, I.C.A. Lima, L. Pinto, A.S. Luna, *Chemometrics web app part 1: data handling*, Chemometrics and Intelligent Laboratory Systems, 231 (2022) 104696. DOI: [10.1016/j.chemolab.2022.104696](https://doi.org/10.1016/j.chemolab.2022.104696)
2. **Prohibition of Unauthorized Reproduction & Redistribution:** Copying, modifying, decompiling, reverse engineering, re-licensing, sub-licensing, mirroring, or redistributing the source code or binary executables without explicit prior written consent from LTAP-UERJ is strictly prohibited.
3. **Non-Commercial Use Only:** The application may only be used for personal, educational, or non-commercial academic research purposes unless a specific commercial license has been granted by LTAP-UERJ.
4. **Disclaimer of Liability:** LTAP-UERJ and the developers accept no responsibility or liability for damages, misinterpretation, or loss resulting from the use of this software or its generated datasets. The software is provided "as is", without warranties of any kind.

For licensing inquiries or commercial use permissions, please contact [ltapuerj@gmail.com](mailto:ltapuerj@gmail.com).

---

## 📧 Contact & Team

**Process Analytical Technology Laboratory (LTAP/UERJ)**

| Name | Email |
| :--- | :--- |
| **Paulo Henrique Couto Simões** | [ph.simoes@gmail.com](mailto:ph.simoes@gmail.com) |
| **Julio Cesar Siqueira** | [juliosiqueira86@hotmail.com](mailto:juliosiqueira86@hotmail.com) |
| **Licarion Pinto** | [licarion@gmail.com](mailto:licarion@gmail.com) |
| **Aderval Luna** | [adsluna@gmail.com](mailto:adsluna@gmail.com) |

---

<p align="center">
  <a href="https://www.ltapuerj.com.br/">LTAP-UERJ</a> •
  <a href="https://www.uerj.br/">UERJ</a> •
  <a href="https://www.faperj.br/">FAPERJ</a> •
  <a href="https://www.gov.br/cnpq/pt-br">CNPq</a> •
  <a href="https://www.gov.br/capes/pt-br">CAPES</a>
</p>
