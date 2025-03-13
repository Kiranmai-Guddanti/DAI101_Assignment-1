# DAI101_Assignment-1

# Titanic Dataset - Data Cleaning and Exploratory Data Analysis (EDA)

## Overview
The *Titanic dataset* contains passenger details from the Titanic shipwreck, including survival status, demographic information, ticket details, and fare prices. The dataset has been cleaned and analyzed to understand key patterns and insights.

## Data Cleaning Steps
### 1. Handling Missing Values
- The dataset had missing values in key columns such as Age, Fare, and Embarked.
- Age: Missing values were filled using the *median age* to maintain distribution balance.
- Fare: Missing values were filled with the *median fare*.
- Embarked: Filled using the *mode* (most common port).

### 2. Removing Duplicates
- Duplicate entries were checked and removed if found to ensure data consistency.

### 3. Standardizing Categorical Values
- Sex column values were converted to lowercase (male, female) for consistency.
- Embarked column values were standardized.

### 4. Handling Outliers
- *Box plots* were used to identify outliers in Fare and Age.
- Outliers were capped at an upper limit based on the *Interquartile Range (IQR) method*.

### 5. Data Type Conversions
- Age and Fare were converted to *numeric types*.
- Survived, Pclass, and other categorical variables were converted to *category types* for better analysis.

## Exploratory Data Analysis (EDA)

### 1. Univariate Analysis
- *Summary Statistics*:
  - Mean, median, mode, variance, and skewness were calculated for numerical columns (Age, Fare).
  - Frequency distributions were computed for categorical variables (Pclass, Sex, Embarked).
- *Visualizations*:
  - *Histograms & Box Plots*: Used to analyze the distribution of Age and Fare.
  - *Bar Charts*: Showed the count of passengers by class, gender, and embarkation port.

### 2. Bivariate Analysis
- *Correlation Matrix & Heatmap*:
  - Explored relationships between Fare, Age, Pclass, and Survived.
- *Scatter Plots*:
  - Analyzed relationships between Fare and Age, Pclass and Survived.
- *Grouped Comparisons*:
  - Survival rates were analyzed by Pclass, Sex, and Embarked.

### 3. Multivariate Analysis
- *Pair Plots:*
  - Visualized multiple numerical features together to observe interactions between Age, Fare, and Pclass.
- *Violin & Box Plots*:
  - Compared ticket fare and age distributions for different passenger classes.
- *Interaction Between Gender, Class, and Survival:*
  - A stacked bar plot was used to analyze how survival rates varied across Sex and Pclass.
- *Fare, Age, and Class Combined Analysis:*
  - A 3D scatter plot helped to understand if wealthier or younger passengers in different classes had better survival chances.
- *Survival Rate by Embarked Port, Class, and Fare:*
  - A violin plot showed fare distribution across different embarkation points, highlighting class-based differences.

## Key Findings & Observations
- *Survival Rate by Gender:*
  - Females had a significantly higher survival rate than males.
- *Effect of Passenger Class:*
  - First-class passengers had a higher survival rate compared to second and third-class passengers.
- *Age and Survival:*
  - Younger passengers, especially children, had higher survival rates.
- *Fare Distribution:*
  - Higher fares were generally associated with first-class passengers who had better survival chances.
- *Embarked Port & Survival:*
  - Passengers who embarked from port C (Cherbourg) had a higher survival rate compared to those from S (Southampton) and Q (Queenstown).
- *Interplay Between Class, Fare, and Survival:*
  - Higher-class passengers who paid more had significantly better survival chances.
  - Third-class passengers with lower fares had the lowest survival rates.
