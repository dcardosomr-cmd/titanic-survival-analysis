# Titanic Survival Analysis

## Project Overview
This project analyzes the survival patterns of passengers aboard the RMS Titanic, which sank on April 15, 1912, after colliding with an iceberg. Using a dataset of 891 passenger records, this analysis explores various factors that influenced survival rates, including:

- Gender and age demographics
- Passenger class (socioeconomic status)
- Family structure and travel companions
- Port of embarkation
- Fare paid for the journey

## Objectives
The primary goals of this analysis were to:

1. Identify key factors that influenced passenger survival
2. Examine the impact of the "women and children first" evacuation protocol
3. Analyze the relationship between social class and survival rates
4. Investigate how family structure affected survival outcomes
5. Uncover hidden patterns beyond the commonly cited evacuation rules

## Key Findings
### Gender Distribution
- The ship carried **577 male passengers (64.8%)** and **314 female passengers (35.2%)**
- Women had a significantly higher survival rate than men
- The greatest discrepancy in survival was observed in the 20-30 age group

### Age Analysis
- The **30-40 age group** had the highest survival rate
- However, this group also had the second-highest number of fatalities
- The **20-30 age group** had one of the lowest survival percentages

### Class and Social Status
- **Lower passenger classes had lower survival probabilities**
- First-class passengers had better access to lifeboats
- Third-class passengers showed the greatest gender disparity in survival rates
- When analyzed by class, a **Simpson's Paradox** was observed: the overall trend contradicted detailed class-specific analyses

### Family Structure Impact
- **60.3% of passengers traveled alone**
- Solo travelers: 29% (from females), 71% (from males)
- Family travelers: 72% (from females), 28% (from males)
- Male solo travelers in the 20-30 age group showed patterns suggesting they assisted others
- Women with children likely prioritized their families during evacuation

## 💡 Hidden Insights

The analysis revealed that survival did not depend solely on the "women and children first" evacuation protocol. The combination of factors suggests:

1. **Young solo men likely helped others**: The 20-30 male solo traveler group had high casualties, suggesting altruistic behavior
2. **Mothers prioritized their children**: Women with families showed different survival patterns than solo female travelers
3. **Social class provided advantages**: Higher classes had better access to lifeboats and information
4. **Family dynamics mattered**: Traveling with family influenced survival chances differently for men and women

## 📁 Repository Structure

```
titanic-survival-analysis/
│
├── data/
│   └── Titanic_BD.csv          # Original dataset
│
├── notebooks/
│   └── Python-Final-Project.ipynb  # Jupyter notebook with analysis
│
├── presentation/
│   └── PP-Titanic-Python.pptx    # Project presentation
│
└── README.md                   # This file
```

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## 📈 Methodology

### 1. Data Cleaning
- Handled missing values in Age column (177 missing values filled with median by gender)
- Removed Cabin column (687 missing values - too many to impute)
- Filled missing Embarked values (2 missing) with the most common port

### 2. Exploratory Data Analysis
- Analyzed passenger distribution by gender
- Examined survival rates across different age groups
- Investigated correlations between variables
- Created visualizations for key patterns

### 3. Statistical Analysis
- Calculated survival rates by demographic groups
- Examined class-based survival patterns
- Analyzed family structure impact on survival
- Identified Simpson's Paradox in class-based analysis

## 🎓 Conclusions

The Titanic disaster demonstrates that survival was influenced by a complex interplay of factors:

1. **Gender**: Women had significantly higher survival rates, but this was not uniform across all classes
2. **Age**: Younger passengers in certain demographics showed patterns of self-sacrifice
3. **Social Class**: Economic status strongly correlated with survival, likely due to cabin location and lifeboat access
4. **Family Status**: Traveling alone versus with family affected survival chances differently for men and women
5. **Human Behavior**: Evidence suggests altruistic behavior from young male solo travelers

The analysis reveals that while the "women and children first" protocol was followed to some extent, **social class, family dynamics, and individual choices significantly influenced who survived**. The tragedy highlights issues of social inequality and the complexity of human behavior in crisis situations.

## Dataset Information
- **Source**: Titanic passenger manifest
- **Records**: 891 passengers
- **Period**: 2015-2017 (for a similar City/Resort Hotel booking analysis referenced)
- **Features**: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

## Contributing
This project was developed as an academic exercise in data analysis using Python. Feedback and suggestions are welcome!

## License
This project is available for educational purposes.

## Author
**dcardosomr-cmd**
- GitHub: [@dcardosomr-cmd](https://github.com/dcardosomr-cmd)

---

*Analysis conducted as part of a Python data analysis course - December 2024/January 2025*
