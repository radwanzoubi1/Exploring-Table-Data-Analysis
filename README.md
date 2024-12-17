# Exploring Table Data Analysis

This project focuses on **Exploratory Data Analysis (EDA)** of a tabular dataset related to **Autism Spectrum Disorder (ASD)**. The dataset includes behavioral and demographic features collected from a screening process to detect ASD traits in toddlers. The project involves preprocessing the dataset, analyzing statistical summaries, addressing data quality issues, visualizing key features, and interpreting meaningful insights.

---

## About the Dataset

### Domain:
- **Autism Spectrum Disorder (ASD)**: A neurodevelopmental condition associated with high healthcare costs. Early diagnosis significantly reduces these costs; however, current diagnosis methods are time-consuming and expensive.
- **Purpose**: This dataset addresses the urgent need for cost-effective, time-efficient, and accessible screening methods to help health professionals identify ASD traits in toddlers.

### Dataset Overview:
- **Data Type**: Predictive and Descriptive (Nominal, Binary, and Continuous)
- **Task**: Classification (but can also be used for clustering and feature assessment)
- **Area**: Medical, Health, and Social Science
- **Number of Records**: 1,054 instances
- **Number of Features**: 18 attributes, including the class variable
- **Missing Values**: No missing values

### Attribute Information:
1. **A1 - A10**: 
   - Behavioral questions (Q-Chat-10) with answers mapped to binary values (`1` or `0`).
   - Mapping logic:
     - For Questions **1-9**: If the response is **"Sometimes, Rarely, or Never"**, assign `1`.
     - For Question **10**: If the response is **"Always, Usually, or Sometimes"**, assign `1`.
   - **Q-Chat-10 Score**: A score of more than `3` indicates potential ASD traits; otherwise, no ASD traits are observed.

2. **Remaining Features**:
   - Collected from the "submit" screen in the **ASDTests** screening app.
   - Includes demographic and categorical variables related to the toddler and family.

3. **Class Variable**:
   - Automatically assigned based on the screening score:
     - **Class `1`**: ASD traits detected.
     - **Class `0`**: No ASD traits observed.

### Citation:
If you use this dataset, please cite the following relevant papers:
1. Tabtah, F. (2017). *Autism Spectrum Disorder Screening: Machine Learning Adaptation and DSM-5 Fulfillment*. Proceedings of the 1st International Conference on Medical and Health Informatics 2017, pp.1-6. Taichung City, Taiwan, ACM.  
2. Thabtah, F. (2017). *ASDTests. A mobile app for ASD screening*. www.asdtests.com [Accessed December 20th, 2017].  
3. Thabtah, F. (2017). *Machine Learning in Autistic Spectrum Disorder Behavioural Research: A Review*. Informatics for Health and Social Care Journal.  
4. Thabtah, F., Kamalov, F., Rajab, K. (2018). *A new computational intelligence approach to detect autistic features for autism screening*. International Journal of Medical Informatics, Volume 117, pp. 112-124.

---
### Data Source:

- Autism Screening for Toddlers:
https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers
---

## Project Objectives

1. **Business Understanding**:
   - Identify the purpose and relevance of the dataset.
   - Analyze the prediction task and its impact on ASD screening.

2. **Data Understanding**:
   - Explore the dataset structure, types, and statistical summaries.
   - Address data quality issues, such as duplicates or inconsistencies.

3. **Data Visualization**:
   - Visualize feature distributions and identify meaningful patterns.
   - Explore feature relationships using various plots.

4. **Exploratory Questions**:
   - Pose and answer three key questions relevant to the dataset.

5. **Exceptional Analysis**:
   - Implement **UMAP** (Uniform Manifold Approximation and Projection) for dimensionality reduction.

---

## Questions Explored

1. **What is the distribution of ASD traits (class variable) across different age groups?**
   - Visualized using histograms and boxplots.

2. **How do categorical features like family history and jaundice influence ASD outcomes?**
   - Analyzed using bar charts and comparison plots.

3. **What is the relationship between the Q-Chat-10 score and the ASD outcome?**
   - Explored using scatter plots and KDE (Kernel Density Estimation) plots.

---

## Tools and Libraries Used

The following libraries and tools were used for data processing, analysis, and visualization:

- **Python 3.11.9**: Programming language.
- **Jupyter Notebook**: Interactive coding environment.
- **Pandas**: Data manipulation and preprocessing.
- **NumPy**: Numerical operations.
- **Matplotlib**: Data visualization.
- **Seaborn**: Statistical data visualization.
- **UMAP**: Dimensionality reduction method for high-dimensional data.
- **nbconvert**: Exporting the notebook to an HTML report.

---

## Project Structure

```plaintext
.
├── Exploring-Table-Data-Analysis.ipynb   # Main Jupyter Notebook with code and visualizations
├── Toddler Autism dataset July 2018.csv  # Dataset used for analysis
├── README.md                             # Project documentation
```

## How to Run
**1. Clone the Repository:**
```md
git clone https://github.com/radwanzoubi1/Exploring-Table-Data-Analysis.git
cd Exploring-Table-Data-Analysis
```

**2. Install Dependencies:**

```bash
pip install pandas matplotlib seaborn numpy umap-learn
```

**3. Run the Notebook:**

- **Open the Jupyter Notebook**:

```bash
jupyter notebook Exploring-Table-Data-Analysis.ipynb
```

- Run all cells to reproduce the analysis.

