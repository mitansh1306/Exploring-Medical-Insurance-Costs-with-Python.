# 🏥 Insurance Cost Analysis Using Python

## 📌 Project Overview

This project focuses on analyzing a medical insurance dataset to understand the factors associated with **medical insurance charges**.

Using Python-based data analysis and statistical techniques, the project covers the complete workflow from **data exploration and cleaning to feature engineering, visualization, correlation analysis, and statistical testing**.

---

## 📊 Dataset

The dataset contains **1,338 records and 7 variables**:

| Column | Description |
|---|---|
| `age` | Age of the individual |
| `sex` | Gender |
| `bmi` | Body Mass Index |
| `children` | Number of children/dependents |
| `smoker` | Smoking status |
| `region` | Residential region |
| `charges` | Medical insurance charges |

### Dataset Characteristics

- **Rows:** 1,338
- **Columns:** 7
- **Missing values:** None
- **Duplicate records:** 1 duplicate removed during cleaning
- **Final records after cleaning:** 1,337

---

## 🛠️ Technologies & Libraries

- **Python**
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **SciPy** – Statistical analysis

---

## 🔎 Project Workflow

### 1. Data Loading

The dataset was imported using Pandas:

```python
df = pd.read_csv('insurance.csv')
```

### 2. Exploratory Data Analysis

Initial exploration included:

- Dataset dimensions
- Data types
- Descriptive statistics
- Column inspection
- Missing-value analysis
- Distribution analysis
- Categorical-value analysis

### 3. Data Cleaning

The dataset was checked for:

- Missing values
- Duplicate records
- Incorrect data types
- Categorical variables requiring encoding

One duplicate record was identified and removed.

### 4. Data Preprocessing

Categorical variables were converted into numerical representations where required.

For example:

```python
df_cleaned['sex'] = df_cleaned['sex'].map({
    "male": 0,
    "female": 1
})
```

Additional preprocessing and feature engineering were performed to prepare the dataset for statistical analysis.

### 5. Data Visualization

Visualizations were created using **Matplotlib and Seaborn** to investigate relationships between variables and insurance charges.

Examples include:

- Distribution plots
- Count plots
- Box plots
- Scatter plots
- Correlation heatmaps

### 6. Correlation Analysis

A correlation matrix was generated to examine relationships between numerical variables:

```python
sns.heatmap(
    df.corr(numeric_only=True),
    annot=True
)
```

This helped identify relationships between variables and the target variable, `charges`.

### 7. Statistical Analysis

Statistical techniques were also used to evaluate relationships between categorical variables and insurance charges.

The project includes statistical testing such as:

- **Pearson correlation**
- **Chi-square testing**

These techniques provide a more quantitative approach to understanding relationships in the dataset.

---

## 📈 Key Analysis Areas

The project investigates how insurance charges vary with factors such as:

- Age
- BMI
- Smoking status
- Number of children
- Gender
- Region

The analysis combines **EDA + visualization + statistical testing** rather than relying only on visual observations.

---

## 💡 Key Learnings

Through this project, I strengthened my practical understanding of:

- Exploratory Data Analysis
- Data cleaning
- Handling duplicate records
- Categorical encoding
- Feature engineering
- Data visualization
- Correlation analysis
- Statistical hypothesis testing
- Using Python for real-world datasets

---

## 📂 Project Structure

```text
Insurance-Cost-Analysis/
│
├── insurance.csv
├── project-1.ipynb
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/Insurance-Cost-Analysis.git
```

### 2. Navigate to the project directory

```bash
cd Insurance-Cost-Analysis
```

### 3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
project-1.ipynb
```

---

## 🎯 Project Objective

The primary objective of this project was to develop a structured **data-analysis workflow using Python**, starting from raw data and progressing through cleaning, exploration, visualization, feature engineering, and statistical analysis.

---

## 👨‍💻 Skills Demonstrated

**Python | Pandas | NumPy | Matplotlib | Seaborn | SciPy | EDA | Data Cleaning | Feature Engineering | Statistical Analysis | Data Visualization**

---

⭐ If you found this project useful, feel free to explore the repository and connect with me.
