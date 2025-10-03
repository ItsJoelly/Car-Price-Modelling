# 🚗 Car Price Prediction – Machine Learning Project

A machine learning project that predicts the **selling price of used cars** based on features such as brand, year, mileage, fuel type, ownership history, and transmission type.  

---

## 📦 Dataset Overview

The dataset contains 150+ records with the following features:

- `Car_Name`: Model of the car  
- `Year`: Manufacturing year  
- `Selling_Price`: Target variable – resale price of the car  
- `Present_Price`: Price of the car when new  
- `Driven_Miles`: Total miles driven  
- `Fuel_Type`: Petrol, Diesel, or CNG  
- `Selling_type`: Individual or Dealer  
- `Transmission`: Manual or Automatic  
- `Owner`: Number of previous owners (0–3)  

---

## ✅ Project Workflow

1. **Data Cleaning**  
   - Removed rows with missing values  
   - Handled outliers in mileage using IQR  

2. **Feature Engineering**  
   - Created car age from `Year`  
   - Dropped `Car_Name` (replaced with one-hot encoded features)  

3. **Encoding**  
   - Applied one-hot encoding to categorical features (`Fuel_Type`, `Selling_type`, `Transmission`, etc.)  

4. **Model Training**  
   - Used **Linear Regression**  

5. **Evaluation**  
   - Calculated R² score on training and test sets  

6. **Prediction Function**  
   - Built a function to predict selling price from user-defined input (year, mileage, fuel type, etc.)  

---

## 🔍 Key Observations

- **Present Price** and **Year (car age)** are the strongest predictors of resale value  
- **Driven Miles** has an inverse effect on selling price  
- Cars with **Automatic transmission** and **Diesel fuel** generally retain higher value  

---

## 📊 Visual Insights

- `Selling_Price` increases proportionally with `Present_Price` for newer vehicles  
- Older cars depreciate faster, even if their initial price was high  

### 📷 Example Visualization  

![Selling Price vs Present Price](screenshots/output.png)  

---

## 🛠️ Tech Stack

- **Python**  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`  

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone 
cd Car-Price-Prediction

# 2. Install required packages
pip install -r requirements.txt

# 3. Launch the Jupyter Notebook
jupyter notebook
```

## 📊 Model Accuracy

- Train R² Score: 0.86
- Test R² Score: 0.74
- Model Used: Linear Regression

---

## 📜 License

This project is under the MIT License.

---
