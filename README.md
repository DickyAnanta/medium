# 🎓 Analisis Prediktif Performa Akademik Siswa Menggunakan Model Klasifikasi Adaptif Berbasis Random Forest

> *“Bisakah kecerdasan buatan membantu guru memahami siswa lebih baik?”*

---

## 🧠 Abstrak (Bahasa Indonesia)

Penelitian ini mengembangkan model **klasifikasi adaptif** untuk memprediksi *performa akademik siswa* menggunakan algoritma **Random Forest Classifier**. Dataset berasal dari [UCI Machine Learning Repository – *Student Performance*](https://archive.ics.uci.edu/dataset/320/student+performance), yang berisi data demografis, sosial, perilaku, dan nilai akhir siswa di Portugal.

Tahapan pengolahan data meliputi pembersihan, pengkodean kategori menjadi numerik, pembentukan target biner berdasarkan median nilai akhir, dan pelatihan model menggunakan pembagian data 80:20.  
Model ini mencapai **akurasi 83,6%**, dengan variabel paling berpengaruh meliputi *waktu belajar, jumlah kegagalan, absensi,* dan *hubungan keluarga*.

Hasilnya menunjukkan bahwa pendekatan **machine learning adaptif** mampu mendeteksi risiko akademik secara dini dan mendukung *decision-making* berbasis data di bidang pendidikan.

---

## ✨ Abstract (English)

This study develops an **adaptive classification model** to predict students’ academic performance using the **Random Forest Classifier** algorithm. The dataset was obtained from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance), containing demographic, social, behavioral, and academic records of Portuguese secondary school students.

After data cleaning, categorical encoding, binary target creation, and training-test split (80:20), the model achieved **83.6% accuracy**.  
Key predictors include *study time, number of failures, absences,* and *family relationships*.  
Results show that adaptive machine learning effectively identifies at-risk students early and supports **data-driven educational policy-making**.

---

## 🎯 Latar Belakang

Pendidikan modern kini semakin kompleks. Guru, konselor, dan pengambil kebijakan sering menghadapi tantangan dalam memahami faktor-faktor yang memengaruhi keberhasilan akademik siswa.  
Di sinilah **Educational Data Mining (EDM)** berperan — sebuah pendekatan berbasis *machine learning* yang menganalisis data siswa untuk menemukan pola dan wawasan tersembunyi.

Dataset *Student Performance* dari UCI menjadi fondasi penelitian ini. Data ini merepresentasikan **siswa sekolah menengah di Portugal**, lengkap dengan informasi sosial, perilaku belajar, dan nilai akhir mereka.  
Tujuannya: **memprediksi performa akademik siswa secara adaptif**, menggunakan algoritma *Random Forest*.

---

## ⚙️ Metodologi dan Penjelasan Kode

Notebook yang digunakan mencakup beberapa tahap penting:

1. **Pengunduhan dataset** melalui `kagglehub` dari repositori UCI.  
2. **Instalasi pustaka** `dowhy` dan `shap` untuk mendukung analisis kausalitas dan interpretabilitas model.  
3. **Praproses data**:
   - Mengubah variabel kategorikal menjadi numerik dengan `LabelEncoder`.  
   - Membentuk kolom target biner berdasarkan median nilai akhir (`G3`).  
4. **Pelatihan model**:
   - Menggunakan algoritma **Random Forest Classifier** dari *scikit-learn*.  
   - Membagi data menjadi **train-test split (80:20)**.  
5. **Evaluasi performa** dengan metrik:
   - Akurasi  
   - Precision & Recall  
   - Confusion Matrix  

Tujuan utama kode ini adalah membangun model yang **adaptif terhadap distribusi nilai siswa** — bukan sekadar klasifikasi tetap, tetapi menyesuaikan batas kelas berdasarkan distribusi data aktual.

---

## 📊 Hasil dan Pembahasan

Hasil pengujian menunjukkan bahwa:

- **Akurasi model:** 83,6%  
- **Prediksi antar kelas:** seimbang antara kategori *berperforma tinggi* dan *rendah*  
- **Fitur paling berpengaruh:**  
  - Waktu belajar  
  - Jumlah kegagalan  
  - Absensi  
  - Hubungan keluarga  

Interpretasi menggunakan *feature importance* mengungkap bahwa:
- Semakin lama waktu belajar, semakin tinggi kemungkinan nilai akhir yang baik.  
- Jumlah kegagalan dan absensi berkorelasi negatif dengan performa.  
- Dukungan keluarga memberi kontribusi signifikan terhadap hasil akademik siswa.

---

## 🧩 Kesimpulan

Model **Random Forest Classifier** terbukti efektif untuk memprediksi performa akademik siswa.  
Dengan pendekatan klasifikasi adaptif berbasis median, sistem menjadi lebih fleksibel terhadap variasi populasi siswa.  

Pendekatan ini dapat:
- Membantu guru mengidentifikasi siswa yang berisiko gagal.  
- Menjadi alat bantu keputusan berbasis data untuk institusi pendidikan.  
- Menunjukkan potensi besar *machine learning* dalam mendukung kebijakan pendidikan cerdas (*smart education policy*).

---

## 📚 Referensi (APA 7th Edition)

- Breiman, L. (2001). *Random Forests*. *Machine Learning, 45*(1), 5–32. https://doi.org/10.1023/A:1010933404324  
- Cortez, P., & Silva, A. (2008). *Using Data Mining to Predict Secondary School Student Performance*. University of Minho, Portugal. Retrieved from https://archive.ics.uci.edu/dataset/320/student+performance  
- Lundberg, S. M., & Lee, S.-I. (2017). *A Unified Approach to Interpreting Model Predictions*. *NeurIPS*, 30, 4765–4774.  
- Pedregosa, F. et al. (2011). *Scikit-learn: Machine Learning in Python*. *Journal of Machine Learning Research*, 12, 2825–2830.  
- Pearl, J. (2009). *Causality: Models, Reasoning and Inference* (2nd ed.). Cambridge University Press.  

---

### ✍️ Penulis
**Dicky Ananta Yudha**

**Varl Aqshal Al-Hafizh**

**Galih Ar Rasyad**  

Mahasiswa Teknik Informatika  
Peneliti muda dalam bidang *Machine Learning* dan *Educational Data Mining*
