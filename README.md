# KLASIFIKASI RENTANG KELAS HARGA TELEPON GENGGAM BERDASARKAN SPESIFIKASINYA
Intro to Machine Learning Project Pacmann - AI/ML Engineering

---

## INTRODUCTION

Dalam era digital seperti sekarang ini, telepon genggam atau Handphone telah menjadi salah satu kebutuhan penting bagi masyarakat. Dengan banyaknya merek dan jenis handphone yang tersedia di pasaran, klasifikasi harga berdasarkan spesifikasi handphone menjadi permasalahan yang seringkali sulit untuk diatasi secara manual.

Permasalahan klasifikasi harga handphone berdasarkan spesifikasi handphone merupakan masalah yang sering ditemukan di dalam industri penjualan handphone. Hal ini dapat membuat penjual bingung dalam menentukan harga yang pantas untuk setiap produk, sementara bagi pembeli, mereka juga bisa terjebak membeli harga yang terlalu mahal untuk sebuah produk handphone. Oleh karena itu, penting untuk menyelesaikan permasalahan ini dengan menggunakan pemrograman machine learning.


## RELATED WORK

R. H. Ali and W. B. Abdulkareem dengan judul paper: “A Comparative Study of Machine Learning Algorithms for Mobile Phone Price Classification”, International Journal of Advanced Computer Science and Applications, vol. 8, no. 3, pp. 226–232, 2017.


## DATASET
Dataset yang digunakan pada final project ini ada 2 file yaitu file train.csv berisi dataset yang memiliki kolom label, 1500 baris, dan 22 kolom yang digunakan untuk training model dan file test.csv yang berisi dataset tanpa kolom label, 500 baris, dan 22 kolom yang digunakan untuk data testing.

Untuk keterangan spesifikasi handphone pada kolom label sebagai berikut :
- index = nomor id yang bersifat unik bernilai integer positif
- daya_baterai = total energi yang disimpan dalam baterai (satuan mAh)
- bluetooth = memiliki fitur Bluetooth atau tidak (1 untuk ya & 0 untuk tidak)
- kecepatan_clock = kecepatan prosesor melaksanakan instruksi
- dual_sim = memiliki kapabilitas penggunaan dual sim (1 untuk ya & 0 untuk tidak)
- kamera_depan = besar resolusi penggunaan kamera depan (satuan MegaPixels)
- four_g = memiliki kapabilitas konektivitas 4G (1 untuk ya & 0 untuk tidak)
- memori_internal = Besar memori internal (satuan GB)
- tebal_hp = tebal handphone (satuan cm)
- berat_hp = massa handphone (satuan gram)
- jumlah_prosesor = jumlah core dalam prosesor (satuan buah)
- kamera_belakang_mp = besar resolusi penggunaan kamera belakang (satuan MegaPixels)
- px_panjang = panjang resolusi piksel
- px_lebar = lebar resolusi piksel
- kapasitas_ram = kapasitas Random Access Memory (satuan MB)
- panjang_layar = panjang layar (satuan cm)
- lebar_layar = lebar layar (satuan cm)
- waktu_telepon = waktu telfon terlama yang bisa dilakukan dari HP tercas penuh hingga habis (satuan jam)
- three_g = memiliki kapabilitas konektivitas 3G (1 untuk ya & 0 untuk tidak)
- touch_screen = memiliki layar sentuh (1 untuk ya & 0 untuk tidak)
- wifi = memiliki fitur wifi (1 untuk ya & 0 untuk tidak)
- price_range = rentang harga kisaran HP (0–3000)


Selain itu untuk data output yaitu dataset baru data hasil prediksi tersimpan dalam file hasil_prediksi_terbaik.csv yang berisi 500 baris dan 2 kolom dengan kolom label yaitu index dan price_range saja

## ALGORITMA KLASIFIKASI
1. Random Forest
2. K-Nearest Neighbors
3. Naive Bayes

## RESULT
![perbandingan_barchart](https://user-images.githubusercontent.com/101574764/232260321-a497882f-1041-4d2d-8b84-218e8cead59c.png)


Conclusion :

Bahwa file baru hasil prediksi (hasil_prediksi_terbaik.csv) berisi 500 baris dan 2 kolom yaitu kolom label “index” dan kolom label “price_range” dengan menggunakan algoritma Naive Bayes yang menghasilkan nilai fmean score / f1 score paling tinggi yaitu pada angka 97%.

Future works :

Dapat dilakukan percobaan dengan menggunakan model atau algoritma lainnya yang memiliki metode optimasi sehingga performa model lebih akurat dan lebih cepat.
