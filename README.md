# Social Media Traffic Prediction

## 📌 Project Title
**Advanced Machine Learning Approaches for Urban Streaming Service Traffic Prediction**  
*Predicting Instagram and YouTube Traffic Patterns in French Metropolitan Cities using Machine Learning*

## 👥 Authors
- Omar Amin Abdelrazek (O.Amin2373@nu.edu.eg)  
- Zakaria Zakaria (z.ahmed2337@nu.edu.eg)  
- Marwan Ghazal (M.Mohamed2365@nu.edu.eg)  
- Salma Mohamed (S.Mohamed2393@nu.edu.eg)  
School of Information Technology and Computer Science, Nile University

---

## 📖 Abstract
Urban telecommunications networks are under growing pressure due to high mobile traffic from platforms like Instagram and YouTube. This study presents a predictive modeling framework using XGBoost, Gradient Boosting, and Random Forest to forecast mobile application traffic across Paris and Lyon using 40,000 records collected in March 2019.

**Key findings:**
- XGBoost outperformed other models with R² > 0.998 and MAE < 5% of average traffic.
- Instagram generated 2.2× more traffic than YouTube.
- Paris traffic volume was 5.4× higher than Lyon.
- Peak usage: Lyon at 17:00, Paris at 22:00.

---

## 📊 Dataset
- **Size**: 40,000 records (10,000 per city-app combination)
- **Cities**: Paris and Lyon
- **Applications**: Instagram, YouTube
- **Timeframe**: March 21–24, 2019 (15-min intervals)
- **Source**: Real-world mobile traffic logs

---

## 🧹 Preprocessing
- Data cleaning and type validation
- Outlier removal using IQR method
- ~11% of records removed for noise reduction

---

## 🛠 Feature Engineering
28 engineered features including:
- **Temporal**: Hour, Day, Weekend flag, Cyclical encodings  
- **Behavioral**: Peak period indicators, Hour groupings  
- **Statistical**: Hourly mean, deviation, Z-scores

---

## 🤖 Models Used
1. **Random Forest**  
2. **Gradient Boosting**  
3. **XGBoost** (best performance)

Each model used:
- 80/20 chronological train-test split
- Hyperparameter tuning with Grid Search

---

## 📈 Performance (Sample)
| City-App         | Model         | R²     | MAE     | MAPE   |
|------------------|---------------|--------|---------|--------|
| Lyon - Instagram | XGBoost       | 0.998  | 2,034   | 14.2%  |
| Paris - Instagram| XGBoost       | 0.998  | 10,693  | 9.4%   |

---

## 🔍 Key Insights
- **City behavior**: Paris peaks later (leisure), Lyon peaks earlier (work)
- **App usage**: Instagram shows social rhythm patterns, while YouTube is more evenly
