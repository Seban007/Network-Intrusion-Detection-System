\# 🧩 Network Intrusion Detection System (NIDS)



A Machine Learning–based \*\*Network Intrusion Detection System (NIDS)\*\* that identifies cyber attacks such as \*\*DDoS\*\*, \*\*PortScan\*\*, and other malicious network activities using the \*\*CICIDS2017 dataset\*\*.



---



\## 🚀 Project Overview



This project focuses on detecting network intrusions by analyzing real network traffic data using supervised machine learning.  

The system is designed to classify whether a network connection is \*\*BENIGN (normal)\*\* or an \*\*ATTACK\*\*, improving the reliability of cybersecurity defense systems.



---



\## 🧰 Tech Stack



\- \*\*Language:\*\* Python 🐍  

\- \*\*Libraries:\*\* `pandas`, `numpy`, `xgboost`, `sklearn`, `joblib`  

\- \*\*Dataset:\*\* \[CICIDS2017 Dataset](https://www.unb.ca/cic/datasets/ids-2017.html)  

\- \*\*Model:\*\* XGBoost Classifier  

\- \*\*Environment:\*\* Jupyter Notebook / VS Code  



---



\## ⚙️ Features



✅ Detects multiple types of network intrusions  

✅ Preprocesses and scales network traffic data  

✅ Trains and saves ML model for later predictions  

✅ Loads and uses model for real-time or test predictions  

✅ Calculates accuracy, precision, recall, and F1-score  



---



\## 🧪 Project Workflow



1\. \*\*Dataset Loading:\*\*  

&nbsp;  The CICIDS2017 dataset is used, containing labeled network traffic data.



2\. \*\*Data Preprocessing:\*\*  

&nbsp;  - Label encoding for categorical values.  

&nbsp;  - Standard scaling for numeric features.  

&nbsp;  - Splitting data into training and test sets.



3\. \*\*Model Training:\*\*  

&nbsp;  - Trains an \*\*XGBoost\*\* model on the preprocessed dataset.  

&nbsp;  - Evaluates the model using performance metrics.



4\. \*\*Model Saving:\*\*  

&nbsp;  - Saves the model, scaler, and encoder using `joblib` for reuse.  



5\. \*\*Prediction Script (`main.py`):\*\*  

&nbsp;  - Loads saved components.  

&nbsp;  - Accepts new network traffic samples.  

&nbsp;  - Outputs whether each sample is \*\*BENIGN\*\* or \*\*ATTACK\*\*.



---



\## 🧮 Performance Metrics



| Metric | Description |

|:--------|:-------------|

| \*\*Accuracy\*\* | Overall correct predictions |

| \*\*Precision\*\* | Correctly identified attacks |

| \*\*Recall\*\* | Sensitivity to detect intrusions |

| \*\*F1-Score\*\* | Harmonic mean of precision and recall |



---



\## 📂 Project Structure



NIDS/

├── main.py # Predicts intrusion or benign traffic

├── train\_model.py # Trains the ML model

├── requirements.txt # Project dependencies

├── model/

│ ├── xgboost\_model.pkl # Trained model

│ ├── scaler.pkl # StandardScaler

│ ├── encoder.pkl # LabelEncoder

├── dataset/

│ └── CICIDS2017.csv # Dataset (not included in repo)

├── results/

│ └── evaluation\_report.txt

├── screenshots/

│ ├── confusion\_matrix.png

│ ├── accuracy\_graph.png

└── README.md # Project documentation





---



\## 🧭 How to Run the Project



1\. \*\*Clone the repository:\*\*

&nbsp;  ```bash

&nbsp;  git clone https://github.com/Seban007/Network-Intrusion-Detection-System.git

&nbsp;  cd Network-Intrusion-Detection-System





Create a virtual environment and install dependencies:



python -m venv venv

venv\\Scripts\\activate   # For Windows

pip install -r requirements.txt





Run model training:



python train\_model.py





Run intrusion detection (prediction):



python main.py



📸 Screenshots

Model Accuracy	Confusion Matrix



&nbsp;	

📊 Results Summary



Dataset: CICIDS2017



Model: XGBoost



Accuracy: ≈ 98.7%



Precision: ≈ 97.9%



Recall: ≈ 98.3%



F1-Score: ≈ 98.1%



The trained model achieved high detection accuracy for network intrusions with minimal false positives.



🧑‍💻 Author



Andrew Sebi Varghese

📧 Email: \[andrewssebivarghese@gmail.com]

💼 GitHub: https://github.com/Seban007



🪪 License



This project is open-source and available under the MIT License

.



