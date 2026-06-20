# 🔢 MNIST Dimensionality Reduction — PCA

Dimensionality reduction project applying **Principal Component Analysis (PCA)** on the MNIST-784 dataset to extract and visualize the most important patterns in 70,000 handwritten digit images.

---

## 🎯 Problem Statement

MNIST images have **784 features** (28×28 pixels each). PCA reduces this high-dimensional space to its most meaningful components — called **eigen-digits** — that capture the essential visual patterns differentiating digits 0–9.

- **Dataset**: MNIST-784 (OpenML)
- **Samples**: 70,000 handwritten digit images
- **Original features**: 784 (28×28 pixels)
- **Reduced components**: 100 principal components

---

## 🔄 Pipeline

### 1. Load & Normalize
- Fetch MNIST-784 from OpenML
- Normalize pixel values to [0, 1] range (divide by 255)
- Visualize sample digit

### 2. Apply PCA
- Reduce 784 dimensions → **100 principal components**
- `whiten=True` for normalized component variance

### 3. Visualize Eigen-Digits
- Display first **25 principal components** as 28×28 images
- Each eigen-digit represents a key visual pattern learned from the data

---

## 📊 Key Results

- **100 components** capture the most significant variance in 784-dimensional pixel space
- Eigen-digits (PC1–PC25) reveal the **stroke patterns, curves, and shapes** common across all handwritten digits
- PCA enables massive compression: **784 → 100 features** while retaining essential structure

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Dataset | MNIST-784 (via OpenML) |
| Dimensionality Reduction | PCA (Scikit-learn) |
| Visualization | Matplotlib |
| Data Handling | NumPy |

---

## 🚀 How to Run

```bash
pip install numpy matplotlib scikit-learn
```

Open `PCA_mnist_784_dataset_week8.ipynb` in Jupyter Notebook and run all cells.

> Note: First run will download MNIST dataset (~55MB) from OpenML automatically.

---

## 📁 Project Structure

```
mnist-pca-dimensionality-reduction/
│
├── PCA_mnist_784_dataset_week8.ipynb   # Main notebook
└── README.md
```

---

## 🔗 Related Projects

- [Handwritten Digits Classification](https://github.com/angelaadida/handwritten-digits-classification) — SVM, RandomForest, Decision Tree on digits

---

## 👩‍💻 Author

**Angela** — Data Scientist | AI • ML • GenAI • RAG  
📍 Kuala Lumpur, Malaysia  
🔗 [GitHub](https://github.com/angelaadida)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
