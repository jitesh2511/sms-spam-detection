# 📧 SMS Spam Detection

A machine learning project that classifies SMS messages as **spam** or **ham** using **logistic regression** — implemented entirely from scratch in a Jupyter Notebook using `numpy` and `pandas`. This is my first ML Project and the first ever project on GitHub too.

---

## 🚀 Project Overview

This project builds a binary classifier to detect whether an incoming SMS message is spam. It includes:

- Data cleaning and preprocessing
- Text vectorization without using external ML libraries
- Logistic regression from scratch (no `scikit-learn`)
- Training loop, prediction, and evaluation metrics
- Final accuracy, recall, and F1 score

---

## 🗂️ Project Structure

```
sms-spam-detection/
├── data/
│   └── spam.csv               # Raw SMS Spam Collection Dataset
├── sms_spam_detector.ipynb    # Main notebook with code and output
├── requirements.txt           # Project dependencies
├── .gitignore                 # Ignored files and folders
├── LICENSE                    # MIT License
└── README.md                  # You're here!
```

---

## 🧪 Dataset

The dataset used is [SMS Spam Collection](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset) — a collection of 5,574 SMS messages labeled as **spam** or **ham**.

- Format: CSV
- Columns: `label`, `message`
- Location: `data/spam.csv` (included in this repo)

---

## ⚙️ How to Run

### 📦 Step 1: Install Dependencies
```bash
pip install -r requirements.txt
```

### 🧠 Step 2: Open the Notebook
```bash
jupyter notebook sms_spam_detector.ipynb
```

### ▶️ Step 3: Run All Cells
The notebook is self-contained and will:
- Load and clean the data
- Vectorize the text messages
- Train a logistic regression model
- Evaluate on a test set

(If you notice, I initialized the weights to zero rather than using np.random.randn(), it was because I trained the model using both random initialized weights and weights initialized as zeros, but the model performed better when I initialized the weights to zero)

---

## 📊 Final Evaluation (Example)

| Metric        |  Value   |
|---------------|----------|
| Accuracy      |  95.45%  |
| Precision     |  96.49%  |
| Recall        |  88.71%  |
| False Alarm   |  3.51%   |
| F1 Score      |  92.44   |

*These values may vary slightly depending on train/test split or threshold.*

---

## 🧰 Technologies Used

- Python 3.x
- Jupyter Notebook
- `numpy`, `pandas`, `matplotlib`, `tqdm`

---

## 📚 What I Learned

This project helped me understand:
- How logistic regression works under the hood
- How to process and vectorize text without built-in libraries
- How to tune classification thresholds to balance precision and recall

---

## 📬 Contact

> *Made with curiosity by Jitesh Krishna — a college student learning how machines learn.*

Feel free to fork ⭐, star ⭐, or open an issue.  
Check out more projects at [https://github.com/JiteshKrishna](https://github.com/JiteshKrishna)

---

## 📌 License

This project is open-source under the [MIT License](LICENSE).
