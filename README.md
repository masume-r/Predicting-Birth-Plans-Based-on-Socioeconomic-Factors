
# 📊 Predicting Birth Plans Based on Socioeconomic Factors

## 📝 Overview
This project analyzes factors influencing individuals' plans to have children using a dataset from the **Korean Longitudinal Survey of Women and Families (KLoWF)** . The study utilizes **Random Forest Classification** and **Logistic Regression** to determine key predictors of birth planning.

### 🔍 Two Perspectives of Analysis
This project examines birth planning from two different perspectives:
1. **Families with at least one child** 📌
   - Analyzing whether individuals who have already experienced parenthood plan to have more children.
   - Investigating the key reasons influencing their decision.
2. **General Population Analysis** 📌
   - Evaluating birth planning decisions without considering previous childbirth experience.
   - Identifying socioeconomic and personal factors impacting birth plans.

---

## 📂 Dataset
### 📌 Source
The dataset is sourced from:
- 📊 **[Korean Longitudinal Survey of Women and Families (KLoWF)](https://gsis.kwdi.re.kr/gsis/en/main.html)**

### 🔍 Features
The dataset includes the following variables:
- 🏡 **Age**
- 👨‍👩‍👦 **Husband's Age**
- 🎓 **Highest Level of Education**
- 🏥 **Health Condition**
- 💰 **Concerns about the Future** (e.g., Financial Difficulties, Health, Relationship with Husband)
- 👔 **Employment Status of Husband**
- ⏳ **Weekly Average Working Hours**
- 💵 **Monthly Average Income**
- 👶 **Have Plan to Have a Baby** (Target Variable: 0 = No, 1 = Yes)

### 📥 How to Obtain the Dataset
Since the dataset is not included in this repository due to licensing restrictions, you can obtain it from the official sources:
1. Visit [KLoWF](https://gsis.kwdi.re.kr/gsis/en/main.html)
2. Navigate to **Data Download**
3. Apply necessary filters for the required variables
4. Download the dataset in CSV format and place it in the `data/` directory

---

## 🛠 Data Preprocessing
Before training the models, the dataset undergoes preprocessing:
- ❌ Removing missing values and invalid records (e.g., filtering out rows with -9 or -8 values)
- 🔄 Encoding categorical variables
- 📏 Feature scaling where applicable
- 📊 Splitting data into training and testing sets
- ⚖️ Addressing class imbalance using **SMOTE oversampling**

---

## 🤖 Model Training
The project implements:
- 🌲 **Random Forest Classifier** to predict birth plans based on socioeconomic factors
- 📈 **Logistic Regression** to analyze the relationship between age and birth plans

---

## 📊 Evaluation Metrics
- ✅ **Accuracy**
- 🔍 **Precision & Recall**
- 📌 **Feature Importance Analysis**

---

## 📈 Results & Insights
✔ **Age is a significant predictor of birth planning** 📊
✔ **Individuals with no plans to have children tend to have higher average incomes** 💵
✔ **Economic and health concerns are major factors influencing decisions** 🏥💰


---

## 🚀 How to Run the Project
1️⃣ Clone this repository:
   ```sh
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   ```
2️⃣ Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3️⃣ Ensure the dataset is in the `data/` directory
4️⃣ Run the preprocessing and model training script:
   ```sh
   python train_model.py
   ```

---

## ⚠️ Limitations
- ⚖ **The dataset is unbalanced, which may affect prediction performance**
- ❓ **Some variables have missing or imputed values that could introduce bias**
- 🔧 **Further hyperparameter tuning and feature engineering could improve accuracy**

---

## 👥 Contributors
- **Your Name** - [GitHub Profile](https://github.com/yourusername)

---

## 📜 License
This project is for academic and research purposes only.


