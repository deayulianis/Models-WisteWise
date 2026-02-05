#🗑️ Waste Classification Using MobileNetV2
## Project Captone Coding Camp 2025

Proyek ini bertujuan untuk membangun model klasifikasi jenis sampah berbasis citra menggunakan Deep Learning dengan arsitektur MobileNetV2. Model dirancang untuk mengidentifikasi jenis sampah dari gambar, kemudian mengelompokkannya ke dalam tiga kategori utama, yaitu Organik, Anorganik, dan B3 (Bahan Berbahaya dan Beracun).

### 📂 Kategori Sampah

Model melakukan klasifikasi dalam dua tingkat:

1) Klasifikasi jenis sampah spesifik
Model mengenali berbagai jenis sampah seperti sisa makanan, plastik, kertas, kaca, logam, baterai, limbah medis, dan limbah elektronik.

2) Pengelompokan ke kategori utama
Hasil prediksi jenis sampah kemudian dikelompokkan ke dalam kategori:

- Organik: sampah yang berasal dari sisa makhluk hidup dan mudah terurai

- Anorganik: sampah non-hayati seperti plastik, kertas, kaca, dan logam

- B3: sampah berbahaya dan beracun seperti baterai, limbah kimia, obat-obatan, dan elektronik

Pendekatan ini memudahkan proses klasifikasi sekaligus mendukung sistem pengelolaan sampah berbasis kategori.

### 🔄 Alur Pengembangan Model

Pengembangan model dilakukan melalui beberapa tahapan utama sebagai berikut:

1) Data Preparation
Dataset citra disiapkan dan disesuaikan strukturnya berdasarkan kelas sampah yang akan dikenali oleh model.

2) Data Preprocessing
Setiap gambar melalui proses penyesuaian ukuran, normalisasi nilai piksel, serta augmentasi data untuk meningkatkan kemampuan generalisasi model.

3) Split Dataset
Data dibagi menjadi data latih (training) dan data validasi (validation) untuk mengevaluasi performa model secara objektif.

4) Modeling
Model dibangun menggunakan arsitektur MobileNetV2 sebagai base model yang telah dilatih sebelumnya (pretrained), kemudian ditambahkan lapisan klasifikasi untuk menyesuaikan dengan jumlah kelas pada dataset.

5) Pengelompokan Kategori
Output prediksi dari model digunakan untuk menentukan kategori utama sampah, yaitu Organik, Anorganik, atau B3, sehingga hasil akhir lebih mudah diinterpretasikan.

6) Evaluasi dan Visualisasi
Performa model dievaluasi menggunakan metrik akurasi serta divisualisasikan dalam bentuk grafik akurasi dan loss selama proses pelatihan.

7) Penyimpanan Model
Model yang telah dilatih disimpan dengan format tflite dan dapat digunakan untuk pengembangan website atau aplikasi lebih lanjut.

### 🧠 Arsitektur Model

Model menggunakan MobileNetV2, yaitu arsitektur Convolutional Neural Network yang ringan dan efisien, sehingga cocok untuk aplikasi klasifikasi citra dengan kebutuhan komputasi yang relatif rendah. Lapisan tambahan digunakan untuk menyesuaikan model dengan tugas klasifikasi jenis sampah.

### 📊 Hasil Evaluasi

- Akurasi Training: 100.00%

- Akurasi Validation: 87.68%

Hasil evaluasi menunjukkan bahwa model mampu mengenali pola citra sampah dengan baik. Perbedaan antara akurasi training dan validation mengindikasikan potensi overfitting, sehingga pada pengembangan selanjutnya dapat diterapkan teknik seperti regularisasi atau penambahan data.

### 🚀 Kesimpulan

Model klasifikasi sampah berbasis citra menggunakan MobileNetV2 berhasil mengelompokkan sampah ke dalam kategori Organik, Anorganik, dan B3 dengan performa yang cukup baik. Model ini dapat menjadi dasar pengembangan sistem smart waste classification untuk mendukung pengelolaan sampah yang lebih efektif dan berkelanjutan.
