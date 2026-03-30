# 🔬 Liver Disease Detector (BYOP Capstone)

An interactive Machine Learning web application designed to predict liver disease risk and provide transparent explanations for its decisions using SHAP.

## 🚀 Project Overview
This project addresses the challenge of early liver disease diagnosis. It utilizes a **Random Forest Classifier** trained on the Indian Liver Patient Dataset. To ensure clinical utility, the app provides a "Decision Analysis" chart for every prediction, showing which lab markers most influenced the result.

## 📂 Repository Structure
*Click on any file or folder to view its contents:*

- [**`app.py`**](./app.py): The main Streamlit web application.
- [**`train.py`**](./train.py): Script to preprocess data and train the saved models.
- [**`data/`**](./data/): Contains the [**`indian_liver_patient.csv`**](./data/indian_liver_patient.csv) dataset.
- [**`models/`**](./models/): Stores serialized assets ([`liver_model.pkl`](./models/liver_model.pkl), [`scaler.pkl`](./models/scaler.pkl), [`encoder.pkl`](./models/encoder.pkl)).
- [**`Project Report - Liver Disease Detector`**](https://github.com/Srihitha2307/Liver-Disease-Detector/blob/main/Project%20Report%20-%20Liver%20Disease%20Detector.docx): The detailed technical documentation for VITyarthi submission.
- [**`requirements.txt`**](./requirements.txt): List of necessary Python libraries.

## 🛠️ Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)<your-github-username>/<your-repo-name>.git
   cd Liver_Disease_Detector

## 🖥️ How to Use the App

Follow these steps to perform a diagnostic analysis:

### 1. Prepare the Environment
Ensure you have installed the requirements and started the server:
```bash
streamlit run app.py
```

### 2.Follow these steps to perform a diagnostic analysis:

1. **Input Metrics:** Use the **Sidebar** to enter laboratory values (Bilirubin, Albumin, Enzymes, etc.) from a patient's report.
2. **Analyze:** Click the **"Run Diagnostic Analysis"** button.
3. **Interpret Results:** - **Status Box:** A **Green** box indicates "Low Risk," while a **Red** box indicates "High Risk," accompanied by an AI confidence percentage.
    - **SHAP Chart:** Review the bar chart at the bottom. Bars extending to the **right (red)** identify factors that increased disease risk, while bars to the **left (blue)** identify factors that pushed the model toward a healthy result.

## 🧪 Technologies Used

- **Python:** Core programming (Pandas for data processing, Scikit-Learn for Machine Learning).
- **Streamlit:** Framework used for building the web-based User Interface.
- **SHAP:** Explainable AI (XAI) used to visualize and interpret model decision-making.
- **Joblib:** Used for model serialization and saving/loading the trained assets.
