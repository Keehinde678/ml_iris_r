# Assignment 5 – Machine Learning in Python (or R)

**Author**: [Kehinde Soetan]  
**Email**: [soetan.6@osu.edu]  
**Date**: [07/31/2025]  
**Environment**: See `environment.yml`  
**Description**:  

This project demonstrates the process of building, evaluating, and comparing machine learning models on the **Iris dataset**. It focuses on  **R (caret/tidymodels)** workflow, covering data preparation, model training, validation, and performance assessment.

The goal is to explore multiple classification algorithms, understand their performance differences, and practice best practices in model evaluation such as cross-validation and confusion matrix analysis.

## Workflow and Methods

1. **Data Loading and Exploration**
   - Loaded the Iris dataset.
   - Explored dataset structure, including number of samples, classes, and features.
   - Conducted basic descriptive statistics and visualizations (e.g., histograms, scatterplots).

2. **Data Preprocessing**
   - Split the dataset into **training (80%)** and **validation (20%)** sets.
   - Checked for missing values and normalized features where necessary.

3. **Model Training**
   - Trained multiple classification models:
     - **Linear Discriminant Analysis (LDA)**
     - **Random Forest**
     - **Decision Tree (rpart)**
     - **Support Vector Machine (SVM)** (optional in Python workflow)
   - Used **10-fold cross-validation** for model evaluation.

4. **Model Evaluation**
   - Summarized cross-validation results including **mean accuracy** and **standard deviation**.
   - Selected the best performing model based on accuracy (LDA in our analysis: 97.5% ± 4%).
   - Tested the final model on the **validation set** for an independent accuracy check.
   - Generated **confusion matrices** to evaluate sensitivity, specificity, and class-wise performance.

5. **Results**
   - **LDA Model** achieved:
     - Mean cross-validation accuracy: **97.5% ± 4%**
     - Validation accuracy: **100%**
     - Perfect sensitivity, specificity, and balanced accuracy for all three species.
   - Other models (Random Forest, rpart) were trained and compared but LDA remained the most reliable for this dataset.

6. **Conclusion**
   - Linear Discriminant Analysis was the most accurate and reliable model for classifying Iris species.
   - Cross-validation and validation checks confirmed model robustness.
   - The project demonstrates the importance of systematic evaluation and comparison of machine learning models.

## Project Structure
my_r_project/

├── data/  Dataset files

├── notebooks/  Jupyter notebooks or RMarkdown files

├── outputs/  Model outputs, plots, and results

├── environment.yml  Environment setup

└── README.md  This file

## Usage
1. Clone the repository:  
   ```bash
   git clone <repository_url>
Navigate to the project folder:

cd my_r_project
Set up the environment:
conda env create -f environment.yml
Activate the environment:
conda activate my_r_project
Open the notebook in Jupyter or RStudio and run the analysis step by step.

Dependencies
Python: scikit-learn, pandas, numpy, matplotlib, seaborn (if Python workflow)

R: caret, randomForest, rpart, e1071, ggplot2 (if R workflow)

License
This project is released under the MIT License.




