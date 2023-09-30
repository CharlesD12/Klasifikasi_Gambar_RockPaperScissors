# Klasifikasi_Gambar_RockPaperScissors

Kode tersebut merupakan model machine learning sederhana untuk mengidentifikasi gambar rock paper scissors. Model ini menggunakan jaringan saraf tiruan (neural network) dengan arsitektur Sequential. Arsitektur ini terdiri dari dua lapisan Dense. Lapisan pertama memiliki 16 neuron dengan aktivasi relu. Lapisan kedua memiliki 3 neuron dengan aktivasi softmax.

Penjelasan Kode :

Mengimport library yang dibutuhkan
Kode ini pertama-tama mengimport library yang dibutuhkan, yaitu:

* **zipfile** untuk mengekstrak file zip
* **os** untuk membuat direktori baru
* **PIL** untuk mengolah gambar ke array
* **numpy** untuk mengubah ke array
* **tensorflow** untuk machine learning
* **IPython.display** untuk menampilkan gambar yang akan diidentifikasi
Membuat direktori baru dan mendefinisikannya
Kode ini kemudian membuat direktori baru bernama dataset. Direktori ini akan digunakan untuk menyimpan data gambar rock paper scissors.

Melakukan ekstrak pada dataset
Kode ini mengekstrak file zip yang berisi data gambar rock paper scissors. File zip tersebut bernama rock-paper-scissors.zip.

Mendefinisikan folder rock-paper-scissors
Kode ini mendefinisikan folder rock, paper, dan scissors untuk memudahkan dalam pemanggilan.

Melihat attribute yang ada dalam folder rock-paper-scissors
Kode ini menampilkan nama-nama file yang ada di dalam folder rock, paper, dan scissors.

Mendefinisikan fungsi
Kode ini mendefinisikan fungsi imgToArray() untuk mengubah gambar menjadi array. Fungsi ini menggunakan library PIL untuk mengubah gambar menjadi grayscale dan resize menjadi ukuran 150x150.

Melakukan proses one hot encoding pada folder rock-paper-scissors
Kode ini melakukan proses one hot encoding pada data gambar. One hot encoding adalah proses mengubah label menjadi array dengan panjang yang sama dengan jumlah label. Dalam kasus ini, jumlah label adalah 3, yaitu rock, paper, dan scissors.

Melakukan pemanggilan dan pengujian pada folder dan gambar
Kode ini mencoba menampilkan nama gambar dari folder rock pada index 0 dan hasil pengindexan dari salah satu gambar.

Melatih model jaringan saraf tiruan
Kode ini melatih model jaringan saraf tiruan dengan data gambar yang telah diolah. Model ini dilatih selama 20 epoch.

Melakukan pegujian pada gambar yang akan diprediksi
Kode ini melakukan pengujian pada gambar yang akan diprediksi. Gambar yang akan diprediksi disimpan dalam file bernama test.jpg.


Penjelasan pengujian:

Kode ini pertama-tama mengubah gambar test.jpg menjadi array. Kemudian, model jaringan saraf tiruan digunakan untuk memprediksi hasil gambar. Hasil prediksi disimpan dalam variabel hasil.


Penjelasan hasil prediksi:

Indeks nilai tertinggi dalam variabel hasil menunjukkan label yang paling mungkin untuk gambar tersebut. Nilai indeks tersebut kemudian digunakan untuk menentukan hasil prediksi.


Kesimpulan

Kode ini merupakan model machine learning sederhana untuk mengidentifikasi gambar rock paper scissors. Model ini menggunakan jaringan saraf tiruan dengan arsitektur Sequential. Model ini dapat dilatih dengan data gambar rock paper scissors yang lebih banyak untuk meningkatkan akurasi prediksi.
