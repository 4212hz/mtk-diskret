---
title: logika dan pembuktian Mohammad Aziz Huzaini 240411100079

---

# Logika Matematika

## Nagasi
**Pengertian**: 
Negasi adalah penyangkalan, peniadaan, atau kata sangkalan terhadap sesuatu. Dalam bahasa Indonesia, negasi dapat diartikan sebagai pengingkaran atau penambahan kata ingkar atau pemarkah negatif pada sebuah kalimat.Berdasarkan Kamus Besar Bahasa Indonesia (KBBI), negasi adalah penyangkalan, peniadaan, atau kata sangkalan seperti kata 'tidak' dan 'bukan'. Istilah negasi digunakan dalam sejumlah bidang, antara lain bahasa dan matematika.Dilansir dari buku Logika Matematika (2021) karya Retno Damayanti, negasi dalam logika matematika juga disebut ingkaran. Penggunaan dalam logika matematika tidak berbeda jauh dengan penggunaannya di ilmu bahasa.

Negasi dalam logika matematika biasa disimbolkan dengan (~). Misalnya pernyataan p negasinya adalah ~p. Sedangkan pada kalimat pernyataan, negasi biasa menggunakan kata tidak, bukan, atau tidak benar.

| T | F | 
|  -| - | 
| T | F |
| F | T |

 dalam bentuk tabel kebenaran:

$$
\begin{array}{|c|c|}
\hline
P & \neg P \\
\hline
\text{benar} & \text{salah} \\
\text{salah} & \text{benar} \\
\hline
\end{array}
$$


## Konjungsi
**Pengertian**: 
Konjungsi adalah operasi logika yang menghubungkan dua pernyataan, menghasilkan nilai benar hanya jika kedua pernyataan tersebut benar. Dalam notasi logika, konjungsi dinyatakan dengan simbol $∧$.

**Contoh**:
- Pernyataan 1: "Hujan turun."
- Pernyataan 2: "Bumi basah."

Konjungsi dari kedua pernyataan tersebut adalah:  
"Hujan turun dan Bumi basah."  
Ditulis sebagai:
$P∧Q$
di mana $P$ dan $𝑄$ masing-masing adalah pernyataan 1 dan 2. Konjungsi ini benar hanya jika kedua pernyataan tersebut benar.
![Capture9](https://hackmd.io/_uploads/S1L3JwFyke.png)


## Disjungsi
Disjungsi adalah operasi logika yang menghubungkan dua pernyataan, menghasilkan nilai benar jika salah satu atau kedua pernyataan tersebut benar. Simbol yang digunakan untuk disjungsi adalah v

Contoh:

Pernyataan 1: "Hari ini cerah."
Pernyataan 2: "Saya akan pergi ke taman."
Disjungsi dari kedua pernyataan tersebut adalah:
"Hari ini cerah atau saya akan pergi ke taman."
Ditulis sebagai:
P∨Q
Disjungsi ini benar jika salah satu atau kedua pernyataan 𝑃 dan Q benar.
![Capture12](https://hackmd.io/_uploads/HycgZwtJJg.png)



## Implikasi 
**Pengertian**: Implikasi adalah hubungan logika antara dua pernyataan, di mana pernyataan pertama (antecedent) mengimplikasikan pernyataan kedua (consequent). Implikasi dinyatakan dengan simbol \( \rightarrow \) dan berarti "jika... maka..."

**Contoh**:
- Pernyataan 1: "Jika hujan, maka tanah akan basah."

Ditulis sebagai:
$P$ → $Q$
di mana $P$ adalah "hujan" dan $Q$ adalah "tanah akan basah." Implikasi ini benar kecuali jika $P$ benar dan $Q$ salah.
![Capture10](https://hackmd.io/_uploads/BJ0lxDF1Jx.png)


## Biimplikasi
Biimplikasi adalah hubungan logika antara dua pernyataan yang menunjukkan bahwa kedua pernyataan tersebut saling mengimplikasikan satu sama lain. Ini berarti bahwa jika satu pernyataan benar, maka pernyataan lainnya juga harus benar, dan sebaliknya. Biimplikasi dinyatakan dengan simbol ↔ dan berarti "jika dan hanya jika..."

Contoh:
Pernyataan 1: "Sebuah angka genap."
Pernyataan 2: "Angka tersebut dapat dibagi 2."
Biimplikasi dari kedua pernyataan tersebut adalah:
"Sebuah angka adalah genap jika dan hanya jika angka tersebut dapat dibagi 2."
Ditulis sebagai:
P↔Q
di mana $P$ adalah "angka genap" dan $𝑄$ adalah "angka dapat dibagi 2." Biimplikasi ini benar jika kedua pernyataan $𝑃$ dan $Q$ memiliki nilai kebenaran yang sama.
![Capture11](https://hackmd.io/_uploads/Hy4ulwYJyx.png)



---
**Latihan Soal**:
Buatlah tabel kebenaran untuk~pernyataan berikut $$P\lor(R\to\ Q)$$

$$\begin{array}{c|c|c|c|cc}P&Q&R&\ Q&R\to\ Q&P\lor(R\to\ Q)\\\hline\text{Т}&\text{Т}&\text{Т}&\text{T}&\text{T}&\text{T}\\\text{Т}&\text{Т}&\text{F}&\text{T}&\text{T}&\text{T}\\\text{T}&\text{F}&\text{T}&\text{F}&\text{F}&\text{T}\\\text{T}&\text{F}&\text{F}&\text{F}&\text{T}&\text{T}\\\text{F}&\text{T}&\text{T}&\text{T}&\text{T}&\text{T}\\\text{F}&\text{T}&\text{F}&\text{T}&\text{T}&\text{T}\\\text{F}&\text{F}&\text{T}&\text{F}&\text{F}&\text{F}\\\text{F}&\text{F}&\text{F}&\text{F}&\text{T}&\text{T}&\end{array}$$