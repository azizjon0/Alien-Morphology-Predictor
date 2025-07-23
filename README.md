# 🧬 BioMorphoRegressor (BMR)

> Predict alien morphology from planetary conditions using ML 🌍👽


Method and idea proposed by Azizjon Achilov, July 2025


This project introduces **BioMorphoRegressor (BMR)** — a speculative ML-based method for predicting the **morphological structure** of alien lifeforms based on atmospheric and environmental features.

BMR takes in a planet’s:
- 🌬 `oxygen_pct` and `nitrogen_pct`  
- 🔆 `uv_level` (low / medium / high)  
- 💧 `humidity` and `water_presence`  
- 📏 `size_m` — estimated body size in meters  

...and outputs expected biological features like number of limbs, eyes, symmetry, skin type, and more.

It’s a blend of **biological inspiration**, **planetary physics**, and **machine learning logic**.

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
```

## 👽 Predicted Alien Features

```json
{
  "num_legs": 2,
  "num_arms": 2,
  "eyes": 2,
  "symmetry": "bilateral",
  "diet": "carnivore",
  "skin_type": "scales",
  "eye_position": "side"
}
```

## 🧪 How to Run

### Install the required libraries:

```bash
pip install -r requirements.txt

```
jupyter notebook Alien_Model.ipynb


## 📊 Model Accuracy (Snapshot)

| Target         | Accuracy |
|----------------|----------|
| `eyes`         | 95.2%    |
| `num_arms`     | 87.3%    |
| `symmetry`     | 93.7%    |
| `num_legs`     | 69.8%    |
| `diet`         | 69.8%    |
| `eye_position` | 73.0%    |
| `skin_type`    | 66.7%    |

> 📌 *Detailed classification reports, precision / recall / f1-scores are available in the notebook.*

---

## 🔮 Future Directions

- Add environmental features like **gravity**, **pressure**, **temperature**
- Include **planet type** (e.g., gas giant, rocky, desert, oceanic)
- Predict **intelligence level** or **mobility type**
- Use **LLMs** or **GANs** to generate alien body designs
- Build interactive web app (e.g., **Streamlit** or **Gradio**)

---

## 🤯 Why?

If we aim to search for life beyond Earth,  
we must also imagine how it could actually **look**, **move**, and **survive** —  
under alien physics, chemistry, and evolutionary rules.

This project is a speculative step in that direction:

- 🔬 **Science-inspired**  
- 🎨 **Imagination-fueled**  
- ⚙️ **Data-driven**

---

## 🛠 Tech Stack

- Python 3
- Pandas, Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

