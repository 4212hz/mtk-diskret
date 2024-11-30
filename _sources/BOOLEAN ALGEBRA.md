---
title: BOOLEAN ALGEBRA

---

# ALJABAR BOOLEAN DAN GERBANG LOGIKA
## Aljabar Boolean
Aljabar Boolean adalah cabang matematika yang digunakan untuk menganalisis dan merancang sistem logika. Konsep dasar dari aljabar Boolean melibatkan variabel yang hanya dapat memiliki dua nilai: benar (1) dan salah (0). Terdapat tiga operasi dasar dalam aljabar Boolean:

AND (∧): Hasilnya benar jika kedua operandnya benar.
Contoh: A ∧ B = 1 hanya jika A = 1 dan B = 1.

OR (∨): Hasilnya benar jika salah satu atau kedua operandnya benar.
Contoh: A ∨ B = 1 jika A = 1 atau B = 1 (atau keduanya).

NOT (¬): Mengubah nilai operand menjadi kebalikannya.
Contoh: ¬A = 1 jika A = 0. 
![Capture8](https://hackmd.io/_uploads/B1tRpUFk1g.png)


## Hukum-Hukum Aljabar Boolean
Hukum Idempotensi: A ∨ A = A dan A ∧ A = A
Hukum Dominas: A ∨ 1 = 1 dan A ∧ 0 = 0
Hukum Negasi: A ∨ ¬A = 1 dan A ∧ ¬A = 0

## Gerbang Logika
Gerbang logika adalah rangkaian elektronika yang merepresentasikan operasi aljabar Boolean. Gerbang logika dasar terdiri dari:

Gerbang AND: Menghasilkan output 1 jika semua inputnya 1.
Gerbang OR: Menghasilkan output 1 jika setidaknya satu inputnya 1.
Gerbang NOT: Menghasilkan output yang merupakan invers dari input.
### Contoh Implementasi Gerbang Logika

Gerbang AND:
Jika A = 1 dan B = 1, maka output = 1.
Jika A = 1 dan B = 0, maka output = 0.

Gerbang OR:
Jika A = 1 dan B = 0, maka output = 1.
Jika A = 0 dan B = 0, maka output = 0.

Gerbang NOT:
Jika A = 1, maka output = 0.
Jika A = 0, maka output = 1.

## Kesimpulan
Aljabar Boolean dan gerbang logika adalah alat penting dalam desain sirkuit digital dan sistem komputer. Dengan memahami konsep-konsep dasar ini, kita dapat merancang dan menganalisis berbagai sistem logika yang kompleks.