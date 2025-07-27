# 🏎️ Driver-Profiling

## F1 Telemetry Clustering with FastF1

This project uses real Formula 1 telemetry data to analyze driver performance styles by clustering based on lap data such as speed, throttle usage, and gear shifts. It leverages the **FastF1** library for data extraction and **scikit-learn** for unsupervised learning.

---

## 🚀 Overview

The goal of this project is to extract and analyze **fastest lap telemetry** from all drivers in a given F1 session, engineer meaningful features, and **cluster drivers by driving style** using KMeans.

### 🔑 Key Highlights:
- Pulls race data from the FastF1 API
- Cleans and processes telemetry (e.g., speed, throttle, gear)
- Uses feature engineering to generate numerical metrics
- Applies clustering (KMeans) to group similar driving styles
- Visualizes clusters using Seaborn and Matplotlib

---

## 📁 Project Structure
	Driver-Behavioural-Profiling/
	├── cache/                     # FastF1 race cache
	├── data/                      # Saved telemetry or feature data
	├── plots/                     # Cluster visualizations
	├── notebooks/
	│   ├── feature_engineering.ipynb   # Feature creation from telemetry
	│   └── visualization.ipynb         # Cluster analysis & plots
	├── requirements.txt           # Required packages
	└── README.md                  # Project documentation



---

## ⚙️ Features Extracted

For each driver's fastest lap, the following features are calculated:

- `SpeedMean`: Average speed (km/h)
- `ThrottleStd`: Standard deviation of throttle input
- `BrakeTime`: Total time brakes were applied
- `GearChanges`: Number of unique gear shifts
- `RPMStd`: Variability in engine RPM

These features help understand **aggressiveness**, **consistency**, and **driving style**.

---

## 📊 Visualizations

Clustering results are visualized using scatter plots:

- **X-axis**: SpeedMean  
- **Y-axis**: ThrottleStd  
- **Colors**: Cluster labels  
- Optionally, driver names can be annotated

---

## 🧠 Tech Stack

- **Data Extraction:** FastF1
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (KMeans)
- **Visualization:** Seaborn, Matplotlib
- **Environment:** Python 3.10+, Jupyter Notebook

---

## 💡 Example Use Cases

- Scouting driver behavior across races
- Understanding car-driver combinations
- Generating feature vectors for predictive modeling
- Comparing team driving patterns

---

## 🧪 How to Run

1. **Install dependencies**  
   ```bash
   pip install -r requirements.txt

2. Create FastF1 cache directory
   ```bash
  	mkdir 

3. Run the Jupyter Notebooks
Open the notebooks in notebooks/ and execute each cell step by step.

---
## ✅ Requirements
 
	fastf1
	numpy
	pandas
	scikit-learn
	matplotlib
	seaborn

---
## Install then using:
	
	pip install -r requirements.txt

---
## 📌 To Do

 Add support for multiple sessions (Quali + Race)

 Include more telemetry metrics (e.g., steering, DRS status)

 Automate full-season batch clustering

 Build a web dashboard to explore clusters interactively
 
---
## 🤝 Acknowledgements
FastF1 for providing clean and structured F1 telemetry

Scikit-learn for clustering tools

The Formula 1 open-source community

---
## 📬 Contact

Kirthic Adhithya J

📧 [kirthicadhithyaj@gmail.com]

🔗 LinkedIn Profile - https://www.linkedin.com/in/kirthicadhithyaj/

