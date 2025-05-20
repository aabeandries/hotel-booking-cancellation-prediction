# Improving Hotel Revenue by Predicting Booking Cancellations 🏨

## 1. Project Overview

This project analyzes hotel booking data to improve revenue management by predicting booking cancellations. The primary focus is to **minimize financial losses caused by cancellations** and **support operational decisions using machine learning**.

### Key Objectives:

- **Objective 1:** Identify the key drivers of booking cancellations using data exploration and feature importance.
- **Objective 2:** Build and optimize a classification model (Random Forest) to predict cancellations.
- **Objective 3:** Estimate financial impact of false positives and false negatives for strategic decision-making.
- **Objective 4:** Provide actionable business strategies such as dynamic overbooking and guest segmentation.

---

## 2. Data Sources

- **Hotel Booking Demand Dataset:**  
  Contains booking details such as lead time, market segment, deposit type, number of special requests, etc.  
  Source: [Kaggle - Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

---

## 3. Technologies Used

- **Programming Language:** Python (Pandas, NumPy, Scikit-learn)
- **Visualization:** Matplotlib, Seaborn, Plotly
- **Modeling:** Random Forest Classifier, F2-score, Precision-Recall tradeoff
- **Environment:** Jupyter Notebook
- **Version Control:** Git

---

## 4. Project Structure

├── README.md

├── data

│ ├── external

│ ├── interim

│ ├── processed

│ └── raw

│

├── models

├── notebooks

│ └── 1.0-aa-hotel-booking-predict.ipynb

│

├── references

├── reports

│ └── figures

├── requirements.txt

└── src


---

## 5. Summary of Findings

### 5.1 Business Insight

- **Cancellation Patterns:**  
  The model identified `deposit_type`, `market_segment`, and `total_special_requests` as the strongest predictors.
  
- **High-Risk Groups:**  
  - Bookings from "Groups" and "Online TA" segments showed significantly higher cancellation rates (61.3% and 36.6% respectively).
  - Non-Refundable bookings were almost 100x more likely to be canceled.

- **Behavioral Clues:**  
  - More special requests are associated with lower cancellation likelihood.
  - Guests needing parking or booking for longer stays are less likely to cancel.

- **Financial Modeling:**  
  Predictive modeling reduces total financial loss by $457,300 through reselling and preemptive actions.

### 5.2 Actionable Recommendations

#### 🛠️ Operational Strategy
- Implement dynamic overbooking for high-risk segments (e.g., 8–12% overbooking for Group bookings).
- Offer incentives for refundable bookings in cancellation-prone segments.

#### 📈 Marketing Optimization
- Send F&B vouchers or check-in reminders for high-risk reservations.
- Offer upgrades to guests with multiple special requests.

#### 📊 System Integration
- Embed the model into the hotel’s Property Management System (PMS) to flag cancellations with >65% probability.
- Use insights for early warnings and resell strategies.

---

## 6. Model Limitations

Despite high F2 performance, several limitations were identified:
- Missing features like `booking date`, `room type`, and `cancellation reason` limit model precision.
- Guest-level data (number of people, guest type) and room pricing were unavailable.
- High occurrence of duplicates and outliers requires deeper cleaning and validation for production deployment.

---

## 7. Contact

- **Name:** Abednego Andries  
- **Email:** abeandries@icloud.com  
- **LinkedIn:** [linkedin.com/in/abednego-andries-7015001a4](https://www.linkedin.com/in/abednego-andries-7015001a4/)
- **GDrive Link:** [Hotel_Booking_Cancellation_Prediction](https://drive.google.com/drive/folders/1J-X-teqBq3wNliuNQJVLV1kaGLblWedL?usp=share_link)

---
