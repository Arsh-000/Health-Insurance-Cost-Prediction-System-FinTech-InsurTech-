# Health-Insurance-Cost-Prediction-System-FinTech-InsurTech

**📌 Overview**
This project builds an end-to-end Health Insurance Cost Prediction system designed for insurance companies to estimate premiums based on user demographics, lifestyle, and medical history.
The system uses segmented machine learning models and is deployed via a Streamlit web application for real-time predictions.

**🎯 Problem Statement**
Health insurance pricing is complex due to multiple risk factors such as:

- Age
- Medical history
- Lifestyle habits (smoking, BMI)
- Income and dependants

Traditional pricing methods rely on static rules, leading to:

- Inaccurate premium estimation
- Poor risk segmentation
- Manual underwriting effort
  
**🧠 Solution Approach**

This system replicates a real-world insurance workflow:

- Data preprocessing and feature engineering
- Risk scoring based on medical history

- Segmentation of users:
Young (≤ 25 years)
Rest (> 25 years)

- Training separate ML models for each segment
- Real-time premium prediction via Streamlit
  
**⚙️ Tech Stack**

- Python
- Pandas, NumPy
- Scikit-learn
- Streamlit
- Joblib

**📊 Features Used**

- Demographic Features
- Age
- Gender
- Marital Status
- Financial Features
- Income
- Number of Dependants
- Lifestyle Features
- Smoking Status
- BMI Category
- Medical Features
- Medical History
- Genetical Risk
- Other Features
- Employment Status
- Region
- Insurance Plan
  
**🤖 Model Architecture**

🔹 Segmented Modeling Approach
Model 1 → Young Users (≤ 25)
Model 2 → Rest of Population (> 25)

🔹 Feature Engineering
Custom medical risk scoring function
One-hot encoding for categorical variables
Separate scaling pipelines for each segment

👉 This approach improves accuracy and reflects real-world insurance practices.

**📈 Output**
Predicted Health Insurance Premium Cost

**🖥️ Web Application**
The project includes an interactive Streamlit interface where users can:

- Input personal, financial, and medical details
- Get instant premium prediction
- Simulate real-world underwriting scenarios

**🚀 How to Run Locally**
git clone https://github.com/<your-username>/health-insurance-cost-predictor.git
cd health-insurance-cost-predictor
pip install -r requirements.txt
streamlit run app.py

## 📁 Project Structure

```
health-insurance-cost-predictor/
│
├── app.py
├── prediction_helper.py
├── requirements.txt
├── README.md
│
├── artifacts/
│   ├── model_young.joblib
│   ├── model_rest.joblib
│   ├── scaler_young.joblib
│   └── scaler_rest.joblib
│
├── notebooks/
│   ├── model_training.ipynb
│   └── segmentation_analysis.ipynb
```

**💡 Business Impact**

- Enables accurate and dynamic premium pricing
- Reduces manual underwriting effort
- Improves risk-based segmentation
- Supports scalable insurance operations

**🔥 Key Highlights**

- Segmented ML modeling (industry-relevant approach)
- Custom medical risk scoring logic
- End-to-end pipeline (data → model → deployment)
- Interactive UI for real-world usage

**🔮 Future Improvements**

- Add SHAP explainability for transparency
- Improve segmentation using clustering
- Deploy as an API (FastAPI)
- Add monitoring and model drift detection
cd health-insurance-cost-predictor
pip install -r requirements.txt
streamlit run app.py
