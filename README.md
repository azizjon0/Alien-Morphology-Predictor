# 🧬 Alien Morphology Predictor

> Predict how alien lifeforms might evolve based on planetary atmosphere and environmental conditions 🌍👽

---

## 📌 About the Project

This is a **Machine Learning MVP** that predicts the **morphology of alien creatures**, including:

- number of **legs**, **arms**, **eyes**
- **symmetry**
- **diet**
- **skin type**
- **eye position**

Based on simulated planetary conditions:

- 🌬 `oxygen_pct` and `nitrogen_pct`  
- 🔆 `uv_level` (low / medium / high)  
- 💧 `humidity` and `water_presence`  
- 📏 `size_m` — estimated body size in meters  

🧠 **Model:** `RandomForestClassifier` with `MultiOutputClassifier`  
📊 **Dataset:** 250 augmented samples inspired by modern and Jurassic species under different planetary conditions.

---

## 🚀 Example Input & Output

```python
planet = {
    'oxygen_pct': 27,
    'nitrogen_pct': 70,
    'uv_level': 'low',
    'humidity': 'high',
    'water_presence': 'high',
    'size_m': 0.9
}
