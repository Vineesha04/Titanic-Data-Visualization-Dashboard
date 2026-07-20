# 🚢 Titanic Data Visualization Dashboard

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal)
![License](https://img.shields.io/badge/License-MIT-green)

A professional exploratory data analysis and visualization project based on the Titanic passenger dataset.

The project demonstrates data cleaning, feature engineering, statistical analysis, visual storytelling, and executive dashboard development using Python.

---

## 📊 Executive Dashboard

![Titanic Executive Dashboard](images/titanic_premium_executive_dashboard.png)

---

## 🎯 Project Objective

The objective of this project is to transform the Titanic passenger dataset into a clear and meaningful visual story.

The analysis explores how passenger characteristics such as gender, class, age, fare, family structure, cabin availability, embarkation port, and social title were associated with survival.

---

## ✨ Project Highlights

- Cleaned and validated the raw Titanic dataset
- Treated missing age values using passenger title and class
- Transformed cabin information into useful analytical features
- Engineered demographic, family, and travel-related variables
- Created 12 publication-quality visualizations
- Developed a premium executive dashboard with KPI cards
- Added exact analytical summary tables
- Exported a cleaned and feature-engineered dataset
- Documented findings, limitations, and future improvements

---

## 🧹 Data Cleaning

The cleaning workflow included:

- Inspecting missing values and duplicates
- Filling missing `Age` values using median age by passenger title and class
- Filling missing `Embarked` values using the mode
- Extracting deck and cabin-availability information
- Removing the original high-missing `Cabin` column after extracting useful features
- Validating numerical and categorical values

---

## 🧠 Feature Engineering

The following features were created:

| Feature | Description |
|---|---|
| `Title` | Passenger title extracted from name |
| `FamilySize` | Total family members aboard, including the passenger |
| `IsAlone` | Indicates whether the passenger travelled alone |
| `TravelStatus` | Human-readable solo or family travel label |
| `FamilyCategory` | Alone, Small Family, or Large Family |
| `AgeGroup` | Passenger age category |
| `FareGroup` | Fare category based on quartiles |
| `CabinKnown` | Indicates whether cabin information was recorded |
| `Deck` | Deck letter extracted from cabin |
| `IsChild` | Indicates whether the passenger was a child |
| `IsMother` | Engineered motherhood indicator |
| `TicketGroupSize` | Number of passengers sharing the same ticket |
| `Surname` | Family surname extracted from the passenger name |

---

## 📈 Key Findings

1. The overall survival rate was approximately **38.4%**.
2. Female passengers had a survival rate of approximately **74.2%**, compared with **18.9%** for male passengers.
3. First-class passengers had the highest class-based survival rate at approximately **63.0%**.
4. Third-class passengers experienced the lowest class-based survival outcome.
5. Passengers travelling with small families achieved the highest family-based survival rate.
6. Higher fares were generally associated with stronger survival outcomes.
7. Passenger titles captured useful demographic and social information.
8. Gender and passenger class produced the largest visible survival differences.

---

## 📷 Selected Visualizations

### Survival by Gender

![Survival by Gender](images/survival_by_gender.png)

### Survival by Passenger Class

![Survival by Passenger Class](images/survival_by_class.png)

### Age Distribution

![Age Distribution](images/age_distribution.png)

### Gender and Passenger Class

![Gender and Class](images/survival_gender_class.png)

### Correlation Heatmap

![Correlation Heatmap](images/correlation_heatmap.png)

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- GitHub

---

## 📁 Repository Structure

```text
Titanic-Data-Visualization-Dashboard/
│
├── Titanic_Data_Visualization_Dashboard.ipynb
├── titanic_cleaned_and_featured.csv
├── requirements.txt
├── README.md
├── LICENSE
├── .gitignore
│
└── images/
    ├── titanic_premium_executive_dashboard.png
    ├── overall_survival.png
    ├── age_distribution.png
    ├── survival_by_gender.png
    ├── survival_by_class.png
    ├── survival_gender_class.png
    ├── fare_by_class.png
    ├── age_vs_fare.png
    ├── survival_by_age_group.png
    ├── survival_by_family.png
    ├── survival_by_port.png
    ├── correlation_heatmap.png
    └── survival_by_title.png
```

---

## ▶️ How to Run

### Option 1: Google Colab

1. Download or clone this repository.
2. Open `Titanic_Data_Visualization_Dashboard.ipynb` in Google Colab.
3. Upload the required dataset if prompted.
4. Run all cells in order.

### Option 2: Jupyter Notebook

Clone the repository:

```bash
git clone https://github.com/Vineesha04/Titanic-Data-Visualization-Dashboard.git
cd Titanic-Data-Visualization-Dashboard
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Titanic_Data_Visualization_Dashboard.ipynb
```

---

## ⚠️ Limitations

- The dataset does not represent every individual aboard the Titanic.
- A large portion of cabin information was missing.
- Some passenger ages were estimated.
- The project identifies associations but does not prove causation.
- Important operational factors such as evacuation timing and lifeboat access are unavailable.
- The analysis is descriptive rather than predictive.

---

## 🚀 Future Improvements

- Build an interactive dashboard using Plotly or Streamlit
- Add statistical hypothesis testing
- Train machine-learning survival prediction models
- Compare Logistic Regression, Random Forest, and XGBoost
- Add SHAP-based model explanations
- Deploy the dashboard as a web application

---

## 📄 License

This project is licensed under the MIT License.
