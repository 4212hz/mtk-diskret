---
title: Probabilitas

---

# Probabilitas

Probabilitas adalah metrik untuk menentukan kemungkinan terjadinya suatu peristiwa. Banyak hal yang tidak mungkin diprediksi dengan kepastian 100%. Dengan menggunakannya, Anda hanya dapat memprediksi probabilitas terjadinya suatu peristiwa, yaitu seberapa besar kemungkinan terjadinya. Dalam tutorial ini, Anda akan mempelajari Teorema Bayes, subtopik penting dalam teori probabilitas.

## Probabilitas Bersyarat
Misalkan A dan B adalah dua kejadian yang terkait dengan suatu eksperimen acak. Maka, probabilitas terjadinya A dengan syarat B telah terjadi dan P(B) ≠ 0 disebut Probabilitas Bersyarat. Probabilitas ini dilambangkan dengan P (A/B). Jadi, Anda memperoleh:

$P(A \mid B) = \frac{P(A \cap B)}{P(B)}$

## Perhitungan Probabilitas 
Sekarang kita kembali ke permasalahan kita: diberikan sampel fitur baru ( X₁, X₂ ), kita ingin memprediksi target B. Jika kita tetap menggunakan contoh dimana Suhu = sedang ( X₁ = M ) dan Angin = lemah ( X₂ = W ), kita harus menghitung
$P(B = T \mid X_1 = M, X_2 = W) = \frac{P(X_1 = M \mid B = T) \cdot P(X_2 = W \mid B = T) \cdot P(B = T)}{P(X_1 = M) \cdot P(X_2 = W)}$
Dan 
$P(B = F \mid X_1 = M, X_2 = W) = \frac{P(X_1 = M \mid B = F) \cdot P(X_2 = W \mid B = F) \cdot P(B = F)}{P(X_1 = M) \cdot P(X_2 = W)}$
untuk mencari yang terbesar dari keduanya. Baiklah, mari kita hitung berdasarkan bagiannya.

## Probabilitas Prediksi
Langkah lain yang diambil oleh model Naive Bayes adalah menghitung probabilitas relatif untuk kedua keputusan benar dan salah . Hal ini dilakukan karena probabilitas posterior tidak berjumlah sama dengan unit ( 0,63 > 0,42 = 1,05 ≠ 1 atau, jika Anda ingin lebih tepat, 5/12 + 5/8 = 25/24 ≠ 1 ).

Kita dapat mendefinisikan PT sebagai probabilitas untuk memprediksi benar dan PF sebagai probabilitas untuk memprediksi salah sebagai berikut:
$P(T) = \frac{P(B = T, X_1, X_2)}{P(B = T, X_1, X_2) + P(B = F, X_1, X_2)}$
Dan
$P(F) = \frac{P(B = F, X_1, X_2)}{P(B = F, X_1, X_2) + P(B = T \mid X_1, X_2)}$
Perhatikan bahwa kami menghilangkan nilai aktual untuk X₁ dan X₂ demi kesederhanaan. Selain itu, sekarang kami dapat memastikan bahwa PT + PF = 1 .

Keuntungan utama menggunakan probabilitas (yang jumlahnya sama dengan satuan) adalah jika kita menemukan probabilitas pertama lebih besar dari 0,5, kita dapat membuat keputusan tanpa menghitung probabilitas kedua. Atau, jika kita berhadapan dengan lebih dari dua kelas untuk variabel target kita, segera setelah kita menemukan satu probabilitas yang lebih besar dari 0,5, itu sudah menjadi jawaban kita.

Dengan memasukkan probabilitas posterior yang telah kita hitung, kita memperoleh

$P_{T} = \frac{\frac{5}{12}}{\frac{5}{12} + \frac{5}{8}} = \frac{2}{5} = 0.4$

$P_{F} = \frac{\frac{5}{8}}{\frac{5}{12} + \frac{5}{8}} = \frac{3}{5} = 0.6$

dan, sekali lagi, kita akan memilih B = F. Namun begitu kita menghitung probabilitas prediksi pertama, PT = 0.4 , karena PT < 0.5 , kita akan secara otomatis memprediksi kelas lainnya (selain T ); yaitu, F — yang, sekali lagi, berarti kita tidak boleh pergi ke pantai .
# Teorema Bayes

Teorema Bayes adalah rumus matematika untuk menghitung probabilitas bersyarat dalam probabilitas dan statistik. Dengan kata lain, rumus ini digunakan untuk mencari tahu seberapa besar kemungkinan suatu peristiwa berdasarkan kedekatannya dengan peristiwa lain. Hukum Bayes atau aturan Bayes adalah nama lain untuk teorema ini.

## Rumus Teorema Bayes
Rumus untuk teorema Bayes dapat ditulis dalam berbagai cara. Berikut ini adalah versi yang paling umum:

$P(A \mid B) = \frac{P(B \mid A).P(A)}{P(B)}$

- P(A ∣ B) merupakan probabilitas bersyarat terjadinya peristiwa A, jika B benar.
- P(B ∣ A) adalah probabilitas bersyarat terjadinya peristiwa B, jika A benar.
- P(A) dan P(B) merupakan probabilitas terjadinya A dan B secara independen satu sama lain.

