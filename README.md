# 🌾 Edge–Fog–Cloud Assisted Stubble Management for Smart Agriculture  

## 📌 Overview  
Stubble burning, a common post-harvest practice in Northern India, contributes significantly to **air pollution, greenhouse gas emissions, and soil degradation**.  

This project presents a **multi-tier AI-enabled framework** integrating **Edge–Fog–Cloud computing, UAVs, IoT sensors, and machine learning models** for **real-time stubble fire detection, prediction, and verification**.  

The system moves from reactive enforcement to **data-driven prevention and early intervention**.  

---

## ⚙️ System Architecture  
1. **Edge Layer (Fuzzy Logic)**  
   - Computes vegetation indices (NDVI, NDTI) from satellite data.  
   - Applies fuzzy logic for early stubble detection.  

2. **Cloud Layer (XGBoost)**  
   - Aggregates data from satellites, weather APIs, and historical fire records.  
   - Predicts fire-prone regions using **XGBoost (AUC = 0.987, Accuracy = 95.4%)**.  

3. **Fog Layer (IoT Validation)**  
   - Selectively activates IoT ground sensors (CO₂, smoke, temperature, humidity).  
   - Confirms or rejects cloud predictions with localized sensing.  

4. **UAV Layer (MobileNetV2)**  
   - UAVs visually confirm fire incidents.  
   - **MobileNetV2 model** achieves **96% accuracy** in fire/no-fire classification.  

---

## 🛠️ Tech Stack  
- **Languages**: Python  
- **Libraries/Frameworks**: XGBoost, TensorFlow/Keras, NumPy, Pandas, OpenCV, Matplotlib  
- **ML Models**: Fuzzy Logic, XGBoost, MobileNetV2 (transfer learning)  
- **Data Sources**: Sentinel-2, MODIS, VIIRS, UAV imagery, IoT sensor simulations  
- **APIs**: Meteorological Data APIs  

---

## 📊 Key Results  
- ✅ **XGBoost**: AUC = 0.987, Accuracy = 95.4%  
- ✅ **MobileNetV2**: Accuracy = 96%, Precision = 96.3%, Recall = 96%, F1 = 95.9%  
- ✅ **System efficiency**: Reduced latency and bandwidth via Edge–Fog–Cloud design  
- ✅ **Scalability**: Adaptable to forest fires, crop disease monitoring, and flood alerts  

---

## 📂 Repository Structure  
```
stubble-management-system/
│── README.md
│── report/
│   └── Internship_Report.pdf
│── src/
│   ├── fuzzy_logic/       # Edge-level NDVI, NDTI + fuzzy rules
│   ├── xgboost_model/     # Fire-prone prediction (XGBoost)
│   ├── mobilenetv2/       # UAV fire confirmation model
│   └── data/              # Sample datasets
│── results/
│   └── graphs/            # ROC, confusion matrix, performance plots
│── LICENSE
```

---

## 🚀 How It Works  
1. **Edge devices** compute NDVI/NDTI vegetation indices and apply fuzzy rules.  
2. **Cloud layer** predicts fire-prone areas with XGBoost.  
3. **Fog layer** validates predictions with IoT sensor readings.  
4. **UAVs** are dispatched for visual confirmation using MobileNetV2.  
5. **Alerts** are issued to authorities through dashboards/notifications.  

---

## 🌍 Impact  
✔️ Provides **real-time, accurate fire monitoring**  
✔️ Reduces **air pollution & health hazards** from stubble burning  
✔️ Supports **sustainable agriculture** by protecting soil fertility  
✔️ Extensible to **forest fire detection, crop disease outbreaks, or flood early warning**  

---

## 📈 Future Enhancements  
- Large-scale pilot deployment with farmers & local govt.  
- Expand MobileNetV2 to **multi-class classification** (smoke intensity, crop type).  
- Mobile app/dashboard for real-time alerts.  
- Edge AI optimizations for **low-power IoT devices**.  

---

## ✍️ Contributors  
- Ramandeep Kaur (TIET, Patiala)  
- Vansh Garg (NIT Delhi)  
- Kashish (TIET, Patiala)  

**Supervisors**: Prof. (Dr.) Geeta Sikka, Dr. Sahil, Dr. Amandeep Kaur (NIT Delhi)  

---

🔗 *Full methodology, results, and references are available in* `report/Internship_Report.pdf`  
