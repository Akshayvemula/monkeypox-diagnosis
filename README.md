# 🐒 Monkeypox Diagnosis using Deep Learning

## 📌 Overview
This project presents an **AI-based Monkeypox Detection System** that classifies skin lesion images as **Monkeypox** or **Normal** using **deep learning models**.  
It combines **transfer learning (Modified VGG16)** and a **Custom CNN** to achieve high accuracy in identifying monkeypox lesions, addressing the challenges of early detection and misdiagnosis due to its similarity with other skin diseases.

The system also integrates a **Gradio/Tkinter GUI** for real-time predictions, making it accessible to healthcare workers and researchers.

---

## ✨ Features
- 🔬 **Deep Learning Models**  
  - Modified **VGG16** with transfer learning.  
  - Custom-designed **CNN** optimized for skin lesions.  
  - Ensemble approach for improved accuracy.  

- 📊 **Evaluation Metrics**  
  - Accuracy, Precision, Recall, F1-score, AUC.  
  - Confusion matrices and performance comparison charts.  

- 🖥️ **User Interface**  
  - **Tkinter GUI** for dataset handling, training, and prediction.  
  - **Gradio Web Interface** for easy testing.  

- 📂 **Data Handling**  
  - Automated dataset preprocessing (resize, normalize, augment).  
  - Supports training/validation splits.  

- ⚡ **Deployment Ready**  
  - Export models for reuse (`.h5`, `.json`).  
  - Can be optimized for mobile/edge devices.  

---

## 🏗️ System Architecture
1. **Data Acquisition** – Collects and organizes Monkeypox/Normal images.  
2. **Preprocessing** – Resizes, normalizes, augments dataset.  
3. **Model Training** – Trains both Modified VGG16 and Custom CNN.  
4. **Evaluation** – Compares models using metrics & confusion matrices.  
5. **Prediction** – Classifies uploaded test images.  
6. **Interface** – Tkinter/Gradio GUI for interaction.  

---

## 📊 Results
- **VGG16 Accuracy**: ~98.2%  
- **Custom CNN Accuracy**: ~99.1%  
- **Ensemble Accuracy**: **87.13%** (on public dataset with balanced performance across metrics).  
- Achieved balanced Precision, Recall, and F1-score (>85%).  

---

## ⚙️ Requirements
- Python 3.8+  
- Libraries:  
  ```bash
  pip install numpy pandas matplotlib seaborn tensorflow opendatasets scikit-learn gradio
  🚀 Usage

Clone the repository:

git clone https://github.com/yourusername/monkeypox-diagnosis.git
cd monkeypox-diagnosis


Run the notebook:

Open Copy_of_monkeypoxfixed.ipynb in Jupyter/Colab.

Or run as script:

python monkeypox_detector.py


For Gradio Web App:

python app.py


Then open the provided link in your browser.

📂 Repository Structure
monkeypox-diagnosis/
│── Copy_of_monkeypoxfixed.ipynb   # Fixed training/testing notebook
│── final_documentation.pdf        # Full project report
│── app.py                         # Gradio web interface (optional)
│── models/                        # Saved models (.h5/.json)
│── dataset/                       # Monkeypox dataset (not included in repo)
│── README.md                      # Project documentation




