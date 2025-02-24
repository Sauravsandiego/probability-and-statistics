# **wine quality prediction** using machine learning:

```markdown
# Wine Quality Prediction using Machine Learning

## Project Status: Completed

---

## Installation

1. Clone the repository:
   ```bash
   https://github.com/Sauravsandiego/probability-and-statistics.git
   cd wine-quality-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the project:
   - To train the model:
     ```bash
     python train_model.py
     ```
   - To test the model:
     ```bash
     python test_model.py
     ```

4. The dataset used for training can be downloaded from the [UCI Wine Quality Dataset](https://archive.ics.uci.edu/ml/datasets/Wine+Quality).

---

## Project Objective

The primary objective of this project is to develop a machine learning model capable of predicting wine quality based on its physicochemical properties. This model can assist winemakers in predicting the quality of wine produced using various ingredients and processes, helping improve wine production and quality control.

---

## Contributors

- **Saurav Kumar Subudhi** - Data Scientist
- **Evin Joy** - Data Scientist

---

## Methods Used

- Machine Learning
- Feature Engineering
- Data Preprocessing
- Model Selection & Hyperparameter Tuning
- Synthetic Minority Over-sampling Technique (SMOTE) for handling class imbalance

---

## Technologies

- Python
- scikit-learn
- XGBoost
- CatBoost
- pandas
- NumPy
- Matplotlib
- seaborn
- imbalanced-learn

---

## Project Description

This project focuses on predicting the quality of red wine based on various physicochemical properties. The dataset used comes from the UCI Machine Learning Repository, consisting of **1599** red wine samples, each described by **12** features including acidity, alcohol content, pH, and sugar concentration.

### Dataset Overview:
- **Source**: UCI Machine Learning Repository
- **Variables**: 12 physicochemical attributes (e.g., fixed acidity, volatile acidity, citric acid, residual sugar, pH, alcohol content, etc.)
- **Target**: Quality score on a scale of 0–10
- **Classes**: The quality score is categorized into three labels: Low (0-4), Medium (5-6), and High (7-10).

### Key Steps:
- **Data Cleaning and Preprocessing**: Handled missing values, scaled features using RobustScaler, and categorized quality ratings into three classes.
- **Feature Engineering**: Created polynomial features to capture non-linear relationships and interactions between features.
- **Modeling**: Applied various machine learning models including XGBoost and CatBoost. XGBoost was selected as the final model after hyperparameter tuning, providing the best balance between accuracy and computational efficiency.
- **Handling Class Imbalance**: SMOTE was used to generate synthetic samples for underrepresented classes, ensuring fair model performance across all wine quality levels.

### Key Challenges:
- Class imbalance, where the "Medium" quality class was overrepresented compared to "Low" and "High" quality classes, which was addressed through SMOTE.
- Fine-tuning XGBoost for optimal performance took significant experimentation with hyperparameters.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgments

We would like to thank our instructors for their support and guidance throughout the course. Special thanks to the creators of the UCI Wine Quality Dataset for making the dataset publicly available.