Jika kita mengganti nama beberapa hal, kita dapat menggunakan Teorema Bayes dalam masalah kita. Karena kejadian kita didasarkan pada variabel target Pantai ( B ), mari kita ganti Kejadian E dengan Pantai B . Selain itu, kondisi kita (kita punya dua) diberikan oleh dua fitur, bernama Temperatur ( X₁ ) dan Angin ( X₂ ), jadi mari kita ganti Kondisi C dengan fitur X₁, X₂ . Perlu diingat bahwa karena kita punya dua fitur dalam masalah ini, kita akan menggunakan semacam probabilitas gabungan . Semua modifikasi ini menghasilkan persamaan berikut:
$P(B \mid X_1, X_2) = \frac{P(X_1, X_2 \mid B) \cdot P(B)}{P(X_1, X_2)}$
Jika membantu, Anda dapat menambahkan langkah ekstra di sini dan secara mental menyebut X = X₁, X₂ , sehingga persamaan menjadi lebih mudah dipahami,
$P(B \mid X) = \frac{P(X \cap B) \cdot P(B)}{P(X)}$
dan Anda selalu dapat mengganti X dengan X₁, X₂.
## Contoh Teorema Bayes

Soal 1: 
Tiga guci berisi 6 bola merah, 4 bola hitam; 4 bola merah, 6 bola hitam, dan 5 bola merah, 5 bola hitam. Salah satu guci dipilih secara acak dan sebuah bola diambil dari guci tersebut. Jika bola yang diambil berwarna merah, carilah peluang bahwa bola tersebut diambil dari guci pertama.

Solusi: Misalkan E1, E2, E3, dan A adalah peristiwa-peristiwa yang didefinisikan sebagai berikut:

E1 = guci pertama dipilih 
E2 = guci kedua dipilih
E3 = guci ketiga dipilih 
A = bola yang ditarik berwarna merah
Karena ada tiga guci dan salah satu dari ketiga guci tersebut dipilih secara acak, maka:
Diketahui P(E1) = P(E2) = P(E3) = ⅓
Jika E1 telah terjadi, maka guci pertama telah dipilih, yang berisi 6 bola merah dan 4 bola hitam. Peluang terambilnya bola merah dari guci tersebut adalah 6/10.
Jadi, P(A/E1) = 6/10
Demikian pula, Anda memiliki P(A/E2) = 4/10 dan P(A/E3) = 5/10

Anda diminta untuk menemukan P(E1/A), yaitu jika bola yang terambil berwarna merah, berapakah peluang bahwa bola tersebut terambil dari guci pertama?
Jawaban: 
$P(E_1 \mid A) = \frac{P(E_1) \cdot P(A \mid E_1)}{P(E_1) \cdot P(A \mid E_1) + P(E_2) \cdot P(A \mid E_2) + P(E_3) \cdot P(A \mid E_3)}$
$= \frac{\frac{1}{3} \cdot \frac{6}{10}}{\left(\frac{1}{3} \cdot \frac{6}{10}\right) + \left(\frac{1}{3} \cdot \frac{4}{10}\right) + \left(\frac{1}{3} \cdot \frac{5}{10}\right)}$
$= \frac{2}{5}$


Soal 2:
Sebuah perusahaan memiliki dua pabrik yang menghasilkan produk dengan tingkat kerusakan yang berbeda. Pabrik A menghasilkan 60% dari total produk dan memiliki probabilitas kerusakan produk sebesar 2%. Pabrik B menghasilkan 40% dari total produk dan memiliki probabilitas kerusakan produk sebesar 5%. Jika sebuah produk yang diambil secara acak ternyata rusak, berapa probabilitas bahwa produk tersebut berasal dari Pabrik A?
Jawaban:
$P(R) = (0.02 - 0.60) + (0.05 - 0.40) = 0.032$
$P(A \mid R) = \frac{0.02 - 0.60}{0.032} = 0.375$

Soal 3:
Sebuah laboratorium memiliki 3 mesin, yaitu Mesin A, Mesin B, dan Mesin C, yang memproduksi barang. Proporsi produksi dan probabilitas barang cacat dari masing-masing mesin adalah sebagai berikut:
- Mesin A menghasilkan 50% dari total produksi, dan 2% dari barangnya cacat.
- Mesin B menghasilkan 30% dari total produksi, dan 5% dari barangnya cacat.
- Mesin C menghasilkan 20% dari total produksi, dan 10% dari barangnya cacat.
Jika sebuah barang dipilih secara acak dan diketahui cacat, berapa probabilitas barang tersebut berasal dari Mesin C?
Jawaban:
$P(\text{Cacat}) = P(\text{Cacat} \mid A) \cdot P(A) + P(\text{Cacat} \mid B) \cdot P(B) + P(\text{Cacat} \mid C) \cdot P(C)$ $P(\text{Cacat}) = (0.02 \cdot 0.5) + (0.05 \cdot 0.3) + (0.1 \cdot 0.2)$
$P(\text{Cacat}) = 0.01 + 0.015 + 0.02 = 0.045$