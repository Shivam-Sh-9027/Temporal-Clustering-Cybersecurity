# 🧠 Temporal Clustering of Cybersecurity Incidents  
### Using K-Means, Timestamp Feature Engineering, and Data Visualization

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Numpy%20%7C%20Pandas%20%7C%20Sklearn%20%7C%20Matplotlib-orange)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 **Project Overview**
Cybersecurity incidents often follow time-based patterns — certain hours, days, or months show higher attack activity.  
This project performs **temporal clustering** on a cybersecurity dataset using **K-Means** to identify:

- 🔍 Peak hours of incidents  
- 📆 High-risk days of the week  
- 🗓️ Monthly patterns  
- 🧩 Hidden behavioral trends in attack timing  

The clustering helps SOC analysts understand *when* attacks occur the most and optimize monitoring schedules.

---

## 📁 **Project Structure**
Temporal-Clustering-Cybersecurity/
│
├── clustering_analysis.py # Main script
├── incidents.csv # Dataset (uploaded by user)
├── requirements.txt # Required dependencies
├── README.md # Project documentation
└── example_plot.png # (Optional) Visualization output

---

## ⚙️ **Technologies Used**

| Category | Tools |
|---------|-------|
| Programming | Python |
| Data Handling | Pandas, NumPy |
| Machine Learning | Scikit-Learn (KMeans, StandardScaler) |
| Visualization | Matplotlib |
| Feature Engineering | DateTime processing |

---

## 🌟 **Key Features**

✔ Extracts timestamp-based features:  
- Hour  
- Day of Week  
- Month  

✔ Scales features using **StandardScaler**  
✔ Performs **K-Means clustering (k = 3)**  
✔ Adds cluster labels to the dataset  
✔ Visualizes clusters using Matplotlib  
✔ Helps identify **temporal attack patterns**  

---

## 📊 **Example Visualization**

> *Scatter plot representing clusters formed using (Hour vs Day of Week)*

If you include your plot, name it `Output.png` and add it here 👇:


---

## 🚀 **How to Run This Project**

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/Shivam-Sh-9027/Temporal-Clustering-Cybersecurity.git
cd Temporal-Clustering-Cybersecurity
```
### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```
### **3️⃣ Run the Script**
```bash
python clustering_analysis.py
```
---

🧪 Machine Learning Process (Explained)
1. Feature Engineering

Timestamp →

hour = Timestamp.dt.hour

day_of_week = Timestamp.dt.dayofweek

month = Timestamp.dt.month

These features capture temporal patterns.

---

2. Scaling

Used StandardScaler to normalize varying ranges.

---

3. K-Means Clustering
kmeans = KMeans(n_clusters=3, random_state=0, n_init=10)


Reasons for k=3:

Simple grouping

Easy visualization

Works well for time-series clustering

---

4. Visualization

Scatter plot (Hour vs Day) to visualize clusters.

---

📈 Expected Insights

You can answer:

Do attacks peak at night or morning?

Are weekends more vulnerable?

Do incidents spike in certain months?

Which clusters represent dangerous time windows?

This helps SOC analysts, blue teams, and cybersecurity students.

---

📬 Author

Shivam Sharma (Shiv)
Cybersecurity & Data Science Enthusiast

📧 Email: Sharmashiv7055@gmail.com

🔗 LinkedIn: www.linkedin.com/in/shivam-sharma-523080363

💻 GitHub: www.github.com/Shivam-Sh-9027
