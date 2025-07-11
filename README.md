# **GreenRoute – Carbon Footprint Optimization in Supply Chain Logistics**:

**Carbon footprint optimization in supply chain logistics** 🚛🌍  
A group project built with Streamlit and machine learning to estimate and reduce CO₂ emissions on transport routes.


## 📌 Project Overview

GreenRoute is a Python‑based application designed to estimate and optimize carbon emissions for supply chain routes. Users can input origin, destination, vehicle type, fuel type, traffic conditions, and road type to receive:

- Estimated CO₂ emissions using a trained Random Forest model  
- Interactive gauge and maps to visualize emissions  
- Tailored eco-friendly suggestions and strategies to minimize carbon footprint  
- A downloadable PDF report summarizing trip details, estimates & recommendations  

---

## Team Members

- **Tania Khatun**  
- **Shiwani Kumari**  
- **Hriti Jana**  
- **Parna Ganguly**  
- **Sakila Tarannoom**  

---

## 🚀 Features

- **Machine learning–powered estimation** of CO₂ emissions per kilometer  
- **Interactive dashboard** with Streamlit + Folium + Plotly  
- **Dynamic suggestions** based on user inputs (fuel type, road, traffic, vehicle)  
- **PDF export**, including personalized recommendations  
- **Simulation tools** to explore how speed or fuel choices impact emissions  

---

## 🗺️ Why It Matters

- Transportation contributes a significant portion of global greenhouse gas emissions  
- Route and energy optimization can reduce emissions **by 20–30 %** through better planning and load consolidation :contentReference[oaicite:1]{index=1}  
- Green logistics (eco‑efficient routing, reverse logistics, electric fleets) supports **both environmental and economic goals** :contentReference[oaicite:2]{index=2}  

---

## 🧪 How It Works

1. **Input** trip details via intuitive UI  
2. **Geolocation** resolves city names to coordinates using Geopy  
3. **Distance** computed using geodesic distance (km)  
4. **Model prediction** applies RandomForestRegressor trained on vehicle, weather, and route features  
5. **Emissions estimate** = CO₂-per-km × distance  
6. **Visualizations**: gauge chart + map + country emissions trends  
7. **Recommendations engine** provides context‑specific tips  
8. **PDF export** compiles all details into shareable format  

---

## 📂 Repository Structure

```

├── app.py                    ← Streamlit web app
├── model.pkl                 ← Trained machine learning model
├── label\_encoders.pkl        ← Encoders for categorical features
├── feature\_order.pkl         ← Feature order used during model training
├── vehicle\_emission\_datasets2.csv
├── country\_emissions.csv
├── co2\_faqs\_extended.csv     ← FAQ knowledge base for chatbot
├── icon.png                  ← Logo displayed in the dashboard
├── Final\_Background.jpeg     ← Background image (blurred)
└── README.md                 ← This documentation file

````

---

## 💻 Installation & Setup

# Clone the repo
git clone https://github.com/TaniaKhatun18/GreenRoute-Carbon-Footprint-Optimization-in-Supply-Chain-Logistics.git
cd GreenRoute-Carbon-Footprint-Optimization-in-Supply-Chain-Logistics

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows

# Install dependencies
pip install streamlit pandas numpy geopy folium streamlit-folium plotly matplotlib seaborn fpdf joblib
````

---

## 🧠 Usage

# Run the dashboard
streamlit run app.py

![Co2_Emisson_Dashboard](https://github.com/user-attachments/assets/3518f51f-5b45-417f-8fc6-ef9c77aa9b4a)


Configure fields like Origin, Destination, Vehicle Type, Fuel Type, etc. Your results will appear live, including emissions estimate, map, suggestions, and PDF download.

---

## 🧾 Emissions Estimation Logic

Emissions are calculated as:

```
CO₂ Emission = (CO₂ per km) × Distance (km)
```

where **CO₂ per km** is the output of a Random Forest model trained on historical vehicle emissions data (including factors like vehicle specs, fuel type, traffic, weather, etc.).

---

## ✅ Best Practices & Impact

* **Route optimization** can cut fuel use and CO₂ by \~20 % ([GitHub][1])
* **Green logistics** strategies (load-maximization, reverse logistics, fuel switching) provide cost savings and improved sustainability ([Wikipedia][2])

---

## 🔭 Future Enhancements

* Incorporate **real-time traffic APIs** to refine emissions estimates
* Add **multi-stop routing** to optimize for delivery logistics
* Extend to **multi-modal emissions** (rail, sea, road) for full supply chain impact
* Support **electric vehicle emissions factoring grid mixes**, battery range, etc.

---

## 📞 Get In Touch

For questions or collaboration:

* Contact team members on GitHub
* Raise issues or pull requests in this repository

---

Thank you for exploring GreenRoute. We hope it empowers logistics planners to make greener choices, one trip at a time 🌱

```

