# AI vs Human Image Detector - Backend & GUI

This project is a deep learning-based image classifier that predicts whether an uploaded image is **AI-generated or Human-made** using a trained Convolutional Neural Network (CNN) model. It provides a **Graphical User Interface (GUI) using Tkinter** for easy image upload and classification.

---

## 📂 Project Structure

```
📂 project_root/
 ├── 📂 model/                 # Contains the trained deep learning model
 │    ├── ai_vs_human_classifier.h5  # Saved trained model
 │
 ├── 📂 script/                # Contains the backend scripts
 │    ├── server.py           # Flask backend to serve predictions (optional)
 │    ├── requirements.txt    # List of dependencies
 │
 ├── 📂 gui/                   # GUI for image classification
 │    ├── gui.py              # Tkinter-based GUI
 │
 ├── README.md                # Project documentation
```

---

## 🚀 Setup & Installation

### **1️⃣ Install Python & Virtual Environment**
Make sure you have **Python 3.8+** installed. Then, create and activate a virtual environment:

```bash
python -m venv venv  # Create virtual environment
source venv/bin/activate  # Activate on Mac/Linux
venv\Scripts\activate  # Activate on Windows
```

### **2️⃣ Install Required Dependencies**
Run the following command inside the `script/` or `gui/` folder:

```bash
pip install -r requirements.txt
```

If you don’t have `requirements.txt`, install dependencies manually:
```bash
pip install tensorflow opencv-python pillow numpy tkinter
```

---

## 🖥️ Running the GUI

### **1️⃣ Start the Tkinter GUI**
Run the following command from the `gui/` folder:

```bash
python gui.py
```

This will open a GUI where you can upload an image and get a prediction.

### **2️⃣ How It Works**
1. Click **"Upload Image"** to select an image.
2. The image is **displayed in the GUI**.
3. The trained model processes the image.
4. The result (**AI-Generated or Human-Generated**) is displayed in the GUI.

---

## 🔍 How the Model Works

1. The **trained model** (`ai_vs_human_classifier.h5`) is loaded from the `model/` folder.
2. When an image is uploaded, it is **preprocessed** (resized, normalized) before being passed to the model.
3. The **model predicts** whether the image is AI-generated or human-made.
4. The result is displayed in the GUI.

---

## 🛠 Troubleshooting

### **1️⃣ GUI Not Opening?**
- Make sure Tkinter is installed:
  ```bash
  python -m tkinter
  ```
- If you get an error, install it with:
  ```bash
  pip install tk
  ```

### **2️⃣ Getting Incorrect Predictions?**
- Ensure the model is properly trained.
- Try retraining the model with more balanced data.

---

## 📌 Future Improvements
✅ Add more model optimization techniques  
✅ Improve GUI styling and responsiveness  
✅ Deploy the model as a standalone application  

---

## 📜 License
This project is **open-source** and free to use under the MIT License.
