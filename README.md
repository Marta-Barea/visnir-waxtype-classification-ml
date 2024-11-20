# Rapid Classification of Petroleum Waxes: A Vis-NIR Spectroscopy and Machine Learning Approach

## Description

This repository contains the source code for all data processing and the application of machine learning algorithms used in the article "Rapid Classification of Petroleum Waxes: A Vis-NIR Spectroscopy and Machine Learning Approach".

---

## 📂 Repository Structure

- `spectra/`: Folder containing the spectra data.
- `supervised algorithms/`: Source code for all the supervised machine learning models and experiments.
- `unsupervised algorithms/`: Source code related to unsupervised learning techniques and clustering.
- `App/`: A Shiny application to demonstrate and visualize the findings.

## 🛠️ **System Requirements**

### Software
- **R version 4.2.0** 
- RStudio (optional but recommended)

### Packages

- **prospectr (version 0.2.3)**: Used for calculating the first derivative for each sample spectrum with the `savitzkyGolay` function.
- **stats (version 4.1.2)**: Utilized for HCA with the `hclust` function, PCA with the `prcomp` function, and one-way ANOVA with the `aov` function.
- **cluster (version 2.1.2)**: Linkage method selection for the HCA established using the `agnes` function.
- **factoextra (version 1.0.7)**: Used for visualizing HCA results with the `fviz_dend` function and for extracting and visualizing the PCA result with the `fviz_eig` function.
- **ggplot2 (version 3.3.5)**: Employed for plotting the scores and loadings of the PCA with the `ggplot` function and generating the spectralprint radar chart.
- **caret (version 6.0-90)**: Utilized for developing the SVM and RF models.
- **graphics (version 4.1.2)**: The `filled.contour` function was used to generate the contour plot for the SVM model.
- **ggiraphExtra (version 0.3.0)**: Assisted in generating the spectralprint radar chart.
- **shiny (version 1.7.1)**: Utilized for developing the web application.

## ⚙️ How to Use This Repository

### Clone the Repository


   <pre markdown="1"> ```bash
                         git clone https://github.com/Marta-Barea/visnir-waxtype-classification-ml
                         cd visnir-waxtype-classification-ml </pre>

### Running the Shiny Application
1. Place `app.R`, `svm.rds`, `svr.rds`and `test_data.xlsx` in the same folder.
2. In your R console, run: 
   
   <pre markdown="1"> ```R 
                         shiny::runApp("app.R") </pre>

3. Use the web interface to:
- 📁 **Upload** `.csv` or `.xlsx` data files.
- 🛠️ **Preprocess** data using advanced filtering techniques.
- 🤖 **Predict** wax type with AI.

---

### 📂 **Example Dataset**
A sample dataset (`test_data.xlsx`) is included for demonstration purposes. It contains Vis-NIR spectral readings and hydroprocessing grades for various wax samples.


---

### 🤝 **Contributors**
- **University of Cádiz (AGR-291 Research Group)**
  - Specializing in hydrocarbon characterization and spectroscopy.

---

### 📜 **License**
This project is licensed under the GNU GENERAL PUBLIC License. See `LICENSE` for details.

