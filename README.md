# Chemometrics Web App - Data Handling (Part 1)

![Status](https://img.shields.io/badge/Status-Active-green)
![Version](https://img.shields.io/badge/Release-V3-orange)
![License](https://img.shields.io/badge/License-Patented-blue)

Esta aplicação, desenvolvida pelo **LTAP-UERJ**, é uma ferramenta completa para o tratamento, pré-processamento e visualização de dados quimiométricos.

🔗 **Acesse a versão online:** [Clique aqui](https://ltap.shinyapps.io/data_handling/)  
📖 **Artigo Científico:** [ScienceDirect - Chemometrics and Intelligent Laboratory Systems](https://www.sciencedirect.com/science/article/pii/S0169743922002076)  
📝 **Feedback:** Ajude-nos a melhorar nos enviando sugestões para o ltapuerj@gmail.com

---

## 🆕 Novidades das Versões (Change Log)

### **V3 - New Release**
* **Diagnostic Tools:** A aba "Interactive Plots" foi substituída pela seção "Diagnostic Tools", que agora integra:
    * **Comparative PCA:** Ferramenta simplificada para análise exploratória e diagnóstica.
    * **Argument Restrictions:** Simplificação de parâmetros para facilitar o uso no pré-tratamento.
* **Variable Preprocessing:** Adicionada a opção de **Median Centering** (Centramento na Mediana), tornando o fluxo de normalização mais robusto.
* **Data Transposition Tool:** Nova funcionalidade para alternar entre amostras em linhas ou colunas.

### **V2 - Improved Compatibility**
* **Correção de Crashes:** Omissão automática de testes de normalidade em classes com menos de 5 amostras.
* **Refatoração Espectral:** Introdução inicial da lógica de ferramentas de diagnóstico.

---

## 🚀 Funcionalidades Principais

* **Descriptive Analysis:** Informações gerais, análise por variável/classe e testes de normalidade multivariada.
* **Data Imputation:** Substituições simples, Random Forest, KNN, SVD e PCA Imputation (Nipals, Bayesian, Probabilistic).
* **Spectral Transformation:**
    * Suavização e Derivadas (Savitzky-Golay, Moving Average).
    * Correção de Espalhamento (SNV e MSC).
    * Correção de Linha de Base (ALS, Polynomial, Low-Pass FFT, etc.).
    * Alinhamento de Picos (Parametric Time Warping).
* **Spectral Visualization:** Geração de imagens 2D personalizadas e gráficos interativos.
* **Variable Preprocessing:** Auto-escalonamento, Centramento, Transformações Box-Cox e Yeo-Johnson.

---

## 💾 Instalação e Licenciamento

### **Modelos de Distribuição**
* **Versão 1.0:** Código aberto e acesso livre.
* **Versões V2 e V3:** Disponíveis como executáveis em regime **Trial de 30 dias**. Após o período de teste, o uso requer licenciamento junto ao LTAP-UERJ.

### **Instalação via R/RStudio**
1. Instale o R e RStudio.
2. Baixe e execute o arquivo `Data_handling_Packages.R` deste repositório para instalar as dependências.
3. Baixe o código da aplicação e clique em **"Run App"**.

---

## ⚖️ Aviso Legal e Propriedade Intelectual

**Aviso de Patente:** Este software e suas interfaces são protegidos por patente. A documentação comprobatória encontra-se nos arquivos deste repositório. Todos os direitos reservados ao **LTAP-UERJ**.

**Isenção de Responsabilidade:** O uso deste software é de inteira responsabilidade do usuário. O software é fornecido "no estado em que se encontra", sem garantias de qualquer tipo.

**Citação Acadêmica:** 
Se este software for útil para sua pesquisa, por favor, faça a citação do artigo [ScienceDirect - Chemometrics and Intelligent Laboratory Systems](https://www.sciencedirect.com/science/article/pii/S0169743922002076)  

## 📧 Contato e Equipe
* **Bernardo Cardeal:** bernardocardeal@outlook.com
* **Licarion Pinto:** licarion@gmail.com
* **Aderval Luna:** adsluna@gmail.com

## Usage
After the instalation process the app usage consist in simple open the app in Rstudio enviroment and click the Run App button.
