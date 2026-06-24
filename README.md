# 🏥 Smart Hospital Patient Navigator by Mr Halip

A machine learning-powered web application that intelligently recommends the appropriate hospital department based on patient symptoms, vital signs, and medical history.

## Overview

**Smart Hospital Patient Navigator** is an AI-driven triage system built with Streamlit that helps patients find the right medical department for their concerns. Using a trained K-Nearest Neighbors (KNN) model with 99.5% accuracy, the app analyzes patient symptoms and vitals to provide personalized department recommendations.

## Features

✨ **Intelligent Recommendations**

- ML-powered triage system using KNN algorithm (k=7)
- Trained on 102,000+ patient records
- Provides confidence scores for each department

📋 **Comprehensive Patient Assessment**

- Symptom checker with 9 common symptoms
- Severity indicators (temperature & heart rate levels)
- Chief complaint categorization
- Medical history screening
- Patient demographics

🏨 **Six Hospital Departments**

1. **Respiratory Medicine** 🫁 - Lungs and airways conditions
2. **Cardiology** ❤️ - Heart and cardiovascular conditions
3. **Gastroenterology** 🫃 - Digestive system conditions
4. **Neurology** 🧠 - Brain, spine, and nervous system
5. **General Medicine** 🩺 - General health concerns
6. **Dermatology** 🔬 - Skin, hair, and nail conditions

📍 **Actionable Guidance**

- Specific directions to the recommended department
- Estimated wait times
- Pre-visit preparation instructions
- Confidence breakdown by department

🎨 **Modern, Intuitive UI**

- Clean, modern interface with Inter font
- Color-coded departments for easy identification
- Mobile-friendly responsive design
- Accessibility-focused styling

## Requirements

- Python 3.8 or higher
- Streamlit >= 1.32.0
- scikit-learn >= 1.4.0
- pandas >= 2.0.0
- numpy >= 1.26.0

## Installation

1. **Clone or download** this repository
2. **Install dependencies:**

   ```bash
   pip install -r hospital_requirements.txt
   ```

3. **Ensure the model file exists:**
   The app requires a pre-trained model file: `hospital_model_by_halip26.pkl`

## Usage

### Run the Application

```bash
streamlit run hospital_app.py
```

The app will open in your default browser at `http://localhost:8501`

### Using the Triage Form

1. **Select Symptoms** - Check all symptoms that apply
2. **Choose Duration** - Indicate how long symptoms have persisted
3. **Rate Severity** - Select temperature and heart rate levels
4. **Medical History** - Indicate any chronic conditions
5. **Patient Info** - Enter age and gender
6. **Submit** - Click "Get AI Recommendation →"

### Interpreting Results

The app displays:

- **Recommended Department** with description and next steps
- **Confidence Score** showing likelihood distribution across all departments
- **Pre-visit Instructions** specific to the recommended department
- **Model Details** - Model type, training data size, and accuracy

## Model Details

| Aspect        | Details                                                     |
| ------------- | ----------------------------------------------------------- |
| Algorithm     | K-Nearest Neighbors (KNN)                                   |
| k value       | 7                                                           |
| Training Data | 102,000+ patient records                                    |
| Accuracy      | 99.5%                                                       |
| Features      | 17 input features (symptoms, vitals, history, demographics) |
| Departments   | 6 specialized departments                                   |

## Symptoms Assessed

- 🌡️ Fever
- 🤧 Cough
- 🤕 Headache
- 💔 Chest Pain
- 🤢 Stomach Pain
- 😮‍💨 Shortness of Breath
- 🤮 Nausea / Vomiting
- 😵 Dizziness
- 🔴 Skin Rash

## Medical Conditions Screened

- High Blood Pressure (Hypertension)
- Heart Disease
- Asthma

## File Structure

```
smart_hospital_day2/
├── hospital_app.py                    # Main Streamlit application
├── hospital_model_by_halip26.pkl      # Pre-trained ML model (required)
├── hospital_requirements.txt          # Python dependencies
└── README.md                          # This file
```

## Important Disclaimer

⚠️ **This application provides AI-generated suggestions only and is NOT a medical diagnosis.**

- Always consult with a licensed healthcare professional for proper medical evaluation
- This tool is designed to assist with department navigation, not diagnosis
- For emergency situations, seek immediate medical attention
- The app cannot replace professional medical judgment

## Technical Stack

- **Frontend**: Streamlit
- **ML Framework**: scikit-learn
- **Data Processing**: pandas, numpy
- **Styling**: Custom CSS with Tailwind-inspired design

## Author & Credits

- **Model Training**: halip26
- **Application**: Future Classroom · Machine Learning
- **Powered by**: Streamlit

## License

Please refer to the project's license file for usage rights and restrictions.

## Contact & Support

For issues, questions, or feedback about this application, please contact the Future Classroom ML team.

---

**Version**: 1.0  
**Last Updated**: June 2026
