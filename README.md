# 🧠 Brain Tumor Classification with Deep Learning

A deep learning project to classify brain MRI images into four tumor types using a **custom CNN** and **MobileNetV2 (Transfer Learning)**, deployed with an interactive **Streamlit** app.

---

## 🧪 Dataset

- **Source**: [Brain Tumor MRI Dataset (Kaggle)](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
- **Classes**:
  - `glioma_tumor`
  - `meningioma_tumor`
  - `pituitary_tumor`
  - `no_tumor`

---

## 🚀 Models Used

### 🔧 Custom CNN
- 3 Convolutional Layers
- BatchNorm, MaxPooling, Dropout
- Flatten → Dense → Softmax

### 🧠 MobileNetV2
- Pretrained on ImageNet
- Fine-tuned on MRI dataset
- Lightweight and fast

---

## 🧠 Model Performance

| Model        | Accuracy | Precision | Recall | F1-Score |
|--------------|----------|-----------|--------|----------|
| Custom CNN   | 89%      | 88%       | 88%    | 88%      |
| MobileNetV2  | 94%      | 94%       | 94%    | 94%      |

> See `notebooks/model_comparison.ipynb` for evaluation plots and confusion matrices.

---

## 📊 Streamlit Web App

Launch the interactive web app to upload an MRI and get predictions:

```bash
streamlit run app.py
### Requirements
tensorflow==2.12.0
streamlit
numpy
pillow
scikit-learn
matplotlib
seaborn

📬 Author
Eraiyanbu Arulmurugan
Eraiyanbu-Git
