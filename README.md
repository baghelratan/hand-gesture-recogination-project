# Hand-Gesture-Recogination-Project MediaPipe Landmarks from the HaGRID Dataset  

## 📌 Overview  
This project focuses on classifying hand gestures using **landmark data extracted with MediaPipe** from the HaGRID dataset.  

The input is a **CSV file** containing hand landmarks (**x, y, z** coordinates of 21 key points).  
The output is a **trained machine learning model** that classifies hand gestures into different categories.  

---

## 🖐️ Hand Landmarks  
The landmarks used in this project are based on **MediaPipe's hand tracking model**, which detects **21 key points** on a hand.  

![img](https://github.com/user-attachments/assets/12fc5613-47e6-472b-bc4c-d013d1974524)



Each keypoint has **(x, y, z) coordinates**, which are used to classify gestures.  

---

## 📂 Dataset Details  
- The **HaGRID dataset** contains **18 different hand gestures**.  
- Each gesture is represented by **21 hand landmarks** extracted using MediaPipe.  
- The dataset is stored in a **CSV file**, where each row contains **landmark coordinates** and a **gesture label**.  

---

## 🚀 How to Run the Project  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/baghelratan/hand-gesture-recogination-project.git
cd hand-gesture-classification
```

### 2️⃣ Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Model in Google Colab  
- Open **Project_ML.ipynb** in Google Colab.  
- Upload the dataset (`hand_landmarks_data.csv`).  
- Run the notebook step by step to train the model.  

### 4️⃣ Real-Time Gesture Detection  
To test the model in real-time using your webcam, run:  
```bash
python real_time_demo.py
```

---

## 🎥 Demo  

https://github.com/user-attachments/assets/79868dbe-0ef1-42d2-8d16-d03bf17d7c16



Here is a **real-time demo of the model running on my hand**:  
 


## 📊 Project Deliverables  

### ✅ Google Colab Notebook  
- **Data Loading** – Importing the dataset.  
- **Data Visualization** – Plotting hand landmarks.  
- **Preprocessing** – Cleaning and normalizing data.  
- **Model Training** – Testing different classifiers.  
- **Evaluation** – Reporting accuracy, precision, recall, and F1-score.  
- **Conclusion** – Selecting the best model.  

---

## 🔥 Notes & Improvements  
- Hand landmarks are **recentered** (wrist as origin) to handle scale differences.  
- The **z** coordinate does not require additional processing.  
- The **output is stabilized** by taking the **mode of predictions** over a window.  

---
