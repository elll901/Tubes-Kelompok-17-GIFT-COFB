# Tubes-Kelompok-17-GIFT-COFB
Tugas Besar EL2002 - Sistem Digital
Dibuat oleh Kelompok 17 Elektro'21 ITB
Disusun Oleh
					13221054  M Bharata Sri Prana Ludira H
					13221056  Adriel Tohonan Simamora
					13221065  Caitleen Devina
					13221067  Muhammad Luthfi
					13221088  Nico Oktavianto Aritonang

GIFT-COFB adalah block cipher (sandi) yang berbasis AEAD (Authenticated Encryption with Associated Data) yang menggunakan GIFT-128 sebagai mode pengoperasiannya. AEAD adalah metode pengenkripsian data secara autentik (asli) yang menggunakan associated data (data yang ikut bersamaan dengan input) melalui kombinasi itu akan didapat data yang dapat dirahasiakan dengan baik dan juga autentik. Dengan penggunaan GIFT-128, maka GIFT-COFB ini dapat memproses hingga 128 bit informasi yang masuk. Jumlah bit yang bisa diubah sesuai dengan keinginan input. 
GIFT-COFB memiliki dua proses yaitu proses enkripsi dan proses dekripsi. Saat melakukan proses enkripsi sebuah message (M), akan diterima 3 input dan dihasilkan 2 output yaitu sebagai berikut.
Input:
Encryption key (K) : kunci yang digunakan untuk enkripsi plain text yang jadi masukan.
Nonce (N) : angka yang digunakan sebagai input awal enkripsi dan hanya digunakan sekali. Nonce merupakan kepanjangan dari Number Only Used Once.
Associated data and message (A, M) : associated data adalah data yang mengikuti message yang masuk dan berisi informasi mengenai message yang ada, sedangkan message merupakan text yang akan dienkripsi.

Output:
Ciphertext (C) : hasil yang telah dienkripsi.
Tag (T) : sebagai penentu enkripsi yang digunakan menggunakan proses apa.
Sedangkan untuk melakukan proses dekripsi sebuah ciphertext (C) dan tag (T), akan diterima 3 input dan dihasilkan sebuah output yaitu sebagai berikut.
Input:
Encryption key (K) : kunci yang digunakan untuk enkripsi plain text yang jadi masukan.
Nonce (N) : angka yang digunakan sebagai input awal enkripsi dan hanya digunakan sekali. Nonce merupakan kepanjangan dari Number Only Used Once.
Associated data and ciphertext (A, C) : associated data adalah data yang mengikuti message yang masuk dan berisi informasi mengenai message yang ada, sedangkan ciphertext merupakan hasil text yang telah dienkripsi.
Output:
Message (M) : message merupakan text hasil dekripsi yang berisi pesan yang masuk akal.
GIFT-128 adalah sebuah blok yang digunakan untuk mengubah arahan tiap masukan yang ada. COFB berfokus pada implementasi GIFT pada hardware yang akan digunakan. Kombinasi penggunaan GIFT COFB akan membuat ukuran state yang lebih sedikit, dapat dilihat lebih lengkap di bagian analisis konsep sistem.


