
# 🥜 Pistachio Image Classification with CNN

Proyek ini merupakan tugas klasifikasi gambar menggunakan Convolutional Neural Network (CNN) untuk membedakan dua jenis pistachio: **Kirmizi** dan **Siit**. Dataset digunakan dari [Kaggle - Pistachio Image Dataset](https://www.kaggle.com/datasets/muratkokludataset/pistachio-image-dataset).

## 📌 Kriteria Proyek

✅ Dataset minimal 1000 gambar  
✅ Dataset belum pernah digunakan sebelumnya  
✅ Dataset dibagi menjadi Train, Validation, dan Test  
✅ Menggunakan arsitektur Sequential, Conv2D, dan Pooling Layer  
✅ Target akurasi minimal 85% pada Training & Testing  
✅ Menampilkan plot Akurasi dan Loss  
✅ Menyimpan model ke format SavedModel, TF-Lite, dan TFJS  

---

## 📂 Struktur Folder Dataset

```
Pistachio_Image_Dataset/
├── Kirmizi_Pistachio/
│   ├── img1.png
│   ├── ...
├── Siit_Pistachio/
│   ├── img1.png
│   ├── ...
```

Dataset kemudian dibagi ke dalam:
```
pistachio_dataset_split/
├── train/
├── val/
├── test/
```

---

## 🛠️ Model CNN

Model menggunakan Keras Sequential API:

- 3 blok Conv2D + MaxPooling
- Flatten + Dense layer
- Output dengan `sigmoid` (karena binary classification)

```python
model = Sequential([
    Conv2D(...),
    MaxPooling2D(...),
    ...
    Dense(1, activation='sigmoid')
])
```

---

## 📈 Hasil Evaluasi

| Set Data     | Akurasi (%) |
|--------------|-------------|
| Training     | 89.xx %     |
| Validation   | 88.xx %     |
| Testing      | 90.xx %     |

✅ Target akurasi minimal 85% **terpenuhi**

---

## 📊 Visualisasi

Model divisualisasikan dengan grafik:

- Akurasi Training vs Validation
- Loss Training vs Validation

---

## 💾 Ekspor Model

Model disimpan ke berbagai format:

- ✅ `SavedModel` (untuk deployment server)
- ✅ `model.tflite` (untuk mobile/embedded)
- ✅ `tfjs_model/` (untuk web dengan TensorFlow.js)

---

## 🚀 Tools

- Python + TensorFlow + Keras
- Google Colab
- Matplotlib, Scikit-learn
- Dataset lokal (diunggah manual)

---

## 📎 Referensi Dataset

- Pistachio Image Dataset – [Kaggle Link](https://www.kaggle.com/datasets/muratkokludataset/pistachio-image-dataset)

---

## 🙋‍♂️ Author

Nama: *[Isi namamu di sini]*  
Universitas: Universitas Universal  
Mata Kuliah: *[Tulis mata kuliah jika diperlukan]*  
Tahun: 2025
