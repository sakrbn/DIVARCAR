
# 🚗 Fine-Grained Vehicle Classification (FGIC) using ResNet + BCNN + Attention

This project presents a **smart image-based car model classification system**, using a combination of deep learning architectures:

- 🧠 ResNet50 for feature extraction  
- 🔁 Bilinear CNN (BCNN) for modeling fine-grained interactions  
- 👁️ Attention module for focusing on key parts of the image

It is designed for applications like:

- Vehicle insurance automation
- Smart parking systems
- Car listing platforms (e.g., Divar, Carvana)

---

## 📌 Key Features

- Transfer learning with **ResNet50**
- Fine-grained modeling using **Bilinear Pooling**
- Global **Attention block** to enhance feature localization
- Target test accuracy: **75%+**
- Uses real-world car image dataset with 5 classes

---

## 📂 Dataset Structure

```
Divar Image/
├── train/
│   ├── nissan/
│   ├── pegu/
│   ├── pride/
│   ├── samand/
│   └── toyota/
└── test/
    ├── nissan/
    ├── pegu/
    ├── pride/
    ├── samand/
    └── toyota/
```

---

## 📥 Dataset Source

The dataset was sourced from the following Figshare repository:

> 📎 [Car_Divar.zip – Figshare Dataset](https://figshare.com/articles/dataset/Car_Divar_zip/13907999)

---

## 🚀 Model Training Steps

1. Load and mount the dataset from Google Drive  
2. Use `ImageDataGenerator` with data augmentation  
3. Build the model with ResNet50 + Attention + BCNN  
4. Train the model for 30 epochs  
5. Save the best-performing model to `best_fgic_model.h5`

---

## 📈 Sample Results

| Epoch | Train Accuracy | Validation Accuracy |
|-------|----------------|---------------------|
| 10    | ~92%           | ~48%                |
| 30    | ~95%           | **~78–82%** (goal)  |

---

## 🧰 Requirements

```bash
pip install tensorflow
```

---

## 📦 Outputs

- Trained model: `best_fgic_model.h5`
- Notebook: `FGIC_model.ipynb`

---

## 🤝 Contributing

We welcome improvements, added car classes, or optimization efforts.  
Feel free to fork, raise issues, or submit pull requests.

---

## 📜 License

MIT License
