# Titanic Disaster Analysis Using Pandas

This project performs an in-depth analysis of the Titanic dataset using Python and the Pandas library. The analysis includes data exploration, data cleaning, feature engineering, and basic statistical insights.

---

## 📂 Dataset
The dataset used is the **Titanic passenger dataset**, which contains information about passengers such as:

- Passenger Class (`Pclass`)
- Name (`Name`)
- Sex (`Sex`)
- Age (`Age`)
- Number of siblings/spouses aboard (`SibSp`)
- Number of parents/children aboard (`Parch`)
- Fare (`Fare`)
- Survival status (`Survived`)

---

## 🛠 Tools & Libraries
- **Python 3.x**
- **Pandas** for data analysis


---

## 🔍 Steps Performed

### 1. Loading and inspecting the dataset
- Checked the **first and last 5 rows** using `head()` and `tail()`
- Checked **shape, data types, and memory info** using `shape` and `info()`
- Checked **summary statistics** with `describe()`

### 2. Handling missing values
- Dropped **irrelevant columns**: `Cabin` and `Embarked`
- Filled missing values in `Age` with `0` using `fillna()`

### 3. Feature Engineering
- Created **one-hot encoding** for the `Sex` column
- Created a new column **family** = `SibSp + Parch` (total family members onboard)
- Created **fare_per_person** = `Fare / (family + 1)`

### 4. Exploratory Analysis

**Passenger Classes Distribution:**

| Class        | Number of Passengers |
|-------------|--------------------|
| First Class  | 216                |
| Second Class | 184                |
| Third Class  | 491                |

**Gender Distribution:**

| Gender | Number of Passengers |
|--------|--------------------|
| Male   | 577                |
| Female | 314                |

**Survival Rate by Class:**

| Class        | Survival Rate |
|-------------|---------------|
| First Class  | 0.63          |
| Second Class | 0.47          |
| Third Class  | 0.24          |

**Total Survivors and Non-Survivors:**

- **Total Survivors:** 342  
- **Total Non-Survivors:** 549

---

## 🧩 Key Insights
- First class passengers had the **highest survival rate**.  
- Female passengers were **more likely to survive** than males.  
- Families with more members paid **less fare per person** on average.  

---