### 📄 `README.md`

# Iris Classification Web App 🌸

A simple machine learning web application built with **Flask** to classify iris flower species based on their physical dimensions using the classic **Iris dataset**.

---

## 🔍 Features

- 🧠 Predicts Iris species using a pre-trained model (Logistic Regression/SVM/XGBoost)
- 🎨 Clean UI for inputting sepal & petal features


---

## 📦 Project Structure

```
IrisClassificationApp/
│
├── static/              # CSS or image assets
├── templates/           # HTML frontend
│   └── index.html       
├── model/               # Saved ML model (.pkl)
├── app.py               # Flask app logic
├── requirements.txt     # Dependencies
├── LICENSE.md           
└── README.md
```

---

## 🚀 How to Run Locally

### 1. Clone this repo
```bash
git clone https://github.com/yourusername/iris-classification-app.git
cd iris-classification-app
```

### 2. Create and activate a conda environment (optional but recommended)
```bash
conda create -n iris-app python=3.9
conda activate iris-app
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
python app.py
```

Now go to `http://127.0.0.1:5000` in your browser.

---

## 🧠 Model

The model is trained on the Iris dataset from `sklearn.datasets` and saved using `joblib`. You can retrain or switch models using:

```python
from sklearn.datasets import load_iris
from sklearn.ensemble import RandomForestClassifier
from joblib import dump

X, y = load_iris(return_X_y=True)
clf = RandomForestClassifier().fit(X, y)
dump(clf, "model/iris_model.pkl")
```

---


## 📄 License

This project is licensed under the [MIT License](LICENSE.md).

---

## 🙋‍♂️ Author

Made with ❤️ by Jyoti

---



