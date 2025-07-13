# Titanic-EDA-Dashboard-Creation-in-PowerBI


## 📌 Project Objective

The goal is to analyze the Titanic passenger data to understand survival patterns based on factors such as **gender, age, passenger class, fare**, and more. The project uses Python for data wrangling and Power BI for interactive dashboards.

---

## 📊 Dataset Description

The dataset contains information on passengers aboard the Titanic, with the following key features:

| Column Name        | Description |
|--------------------|-------------|
| `PassengerId`      | Unique ID for each passenger |
| `Survived`         | Survival status (0 = No, 1 = Yes) |
| `Pclass`           | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| `Name`             | Passenger name |
| `Sex`              | Gender |
| `Age`              | Age in years |
| `SibSp`            | Number of siblings/spouses aboard |
| `Parch`            | Number of parents/children aboard |
| `Ticket`           | Ticket number |
| `Fare`             | Passenger fare |
| `Cabin`            | Cabin number (many missing values) |
| `Embarked`         | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## 🧹 Data Cleaning & Preprocessing (Python)

Performed using `Titanic EDA.ipynb`, the key steps include:

- **Handling missing values**:
  - Filled missing `Age` values using median imputation
  - Replaced missing `Embarked` values with the most common port
  - Dropped or marked missing `Cabin` values
- **Encoding categorical variables**:
  - Converted `Sex` and `Embarked` using label encoding / one-hot encoding
- **Feature engineering**:
  - Extracted titles from `Name`
  - Created a new `FamilySize` feature (SibSp + Parch + 1)
- **Outlier handling** for `Fare` and `Age`
- **EDA**: Univariate and bivariate analysis using `seaborn`, `matplotlib`, and `pandas`

---

## 📈 Power BI Dashboard

The interactive report (see `Titanic Report.pbix`) includes:

- 📊 **Survival analysis** by class, gender, age, and embarkment port
- 🧍‍♂️ **Demographics distribution** (age distribution, fare, etc.)
- ⚖️ **Comparison charts** (stacked bar, pie, histogram)
- 🌐 **Slicers and filters** to dynamically explore data

### Key Insights:

- Higher survival rate among females and 1st class passengers
- Children had a better chance of survival than adults
- Passengers who embarked from Cherbourg had higher survival rates

## 🛠️ Tools & Technologies Used
Python (Pandas, NumPy, Seaborn, Matplotlib)

Power BI Desktop

Jupyter Notebook

## 🙌 Acknowledgement
Dataset: Kaggle Titanic Dataset

Visualization inspiration from Kaggle & community notebooks
