## 🍄 Proyek Klasifikasi Jamur

Proyek ini merupakan implementasi model klasifikasi biner untuk **memprediksi apakah suatu spesimen jamur bersifat dapat dimakan atau beracun** berdasarkan fitur-fitur deskriptif yang tersedia. Model dibangun menggunakan algoritma **Random Forest**, yang terkenal karena kemampuannya dalam menghasilkan prediksi yang akurat dan menangani data kategori dengan baik.

Dengan memanfaatkan teknik machine learning dan evaluasi berbasis confusion matrix, model ini memberikan performa yang sangat tinggi dan dapat diandalkan untuk tugas klasifikasi.

### 🧠 Algoritma yang Digunakan

Model dikembangkan menggunakan algoritma **Random Forest**, yang merupakan metode ensemble dari beberapa decision tree. Random Forest cocok untuk dataset ini karena:
- Mampu menangani fitur-fitur kategori dengan baik
- Tahan terhadap overfitting
- Memberikan interpretasi fitur yang cukup kuat

### 📊 Evaluasi Model

Model diuji menggunakan 1.625 sampel data dan menghasilkan metrik evaluasi sebagai berikut:

#### Confusion Matrix
| Kelas Aktual | Prediksi: 0 | Prediksi: 1 |
|--------------|-------------|-------------|
| 0 (Negatif)  | 843         | 0           |
| 1 (Positif)  | 23          | 759         |

#### Metrik Kinerja
- **Akurasi**: `98.58%`
- **Presisi (Kelas Positif)**: `100%`
- **Recall (Kelas Positif)**: `97.06%`
- **F1 Score**: `98.51%`

#### Analisis
Model ini menunjukkan **presisi sempurna** tanpa kesalahan tipe I (false positive), menjadikannya ideal untuk aplikasi seperti deteksi racun atau keamanan bahan makanan. Meskipun terdapat 23 false negative, performa keseluruhan tetap seimbang dan kuat.

### 🗂️ Sumber Dataset

Dataset yang digunakan dalam proyek ini tersedia secara publik di Kaggle:  
👉 [UCI Mushroom Classification Dataset](https://www.kaggle.com/datasets/uciml/mushroom-classification)

Dataset ini terdiri dari berbagai fitur kategori seperti bentuk, warna, permukaan, dan bau yang digunakan untuk memprediksi label “edible” atau “poisonous”.

### 🙏 Ucapan Terima Kasih

Terima kasih kepada:
- **UCI dan Kaggle** atas ketersediaan dataset jamur yang berkualitas
- Komunitas open-source yang telah membagikan dokumentasi dan tutorial yang membantu pengembangan proyek ini
- Semua pihak yang telah memberi dukungan dan umpan balik dalam proses eksperimen dan evaluasi

---

> _Catatan_: Proyek ini dapat dikembangkan lebih lanjut melalui tuning hyperparameter, validasi silang, serta pengembangan API menggunakan FastAPI atau Flask untuk keperluan deployment dan integrasi lebih lanjut.
