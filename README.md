# 🌾 Crop-AI: Smart Crop Recommendation using IBM Watson AutoAI

This project uses **IBM Watson AutoAI** to build and evaluate a machine learning model that recommends the most suitable crop for cultivation based on soil and environmental parameters.

The model is trained using a dataset of soil nutrient levels and weather conditions and leverages AutoAI’s automation to handle feature engineering, model selection, and hyperparameter tuning.

---

## 📊 Features Used for Prediction

- **N**: Nitrogen content in the soil
- **P**: Phosphorus content in the soil
- **K**: Potassium content in the soil
- **Temperature**: Average temperature (°C)
- **Humidity**: Relative humidity (%)
- **pH**: Soil pH value
- **Rainfall**: Annual rainfall (mm)

---

## 🧠 Model Overview

- **Tool Used**: IBM Watson AutoAI (cloud.ibm.com)
- **Algorithm**: Random Forest Classifier (auto-selected by AutoAI)
- **Deployment**: Exported as a Jupyter Notebook (`Crop-AI.ipynb`)
- **Performance**: High accuracy with minimal human intervention

---

## 📁 Project Structure

```
Crop-AI-Project/
├── notebooks/
│   └── Crop-AI.ipynb               # AutoAI-generated pipeline notebook
├── data/
│   └── Crop_recommendation.csv     # Dataset used for training
├── README.md                       # Project documentation file
└── .gitignore                      # Ignore rules for Python/Git
```

---

## 🚀 How to Use

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Crop-AI-Project.git
cd Crop-AI-Project
```

### 2. Set Up Your Environment
Install required packages (if running locally):
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### 3. Run the Notebook
Open the notebook in Jupyter or Watson Studio:
```bash
jupyter notebook notebooks/Crop-AI.ipynb
```

---

## 📦 Dataset

- **Filename**: `Crop_recommendation.csv`
- **Records**: ~2,200 samples
- **Description**: Labeled data with environmental parameters and crop labels

---

## 🧪 Sample Prediction

**Input Sample:**
```json
{
  "N": 90,
  "P": 42,
  "K": 43,
  "temperature": 20.87,
  "humidity": 82.0,
  "ph": 6.5,
  "rainfall": 202.93
}
```

✅ **Predicted Crop**: `rice`  
✅ **Confidence**: ~87%

---

## ☁ IBM Cloud Deployment

This model was developed using IBM Watson Studio (AutoAI experiment). You can:
- Import the notebook into a new Watson Studio project
- Modify/retrain using a different dataset
- Deploy using IBM Watson Machine Learning

🔗 [cloud.ibm.com](https://cloud.ibm.com)

---

## 👩‍💻 Author

**Khyati Choudhary**  
B.Tech CSE | Guru Gobind Singh Indraprastha University  
[LinkedIn](https://www.linkedin.com/in/khyatichoudhary) • [GitHub](https://github.com/khyatichoudhary)

---

## 📜 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT)

---

## 🙌 Acknowledgments

- IBM Watson Studio & AutoAI
- Open-source dataset contributors
