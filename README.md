# Chemometrics Web App - Data Handling (Part 1)

![Status](https://img.shields.io/badge/Status-Active-green)
![Version](https://img.shields.io/badge/Release-V3-orange)
![License](https://img.shields.io/badge/License-Patented-blue)
![R](https://img.shields.io/badge/Language-R-blue.svg)

Developed by the **Process Analytical Technology Laboratory (LTAP-UERJ)**, this application is a comprehensive tool for the treatment, preprocessing, and visualization of chemometric data.

---

## 🔗 Quick Links

* **Online Version:** [Access the Web App](https://ltap.shinyapps.io/data_handling/)
* **Scientific Article:** [ScienceDirect - Chemometrics and Intelligent Laboratory Systems](https://www.sciencedirect.com/science/article/pii/S0169743922002076)
* **Support/Feedback:** [ltapuerj@gmail.com](mailto:ltapuerj@gmail.com)

---

## 🆕 Version History (Change Log)

### **V3 - Current Release**
* **Diagnostic Tools:** The "Interactive Plots" tab has been upgraded to the "Diagnostic Tools" section, integrating:
    * **Comparative PCA:** Simplified tool for exploratory and diagnostic analysis.
    * **Argument Restrictions:** Streamlined parameters for easier pretreatment configuration.
* **Variable Preprocessing:** Added **Median Centering** for more robust normalization workflows.
* **Data Transposition Tool:** New functionality to easily switch between samples in rows or columns.

### **V2 - Improved Compatibility**
* **Stability:** Automatic omission of normality tests in classes with fewer than 5 samples to prevent crashes.
* **Spectral Refactoring:** Initial implementation of diagnostic tool logic.

---

## 🚀 Key Features

* **Descriptive Analysis:** General statistics, variable/class analysis, and multivariate normality tests.
* **Data Imputation:** Simple substitutions, Random Forest, KNN, SVD, and PCA Imputation (Nipals, Bayesian, Probabilistic).
* **Spectral Transformation:**
    * Smoothing & Derivatives (Savitzky-Golay, Moving Average).
    * Scatter Correction (SNV and MSC).
    * Baseline Correction (ALS, Polynomial, Low-Pass FFT, etc.).
    * Peak Alignment (Parametric Time Warping).
* **Spectral Visualization:** High-quality 2D images and interactive plots.
* **Variable Preprocessing:** Auto-scaling, Mean Centering, Median Centering, Box-Cox, and Yeo-Johnson transformations.

---

## 💾 Installation & Usage

### **Distribution Models**
* **Version 1.0:** Open source and free access.
* **Versions V2 & V3:** Available as executables under a **30-day Trial** period. Continued use requires licensing from LTAP-UERJ.

### **How to Run (R/RStudio)**
After the installation process, simply open the application in the RStudio environment and click the "Run App" button.

---

## ⚖️ Legal Notice & Intellectual Property

> [!IMPORTANT]
> **Patent Notice:** This software and its interfaces are protected by patent. All rights are reserved to **LTAP-UERJ**. Supporting documentation is available within this repository.

* **Disclaimer:** LTAP-UERJ is not responsible for any damages resulting from the use of this interface or the interpretation of the generated results. The software is provided "as is".
* **Academic Citation:** If this software is useful for your research, please cite:
    * *Chemometrics and Intelligent Laboratory Systems, 2022. DOI: [10.1016/j.chemolab.2022.104654](https://doi.org/10.1016/j.chemolab.2022.104654)*

---

## 📧 Contact & Team

**Process Analytical Technology Laboratory (LTAP/UERJ)**

| Name | Email |
| :--- | :--- |
| **Bernardo Cardeal** | bernardocardeal@outlook.com |
| **Licarion Pinto** | licarion@gmail.com |
| **Aderval Luna** | adsluna@gmail.com |

---
