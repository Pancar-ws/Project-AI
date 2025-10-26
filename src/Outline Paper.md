### Judul:

**Implementasi Convolutional Neural Network (CNN) untuk Identifikasi Jenis Patah Tulang dari Citra Rontgen**

---
### **BAB I — Pendahuluan**

#### 1.1 Latar Belakang
- Proses identifikasi jenis patah tulang dari citra rontgen masih dilakukan manual.
- Metode manual bersifat subjektif dan memerlukan ketelitian tinggi.
- CNN dapat membantu meningkatkan akurasi dan efisiensi diagnosis.
#### 1.2 Rumusan Masalah
1. Bagaimana mengimplementasikan CNN untuk mengidentifikasi jenis patah tulang dari citra rontgen?
2. Bagaimana proses _training_ dan _testing_ model CNN terhadap dataset citra rontgen?
3. Seberapa akurat model CNN dalam mengklasifikasikan jenis patah tulang?
#### 1.3 Tujuan Penelitian
- Mengimplementasikan algoritma CNN untuk klasifikasi citra rontgen tulang.
- Melakukan pelatihan dan pengujian terhadap dataset citra rontgen.
- Mengetahui performa akurasi model CNN dalam membedakan jenis patah tulang.
#### 1.4 Manfaat Penelitian
- Memberikan kontribusi terhadap penerapan _AI_ di bidang kesehatan.
- Membantu mempercepat proses diagnosis awal patah tulang.
- Menjadi dasar pengembangan sistem pendukung keputusan medis.
---
### **BAB II — Tinjauan Pustaka**
_(Berisi teori dan konsep dasar yang mendukung penelitian)_
#### 2.1 Kecerdasan Buatan (_Artificial Intelligence_)
- Pengertian AI secara umum.
- Penerapan AI dalam bidang medis.
#### 2.2 Pembelajaran Mendalam (_Deep Learning_)
- Konsep dasar deep learning dan perbedaannya dengan _machine learning_ biasa.
- Arsitektur jaringan saraf tiruan (ANN) dan lapisan-lapisannya.
#### 2.3 Convolutional Neural Network (CNN)
- **Pengertian CNN**: jaringan saraf tiruan yang dirancang untuk memproses data berbentuk citra.
- **Struktur CNN**:
    - _Input Layer_: menerima citra sebagai masukan.
    - _Convolution Layer_: mengekstraksi fitur dengan filter/kernel.
    - _Pooling Layer_: mengurangi dimensi fitur untuk efisiensi komputasi.
    - _Fully Connected Layer_: melakukan klasifikasi berdasarkan fitur hasil ekstraksi.
- **Cara kerja CNN secara umum** (dari input gambar hingga hasil prediksi).
- Kelebihan CNN dibanding algoritma lain (misalnya dibanding SVM atau ANN biasa).
#### 2.4 Citra Rontgen dan Patah Tulang
- Penjelasan dasar mengenai citra rontgen (X-ray) dan bagaimana citra dihasilkan.
- Jenis-jenis patah tulang yang umum (misalnya: transversal, spiral, kominutif, dan lainnya).
- Tantangan dalam mengenali jenis patah tulang dari citra (noise, kontras, posisi).
#### 2.5 Penelitian Terkait
- Ringkasan beberapa penelitian terdahulu yang menggunakan CNN untuk klasifikasi citra medis.
- Celah penelitian yang menjadi dasar mengapa penelitianmu perlu dilakukan (misalnya: dataset terbatas, jenis fraktur belum spesifik, dsb).
---
### **BAB III — Metodologi Penelitian**
#### 3.1 Desain Penelitian
- Penjelasan alur penelitian: mulai dari pengumpulan data, _preprocessing_, _training_, _testing_, hingga evaluasi.
    > Misalnya ditampilkan dalam bentuk diagram alir.
#### 3.2 Dataset
- Sumber dataset (misalnya: dataset rontgen dari kaggle atau data klinik).
- Jumlah data dan jenis patah tulang yang diklasifikasikan.
- Format citra (ukuran, format file, resolusi).
#### 3.3 _Preprocessing Data_
- Normalisasi ukuran citra.
- Augmentasi (rotasi, flipping, zooming) untuk memperbanyak variasi data.
- Pembagian data menjadi _training set_ dan _testing set_.
#### 3.4 Implementasi CNN
- Arsitektur model CNN yang digunakan (jumlah layer, filter size, activation function, optimizer, dll).
- Framework dan tools (misal: TensorFlow, Keras, Google Colab).
- Parameter training: _batch size_, _epochs_, _learning rate_.
#### 3.5 Evaluasi Model
- Metrik yang digunakan: akurasi, presisi, recall, F1-score.
- Visualisasi hasil menggunakan _confusion matrix_.
---
### **BAB IV — Hasil dan Pembahasan**
#### 4.1 Hasil Pelatihan dan Pengujian
- Hasil _training loss_ dan _accuracy_.
- Grafik akurasi terhadap epoch.
#### 4.2 Evaluasi Performa
- Perbandingan hasil CNN terhadap data uji.
- Interpretasi nilai akurasi dan kesalahan klasifikasi.
#### 4.3 Analisis Hasil
- Penjelasan mengapa model bekerja baik atau kurang baik.
- Faktor yang memengaruhi hasil (dataset, arsitektur, _overfitting_, dsb).
---
### **BAB V — Kesimpulan dan Saran**
#### 5.1 Kesimpulan
- CNN dapat digunakan untuk mengidentifikasi jenis patah tulang dari citra rontgen.
- Model memberikan tingkat akurasi tertentu (tulis hasil jika sudah diuji).
#### 5.2 Saran
- Perlu penambahan variasi dataset dan pengujian dengan model CNN lain (misalnya VGG16, ResNet).
- Dapat dikembangkan ke sistem deteksi otomatis berbasis web atau aplikasi klinis.