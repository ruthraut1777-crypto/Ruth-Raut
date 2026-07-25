[README.md](https://github.com/user-attachments/files/30371064/README.md)
# Neural Network Classification — Internship Portfolio

Two supervised deep learning projects built with **TensorFlow / Keras** as part of an internship program: one predicts tumor malignancy from clinical measurements, the other reads handwritten digits from images.

---

### 🩺 Project 1 — Breast Cancer Classification

Predicts whether a tumor is **Malignant** or **Benign** from 30 diagnostic measurements.

| | |
|---|---|
| Dataset | Breast Cancer Wisconsin (Diagnostic) — via `sklearn.datasets` |
| Samples | 569 (212 malignant / 357 benign) |
| Model | `Flatten → Dense(20, ReLU) → Dense(2, Sigmoid)` |
| Result | **96.5%** test accuracy |

📁 `breast_cancer_classification/`
- `Breast_Cancer_Classification_with_Neural_Network.ipynb` — full notebook, code + outputs
- `Breast_Cancer_Classification_Report.docx` — write-up

---

### 🔢 Project 2 — MNIST Digit Classification

Recognizes handwritten digits (0–9) from 28x28 pixel images, and classifies a custom test image.

| | |
|---|---|
| Dataset | MNIST — via `keras.datasets` |
| Samples | 60,000 train / 10,000 test |
| Model | `Flatten → Dense(50, ReLU) → Dense(50, ReLU) → Dense(10, Softmax)` |
| Result | **97.1%** test accuracy (98.9% training) |

📁 `mnist_digit_classification/`
- `MNIST_Digit_classification_using_Neural_Networks.ipynb` — full notebook, code + outputs
- `MNIST_Project.docx` — original project brief
- `3-digit.PNG` — sample custom image used to test the predictive system
- `MNIST_Digit_Classification_Report.docx` — write-up

---

### 🎞 Presentations

📁 `presentations/` — 10-slide decks summarizing each project (objective, dataset, architecture, results, conclusion)
- `Breast_Cancer_Classification_Presentation.pptx`
- `MNIST_Digit_Classification_Presentation.pptx`

---

## Running the notebooks

Both notebooks were built and tested in **Google Colab** — no local setup required if you use Colab.

To run locally instead:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow seaborn opencv-python pillow
jupyter notebook
```

Then open either `.ipynb` and run all cells top to bottom. Both datasets load automatically (scikit-learn and Keras both bundle/fetch their data — no manual download needed for the cancer dataset; MNIST downloads on first run).

For the MNIST predictive-system cell, make sure `3-digit.PNG` is available in the working directory.

---

## Stack

`Python` · `TensorFlow / Keras` · `scikit-learn` · `NumPy` · `Pandas` · `Matplotlib` · `Seaborn` · `OpenCV`

---

*Submitted as part of an internship program, July 2026.*
