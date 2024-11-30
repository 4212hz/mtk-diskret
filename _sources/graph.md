---
title: graph

---

# graph

## Pengertian Graph
Graf digunakan untuk merepresentasikan objek-objek diskrit dan hubungan antara objek-objek tersebut, sehingga secara sederhana graf didefinisikan sebagai kumpulan titik yang dihubungkan oleh garis-garis/sisi.
Sedangkan definisi matematis untuk graf adalah, pasangan terurut himpunan (V,E), dimana V merupakan himpunan beranggotakan titik-titik (vertex) dan E merupakan himpunan beranggotakan sisi-sisi (edges).
Perhatikan Contoh Graf (V,E) berikut:
    ![Capture22](https://hackmd.io/_uploads/BkUDg42fyg.png)
V:={1,2,3,4}
E:={e1, e2, e3, e4, e5, e6, e7, e8}. Dapat dilihat bahwa Graf di atas merepresentasikan pasangan terurut G:={e1=(1,2),e2=(2,3),e3=(1,3),e4=(1,3),e5=(2,4),e6=(3,4),e7=(3,4),e8=(3,3)}.

## Jenis-jenis graph
### Graf ganda (multi graph):
![Capture23](https://hackmd.io/_uploads/rJpWNNhzyg.png)


### Graf semu (pseudo graph):
![Capture24](https://hackmd.io/_uploads/Bk99X42Mye.png)

### Graf berarah sederhana (directed graph) :
![Capture25](https://hackmd.io/_uploads/HJuimV3GJx.png)

### Graf berarah ganda (multi directed graph) :
![Capture26](https://hackmd.io/_uploads/rJYa7V3Myl.png)


## Social Network Analysis
![Picture1](https://hackmd.io/_uploads/HJQv_IdM1e.png)

Social Network Analysis adalah proses menyelidiki struktur sosial melalui penggunaan jaringan dan teori grafik. Artikel ini memperkenalkan ilmuwan data pada teori jaringan sosial, dengan pengantar singkat tentang teori grafik dan penyebaran informasi. merupakan bidang kajian yang mengekplorasitentang hubungan manusia dengan menggunakan teori graf. Implementasi Social Network Analysis dapat menjelaskan relasi atau hubungan antar aktor melalui visualisasi berbentuk graf. Relasi dalam analisis jaringan sosial dapat diproses dalam bentuk perhitungan yang disebut centrality dalam sebuah jaringan sosial sesuai dengan posisi masing-masing aktor di dalam struktur jaringan tersebut
![Picture2](https://hackmd.io/_uploads/r1NdOUdfke.png)

terdapat node yang mewakili 
orang atau individu atau aktor. 
Relasi  antar objek  dapat dinyatakan dengan link 
atau edges yang terjadi antara aktor tersebut 
Social network terdiri dari banyak aktor 
yang mempunyai relasi satu sama lain hingga
membentuk peta jaringan sosial yang dinyatakan dengan 
graph

## Langkah-langkah Sentralitas
Node yang sangat sentral memainkan peran kunci dalam jaringan, berfungsi sebagai hub untuk berbagai dinamika jaringan. Namun, definisi dan pentingnya sentralitas mungkin berbeda dari kasus ke kasus, dan dapat merujuk pada ukuran sentralitas yang berbeda:

- Derajat — jumlah tetangga dari node tersebut
- EigenVector / PageRank — lingkaran tetangga yang berulang
- Kedekatan — tingkat kedekatan dengan semua node
- Betweenness — jumlah jalur pendek yang melalui node
    ![Capture21](https://hackmd.io/_uploads/S11ipQnzyx.png)


### Tidak semua node dalam jaringan adalah penting  (aktor)
### Mencari node yang paling penting dalam suatu jaringan
### Centrality adalah penentuan aktor menggunakan ukuran pada Social Network Centrality dalam teori graf dan social network .Dibagi menjadi empat jenis, 
- degree centrality, 
- betweeness centrality, 
- closeness centrality 
- eigenvector centrality

# Betweenness Centrality
Betweenness Centrality adalah metrik yang mengukur
seberapa penting suatu node sebagai penghubung antara
node-node yang lain. Node-node ini juga sering disebut
sebagai gatekeepers karena cenderung mengontrol aliran
informasi antar komunitas. Betweenness centrality dapat
dihitung dengan rumus:
        ![Capture27](https://hackmd.io/_uploads/By0SUN2fyg.png)
Dengan
𝜎𝑠𝑡 = jumlah jalur terpendek antara simpul s dan t
𝜎𝑠𝑡(𝑣) = jumlah jalur terpendek yang melewati node v

- Skor betweeness Centrality mewakili seberapa besar informasi yang tersebar dari suatu aktor. Semakin besar skor, artinya aktor tersebut semakin berperan dalam penyebaran informasi 

- Semakin banyak lintasan yang harus melewati persimpangan itu (misal tidak ada jalan alternatif), maka semakin penting arti persimpangan tersebut. Hal ini menandakan seberapa besar suatu node diperlukan sebagai penghubung dalam penyebaran informasi di dalam jaringan

- Ukuran ini juga dapat digunakan untuk mengidentifikasi boundary spanners, yaitu orang atau node yang berperan sebagai penghubung (jembatan) antara dua komunitas

- Menghitung jumlah lintasan terpendek yang melewati suatu node
- Node dengan  betweenness  tinggi  adalah  penting dalam komunikasi dan penyebaran informasi
- Betweenness Centrality
    ![Picture3](https://hackmd.io/_uploads/ByUBhUdfJx.png)
    ![Picture4](https://hackmd.io/_uploads/Sy4U28_zJg.png)

- Normalisasi Betweenness Centrality
    ![Picture5](https://hackmd.io/_uploads/SJrFhU_fkx.png)

# Point Centrality

Point centrality adalah metrik yang paling langsung
menggambarkan sentralitas suatu node dalam suatu jaringan
social. Derajat sentralitasnya dapat dihitung dengan jumlah
node yang terhubung langsung denganya. Semakin tinggi
derajat suatu node, semakin penting pula node itu di jaringan
sosialnya. Point centrality dapat dihitung dengan rumus:
    ![Capture28](https://hackmd.io/_uploads/H1dL_Nhfke.png)

Dengan
𝐶𝑖
𝐷 = bobot nilai degree centrality
𝑘𝑖 = derajat node ke-1
𝑁 = jumlah node dalam suatu graf

# Closeness Centrality

Closeness Centrality adalah metrik yang mengukur
posisi kasar suatu node dalam jaringan dan memberikan
gambaran tentang berapa jauh jaraknya dengan node lain dari
node yang dimaksud. Biasanya, metrik ini menghitung ratarata jarak semua jalur terpendek dari satu node ke semua node
lain dalam suatu jaringan. Metrik ini bisa dihitung dengan
rumus:
    ![Capture29](https://hackmd.io/_uploads/H1bbYE3Mke.png)

