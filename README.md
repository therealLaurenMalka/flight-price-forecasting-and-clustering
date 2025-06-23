
## 📌 Author

**Lauren Malka**  
Data Science & Computer Science student | Passionate about machine learning, forecasting, and scraping dynamic web data.

> ✨ _Feel free to fork, collaborate, or contact me for suggestions or ideas!_  


# ✈️ Flight Price Forecasting & Clustering

This data science project focuses on analyzing, modeling, and clustering flight prices retrieved from **two competing websites**: **Kiwi** and **Kayak**.  
The goal was to **predict price differences** and **identify behavioral patterns** using machine learning techniques.

---

## 📂 Project Structure

- `Stage A – Data Collection:`  
  Scraped flight search results from Kiwi and Kayak using Playwright.  
  Data included departure airports, layovers, duration, dates, and prices.

- `Stage B – Data Cleaning & Feature Engineering:`  
  Cleaned and standardized the datasets, engineered new features such as:
  - `total_flight_length`
  - `ttt` (time to takeoff)
  - Layover flags
  - One-hot encoding for categorical columns

- `Stage C – Regression Modeling:`  
  Built various regression models to **predict flight prices per platform**:
  - Linear Regression
  - Decision Tree
  - Random Forest
  - CatBoost
  - LightGBM
  - XGBoost
  - Gaussian Process
  - K-Neighbors Regressor
  - MLPRegressor  
  Evaluated using **R², MAE, and RMSE**.

- `Stage D – Price Gap Analysis:`  
  Predicted **price differences** between Kiwi and Kayak using the same features.  
  Visualized performance across models and identified where price gaps tend to occur.

- `Stage E – Clustering:`  
  Performed unsupervised clustering (PCA + KMeans, DBSCAN) to find pricing behavior clusters and detect outliers.  
  Compared visualizations **with** and **without** noise.

---

## 📊 Tools & Technologies

- **Python**, **Jupyter Notebook**
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn**, **XGBoost**, **LightGBM**, **CatBoost**
- **Playwright** for scraping
- **PCA**, **KMeans**, **DBSCAN**

---

## 💡 Key Findings

- Kiwi and Kayak sometimes offer significantly different prices for similar flights.
- Machine learning models like **CatBoost** and **LightGBM** performed best in price prediction.
- DBSCAN revealed natural clusters in the flight data and helped identify outliers.
- PCA enabled clean visualization of patterns across booking platforms.

---

## 🔮 Future Work

- Integrate real-time APIs for live price tracking
- Add time-series modeling for forecasting future price trends
- Deploy a dashboard (Streamlit / Tableau) to visualize price gaps dynamically

---

