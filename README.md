# RTC_Kelompok-8 - PEMANTAUAN KUALITAS AIR BERBASIS PEMBELAJARAN MACHINE LEARNING UNTUK DETEKSI DINI KONTAMINASI 
Supervisor : Ahmad Radhy, S.Si., M.Si

Nama Kelompok : 
1. Mukhamad Da'ul Azimi - 2042221071
2. Muhammad Rafi Zidan Hilmi - 2042221125
3. Febrianaufal Izzan Arifin - 2042221140

**Water Quality Project with Rust and Qt**
Proyek ini merupakan kumpulan modul berbasis Rust yang dirancang untuk melakukan klasifikasi kualitas air menggunakan tiga algoritma utama: Neural Network, Support Vector Machine (SVM), dan k-Nearest Neighbor (kNN). Beberapa modul juga terintegrasi dengan Qt untuk menyediakan antarmuka pengguna yang interaktif dan mudah digunakan.

**Struktur Proyek**
•	lookup/
Modul sederhana untuk konversi nilai menggunakan tabel pemetaan.
•	neural_network/
Implementasi Neural Network dengan integrasi GUI Qt. Modul ini mencakup pelatihan model, penyimpanan model (model.bin), serta prediksi kualitas air.
•	svm-knn/
Modul klasifikasi kualitas air menggunakan algoritma SVM dan kNN. Hasil prediksi divisualisasikan dalam format gambar .png.
•	sin-cos/
Proyek pendukung untuk perhitungan nilai sudut sinus dan cosinus menggunakan metode Deret Taylor.

**Panduan untuk mencoba**
Setiap modul dapat dijalankan di lingkungan Ubuntu dengan Visual Studio Code dan Rust terpasang. Berikut garis besar langkah instalasi dan penggunaan:

**Deret Taylor**
1.	Download dan ekstrak file zip sin-cos.
2.	Buka folder di VS Code (code .).
3.	Jalankan perintah cargo build dan cargo run di terminal VS Code.
4.	Modul ini menghitung sinus dan cosinus menggunakan fungsi faktorial dan deret Taylor.
   
**LookupTable**
1.	Download dan ekstrak file zip lookup.
2.	Ikuti langkah serupa seperti modul Deret Taylor.
3.	Modul ini mengimplementasikan pemetaan tabel dan perhitungan sinus-cosinus.
   
**SVM & kNN**
1.	Download dan ekstrak file zip svm-knn.
2.	Pasang library Rust yang dibutuhkan seperti csv, linfa, linfa-svm, linfa-nn, linfa-kernel, linfa-logistic, ndarray, rand, dan plotters.
3.	Jalankan cargo build dan cargo run.
4.	Modul ini memuat data, menjalankan algoritma kNN dan SVM, serta menghitung akurasi klasifikasi kualitas air.
   
**Neural Network dengan Frontend Qt**
1.	Download dan ekstrak file zip neural_network.
2.	Pasang library rand, plotters, csv, plotters, image, rfd dan egui.
3.	Struktur folder berisi main.rs, dan frontend.rs.
4.	Jalankan cargo build --release dan cargo run.
5.	Modul ini menggabungkan neural network dengan tampilan GUI berbasis Qt.
