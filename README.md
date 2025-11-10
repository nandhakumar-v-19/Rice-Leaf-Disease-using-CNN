# 🌾 Rice Leaf Disease Detection

## 📘 Project Overview
This project — **PRCP-1001: Rice Leaf Disease Detection** — focuses on identifying major rice plant diseases using **Convolutional Neural Networks (CNN)**.  
It automates the detection of three critical rice leaf diseases, supporting farmers and researchers with early diagnosis to prevent large-scale crop damage.

---

## 🎯 Problem Statement
The goal of this project is to:
1. **Perform complete data analysis** on the provided rice leaf image dataset.  
2. **Develop a CNN model** capable of classifying rice leaf diseases into three categories:
   - **Leaf Smut**
   - **Brown Spot**
   - **Bacterial Leaf Blight**
3. **Apply data augmentation** and analyze its effects on model performance.  
4. **Compare multiple deep learning models** and identify the most effective one for production.  
5. **Document challenges faced** during preprocessing, training, and evaluation with their corresponding solutions.

---

## 📂 Dataset Information
**Source:** [Rice Leaf Disease Dataset](https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1001-RiceLeaf.zip)  
- Total Images: **120 JPG files**
- Classes: **3** (40 images per class)
  - Leaf Smut
  - Brown Spot
  - Bacterial Leaf Blight

---

## 🧠 Model & Approach
- **Model Used:** Convolutional Neural Network (CNN)
- **Techniques Applied:**
  - Image preprocessing (resizing, normalization)
  - **Data Augmentation** (rotation, flipping, zooming, brightness adjustment)
  - Model evaluation using **accuracy**, **confusion matrix**, and **classification report**
- **Comparison Models:** CNN variants with different optimizers and dropout layers to assess generalization and overfitting.

---

## ⚙️ Tech Stack
- **Language:** Python  
- **Libraries:** TensorFlow / Keras, NumPy, OpenCV, Matplotlib  
- **Environment:** Jupyter Notebook  

---

## 📁 Repository Structure
```
Rice-Leaf-Disease-using-CNN/
│
├── PRCP-1001-RiceLeaf-Disease-Detection.ipynb   # Main Jupyter Notebook
├── dataset/                                     # Image dataset (3 classes)
├── outputs/                                     # Sample predictions and graphs
├── requirements.txt                             # Dependencies
└── README.md                                    # Project documentation
```

---

## 🚀 How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/nandhakumar-v-19/Rice-Leaf-Disease-using-CNN.git
   cd Rice-Leaf-Disease-using-CNN
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open the Jupyter Notebook:**
   ```bash
   jupyter notebook PRCP-1001-RiceLeaf-Disease-Detection.ipynb
   ```

4. **Run all cells** to preprocess the dataset, train the CNN, and view results.

---

## 📊 Results
- The CNN model achieved **high accuracy** in detecting and classifying rice leaf diseases.  
- Evaluation metrics such as accuracy, precision, recall, and F1-score were visualized.  
- The **confusion matrix** confirmed effective separation of all three disease categories.  
- **Data augmentation** significantly improved performance by reducing overfitting.

---

## 🧩 Model Comparison Report
| Model Variant | Optimizer | Accuracy | Key Observations |
|----------------|------------|-----------|------------------|
| CNN (Base) | Adam | 91% | Fast convergence, slight overfitting |
| CNN + Dropout | Adam | 93% |  Highest accuracy and Better generalization |

**Best Model:** CNN + Dropout (93% accuracy)

---

## 💡 Challenges & Solutions
| Challenge | Description | Solution Implemented |
|------------|--------------|----------------------|
| Small dataset size | Limited 120 images | Applied extensive **data augmentation** |
| Class imbalance | Unequal class samples during training | Used **balanced batch generation** |
| Overfitting | Model memorizing training images | Added **dropout layers** and **augmentation** |
| Low clarity images | Noise and lighting variation | Applied **image enhancement filters** |

---

## 🏁 Conclusion
This project successfully demonstrates the use of **deep learning for agricultural disease detection**.  
By leveraging CNN and augmentation techniques, we achieved a robust classification model that can support **automated plant health monitoring** systems.  

---

**📩 Repository:** [Rice Leaf Disease using CNN](https://github.com/nandhakumar-v-19/Rice-Leaf-Disease-using-CNN)
