# 📊 Analisis Kepuasan Mahasiswa terhadap E-Learning Universitas Nurul Huda Menggunakan Algoritma C4.5

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Status](https://img.shields.io/badge/Status-Selesai-brightgreen.svg)

## 📌 Ikhtisar
Repositori ini berisi kode analisis untuk penelitian evluasi tingkat kepuasan mahasiswa terhadap sistem e-learning di Universitas Nurul Huda (UNUHA) menggunakan **algoritma pohon keputusan C4.5** berbasis **model SERVQUAL**.

Penelitian ini bertujuan:
- Mengidentifikasi faktor utama yang memengaruhi kepuasan mahasiswa.
- Membangun model klasifikasi untuk memprediksi tingkat kepuasan ("Puas" atau "Tidak Puas").

📈 Hasil analisis:
- **Akurasi**: 84%
- **F1-Score**: Puas (0,86), Tidak Puas (0,82)
- **F1-Macro (5-fold)**: 0,91
- **Faktor utama**: AS3 (Gain ratio 0,312723), EP1 (0,309469)

---

## ⚙️ Prasyarat

Untuk menjalankan kode, pastikan Anda memiliki:

- Python 3.8 atau lebih tinggi
- Google Colab (disarankan)
- Pustaka Python berikut:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn graphviz joblib
```

---

## ▶️ Cara Menjalankan

### 1. Kloning Repositori

```bash
git clone https://github.com/nama-anda/elearning-satisfaction-c45.git
```

### 2. Siapkan Google Drive (Jika Menggunakan Colab)

- Mount Google Drive di Colab
- Perbarui `data_path`, `output_path`, dan `model_path`

### 3. Siapkan Dataset

Pastikan file Dataset berisi:

- **15 atribut**: TN1–TN3, RL1–RL3, RS1–RS3, AS1–AS3, EP1–EP3
- **Target**: `Kepuasan` (label: *Puas* / *Tidak Puas*)
- **Opsional**: ID Responden

### 4. Jalankan Analisis

- Buka `Analisis_Gain_Ratio_C4.5.ipynb` di Google Colab atau lokal
- Jalankan skrip untuk:
  - Pra-pemrosesan data
  - Hitung gain ratio
  - Latih dan evaluasi model C4.5
  - Visualisasi hasil
  - Validasi silang dan pohon manual

### 5. Lihat Keluaran

Hasil analisis:
- Visualisasi pohon dan matriks kebingungan
- Tabel gain ratio
- Metrik evaluasi dan validasi silang

---

## 📊 Dataset

Dataset terdiri dari hasil kuesioner 125 mahasiswa UNUHA. Format kolom:

- **Atribut SERVQUAL**:
  - Tangibles (TN1, TN2, TN3)
  - Reliability (RL1, RL2, RL3)
  - Responsiveness (RS1, RS2, RS3)
  - Assurance (AS1, AS2, AS3)
  - Empathy (EP1, EP2, EP3)
- **Target variabel**: `Kepuasan` (dengan label: Puas / Tidak Puas)
- Dataset ini bersifat privat dan tidak disertakan dalam repositori.

---

## 🏆 Hasil Utama

| Atribut Utama | Deskripsi                                               | Gain Ratio |
|---------------|----------------------------------------------------------|-------------|
| AS3           | Penguasaan dosen terhadap materi dan teknologi pembelajaran | 0.312723    |
| EP1           | Personalisasi pembelajaran                               | 0.309469    |
| AS2           | Desain aktivitas pembelajaran                            | 0.298309    |

📈 **Kinerja Model:**
- **Akurasi**: 84%
- **F1-Score**:
  - Puas: 0.86
  - Tidak Puas: 0.82
- **F1-Macro (CV)**: 0.91
- **Pohon Keputusan**:
  - Akar: AS3
  - Jumlah simpul: 16
  - Kedalaman maksimum: 3

---

## 🤝 Kontribusi

Jika Anda ingin berkontribusi:

1. Fork repositori ini
2. Buat branch baru:
   ```bash
   git checkout -b fitur-baru
   ```
3. Lakukan perubahan dan commit
4. Kirim Pull Request

---

## 📬 Kontak

Untuk pertanyaan atau dukungan, hubungi:

- **Miftakhul Rahman**: miftakhulr@student.unuha.ac.id  
---

## 🙏 Ucapan Terima Kasih

Terima kasih kepada **Universitas Nurul Huda**, dosen pembimbing, dan semua pihak yang telah mendukung penelitian ini.  
Kontribusi dan masukan Anda sangat dihargai!

---
```
