# Sentiment Analysis Food Estate Merauke

## Deskripsi

Notebook ini berisi implementasi analisis sentimen terhadap topik _Food Estate Merauke_ menggunakan teknik pemrosesan teks dan klasifikasi machine learning. Analisis ini bertujuan untuk memahami bagaimana opini publik terhadap kebijakan _Food Estate_ yang dikembangkan di Merauke, Indonesia.

Proses yang dilakukan dalam notebook ini meliputi:

1. **Pemrosesan Data**:
   - Data diperoleh melalui _scraping_ komentar dari YouTube terkait topik _Food Estate Merauke_.
   - Dataset kemudian di-_shuffle_ untuk menghindari bias dalam model.
2. **Preprocessing Data**:

   - **Pembersihan Teks**: Menghilangkan angka, simbol, tanda kurung, dan emotikon.
   - **Normalisasi Kata**: Mengubah kata tidak baku atau singkatan ke bentuk yang benar.
   - **Stopword Removal**: Menghapus kata-kata umum yang tidak memiliki makna signifikan dalam analisis sentimen.
   - **Stemming**: Mengubah kata ke bentuk dasar menggunakan Sastrawi.

3. **Analisis Sentimen**:
   - Implementasi model klasifikasi untuk menentukan sentimen positif, negatif, atau netral.
   - Evaluasi performa model menggunakan metrik seperti _accuracy_, _precision_, _recall_, dan _F1-score_.

---

## Hasil Analisis Sentimen

### **Confusion Matrix dan Evaluasi Model**

Confusion Matrix menunjukkan performa model dalam mengklasifikasikan sentimen komentar ke dalam tiga kategori: **Negatif (-1), Netral (0), dan Positif (1).**  
Dari hasil evaluasi model, diperoleh metrik berikut:

- **Akurasi model** sebesar **80%**, yang menunjukkan tingkat ketepatan model dalam memprediksi sentimen.
- **F1-score** untuk masing-masing kelas:
  - **Negatif (-1):** 0.70
  - **Netral (0):** 0.76
  - **Positif (1):** 0.86  
    Model memiliki performa terbaik dalam mengenali sentimen **positif**, sementara sentimen **negatif** memiliki recall yang lebih rendah.

### **Distribusi Sentimen**

Grafik _pie chart_ menunjukkan distribusi sentimen dari komentar yang telah diklasifikasikan:

- **60% komentar bersentimen positif**, menunjukkan bahwa mayoritas pengguna memiliki opini yang mendukung atau menyetujui program _Food Estate_ di Merauke.
- **22.2% komentar bersentimen netral**, yang berarti komentar tersebut tidak menunjukkan kecenderungan opini yang jelas terhadap kebijakan tersebut.
- **17.8% komentar bersentimen negatif**, yang menunjukkan adanya ketidakpuasan atau kritik dari sebagian masyarakat terhadap program ini.

### **Kesimpulan**

- Mayoritas komentar dari YouTube menunjukkan sentimen **positif** terhadap _Food Estate Merauke_.
- Model klasifikasi yang digunakan memiliki tingkat akurasi yang cukup baik (**80%**) dalam mengklasifikasikan sentimen komentar.
- Sentimen **negatif** yang ada mengindikasikan bahwa masih terdapat kritik atau kekhawatiran dari masyarakat mengenai program ini.
