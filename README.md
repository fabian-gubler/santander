# Santander - Data Science Kaggle Competition

### :books: **Final Project Report**:  
**[Data Science Project Report – Santander Customer Transaction Prediction](https://raw.githubusercontent.com/fabian-gubler/santander/main/Project_Report.pdf)** – Click the link for a detailed report of our Santandar Kaggle Competition

---

## Project Description

This repository includes the complete solution to the Kaggle competition on **Santander Customer Transaction Prediction**. The challenge aimed to predict which customers will make specific transactions in the future, based on anonymized features, regardless of the transaction amount.

We focused on building robust machine learning models using **LightGBM (LGBM)** and **Convolutional Neural Networks (CNN)**, employing feature engineering and data augmentation techniques to optimize performance.

Kaggle competition overview: [Santander Kaggle Competition](https://www.kaggle.com/competitions/santander-customer-transaction-prediction/overview).

## Installation

To get started with this project, you’ll need **Python 3.11.0** or higher. We recommend using a virtual environment to manage dependencies. Follow these steps to set it up:

```bash
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

The `requirements.txt` includes all necessary dependencies to run the **Jupyter notebooks** included in the project. We also recommend using **JupyterLab** for running and exploring the notebooks:

```bash
pip install jupyterlab
jupyter lab
```

This will open JupyterLab in your browser, where you can navigate to the project’s notebooks and run them to reproduce the results.

---

## Dataset Information

The dataset for this project was sourced from the **Kaggle Santander Customer Transaction Prediction** competition. It can be found in the `data` directory, where it is divided into:

- **train.csv**: The training set with labels
- **test.csv**: The test set without labels
- **sample_submission.csv**: A sample submission file provided by Kaggle

For more details or to download the data directly, visit the competition page: [Santander Kaggle Data](https://www.kaggle.com/c/santander-customer-transaction-prediction/data).

## Repository Contents

This repository is organized as follows:

### 1. **Data**
- Contains raw and processed data files for training and testing the models.

### 2. **Engineering**
- This folder contains notebooks for **Feature Engineering** (version 1 and version 2), where we implemented techniques such as unique counts and reverse feature engineering.

### 3. **Exploration**
- The exploratory data analysis (EDA) notebook can be found here. This analysis was crucial for shaping our feature engineering decisions and model development.

### 4. **Models**
- Includes subfolders for different model types, focusing primarily on **LGBM** and **CNN** models. Additional archives contain early-stage models, and the blending folder holds the notebook used for our final score blending of the best CNN and LGBM models.

### 5. **Submission**
- Contains various model-generated predictions for Kaggle submission, including the final blend of our best LGBM and CNN models in `submission_blending.csv`.

## Key Learnings

1. **Feature Engineering**: Feature engineering had a significant impact on model performance. Techniques like unique counts and reverse features helped us push our models beyond the baseline.
   
2. **Model Blending**: Combining CNN and LGBM models via linear blending proved to be a successful strategy, improving our final AUC score.

3. **Data Imbalance Handling**: Oversampling the minority class (customers with transactions) was essential to prevent bias and optimize model generalization.

4. **Performance Optimization**: Extensive experimentation with hyperparameters and the application of data augmentation techniques helped us fine-tune our models and achieve high AUC scores.

---

Feel free to explore the code and try the models yourself. Should you have any questions or feedback, we would be happy to connect!
