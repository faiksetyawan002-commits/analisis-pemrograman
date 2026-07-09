# Sistem Pencarian Rute Antar Gedung Kampus

## Deskripsi
Proyek ini merupakan implementasi algoritma **Breadth First Search (BFS)** dan **Depth First Search (DFS)** untuk melakukan pencarian rute antar gedung kampus yang direpresentasikan sebagai **graph**.

Graph direpresentasikan menggunakan dua struktur data, yaitu:

- Adjacency List
- Adjacency Matrix

Program melakukan pengujian terhadap kedua algoritma untuk membandingkan performanya berdasarkan waktu eksekusi, jumlah node yang dikunjungi, serta penggunaan memori pada beberapa ukuran graph.

---

## Tujuan

- Membangun sistem pencarian rute antar gedung kampus.
- Mengimplementasikan algoritma BFS dan DFS.
- Membandingkan performa BFS dan DFS.
- Menganalisis kompleksitas waktu dan ruang dari masing-masing algoritma.

---

## Fitur

- Implementasi Breadth First Search (BFS)
- Implementasi Depth First Search (DFS)
- Representasi graph menggunakan Adjacency List
- Representasi graph menggunakan Adjacency Matrix
- Generate graph secara otomatis
- Pengujian pada berbagai ukuran data
- Analisis waktu eksekusi
- Analisis penggunaan memori
- Perbandingan hasil BFS dan DFS

---

## Struktur Data

Program menggunakan dua representasi graph:

### Adjacency List

- Kompleksitas ruang: **O(V + E)**
- Lebih hemat memori
- Cocok untuk graph yang jarang (Sparse Graph)

### Adjacency Matrix

- Kompleksitas ruang: **O(V²)**
- Akses hubungan antar node lebih cepat
- Cocok untuk graph yang padat (Dense Graph)

---

## Algoritma yang Digunakan

### Breadth First Search (BFS)

Karakteristik:

- Menggunakan Queue (FIFO)
- Menelusuri node per level
- Menemukan jalur terpendek pada graph tidak berbobot

Kompleksitas:

- Waktu : **O(V + E)**
- Ruang : **O(V)**

---

### Depth First Search (DFS)

Karakteristik:

- Menggunakan Stack (LIFO)
- Menelusuri sedalam mungkin sebelum backtracking
- Tidak selalu menghasilkan jalur terpendek

Kompleksitas:

- Waktu : **O(V + E)**
- Ruang : **O(V)**

---

## Dataset Pengujian

Graph dibangkitkan secara otomatis dengan ukuran:

| Skala | Jumlah Node |
|--------|------------:|
| Kecil | 50 |
| Sedang | 100 |
| Besar | 250 |
| Sangat Besar | 500 |

Setiap pengujian dilakukan sebanyak **30 kali** untuk memperoleh hasil yang lebih akurat.

---

## Parameter Pengujian

Program membandingkan:

- Waktu eksekusi
- Standar deviasi waktu
- Jumlah node yang diperiksa
- Penggunaan memori

---

## Hasil Pengujian

Secara umum diperoleh bahwa:

- BFS lebih baik dalam menemukan jalur terpendek.
- DFS memiliki penggunaan memori yang lebih efisien.
- Waktu eksekusi kedua algoritma meningkat seiring bertambahnya jumlah node.
- Kedua algoritma memiliki kompleksitas waktu **O(V + E)**.

---

## Cara Menjalankan Program

1. Pastikan Python telah terpasang.
2. Clone repository.

```bash
git clone https://github.com/username/nama-repository.git
```

3. Masuk ke folder project.

```bash
cd nama-repository
```

4. Jalankan program.

```bash
python main.py
```

---

## Struktur Folder

```
project/
│
├── main.py
├── bfs.py
├── dfs.py
├── graph.py
├── utils.py
├── laporan.pdf
├── README.md
└── assets/
```

*(Sesuaikan dengan struktur folder proyek Anda.)*

---

## Teknologi

- Python 3.x
- Collections (deque)
- Time
- Tracemalloc
- Random

---

## Mata Kuliah

**Analisis Algoritma**

Program Studi Ilmu Komputer  
Fakultas Ilmu Sains dan Teknologi  
Universitas Putra Bangsa

---

## Anggota Kelompok

- Faik Setyawan
- Akhmad Raffi Sarmadan
- Faris Azhar
- Naufal Adi Bis

---

## Referensi

1. Goodrich, M. T., Tamassia, R., & Goldwasser, M. H. *Data Structures and Algorithms in Python*. Wiley.
2. Sedgewick, R., & Wayne, K. *Algorithms (4th Edition)*.
3. Weiss, M. A. *Data Structures and Algorithm Analysis in C++ (4th Edition)*.

---

## Lisensi

Proyek ini dibuat untuk keperluan pembelajaran pada mata kuliah **Analisis Algoritma**.
