Analisis Perbandingan Performa Deep Learning (ANN) terhadap Random Forest dalam Memprediksi Niat Pembelian Pengunjung E-Commerce

Ringkasan Proyek
Proyek ini mengeksplorasi penggunaan algoritma Machine Learning dan Deep Learning untuk memprediksi perilaku konsumen di platform e-commerce. Menggunakan Online Shoppers Purchasing Intention Dataset, kami membandingkan efektivitas model Random Forest sebagai metode ensemble tradisional dengan Artificial Neural Network (ANN) yang menggunakan arsitektur multilayer.

👥 Anggota Kelompok (Kelompok 10)
Program Studi Teknik Informatika - STMIK Tazkia

Shanaya Balghis Riyona (241552010012) - shnvablqsr@gmail.com

Thoriqurrahman Akrami (241552010013) - thoriqurrahmana@gmail.com

Dosen Pengampu: Bapak Hendri Kharisma, S.Kom., M.T.

Metodologi dan Eksperimen
1. Dataset
Sumber: UCI Machine Learning Repository.

Jumlah Data: 12.330 sesi kunjungan.

Fitur Utama: Administrative, Informational, ProductRelated, BounceRates, ExitRates, PageValues, dan SpecialDay.

Target: Revenue (Klasifikasi biner: Membeli atau Tidak).

2. Pra-pemrosesan Data
Encoding: Mengonversi data kategorikal menggunakan OrdinalEncoder.

Scaling: Normalisasi fitur numerik dengan StandardScaler untuk mengoptimalkan konvergensi pada model ANN.

Splitting: Membagi data menjadi porsi training dan testing untuk validasi model.

3. Arsitektur Model
Random Forest: Digunakan sebagai baseline dengan pencarian parameter optimal.

Artificial Neural Network (ANN):

Input Layer: Sesuai jumlah fitur input.

Hidden Layers: 2 layer padat (Dense) dengan fungsi aktivasi ReLU.

Regularization: Menggunakan Dropout layer untuk mencegah overfitting.

Output Layer: 1 unit dengan fungsi aktivasi Sigmoid.

Optimizer: Adam Optimizer (Kingma & Ba, 2014).

Hasil dan Kesimpulan
Berdasarkan hasil pengujian pada UAS_Code.ipynb:

Random Forest: Menunjukkan stabilitas tinggi dengan akurasi rata-rata sebesar 90.23%.

ANN: Memberikan performa kompetitif (Akurasi ~90.35%) dan mampu memetakan pola perilaku yang lebih kompleks melalui representasi saraf tiruan.

Insights: Fitur PageValues ditemukan sebagai prediktor paling signifikan dalam menentukan niat beli konsumen.