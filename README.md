# 📈 Peta Kolaborasi Investor Startup di Indonesia 🇮🇩

Proyek ini menggunakan pendekatan **Social Network Analysis (SNA)** untuk memetakan hubungan **co-investment antar investor** yang mendanai startup Indonesia. Fokus utama adalah mengidentifikasi **key players**, **koalisi informal**, dan **struktur jaringan kolaborasi** di ekosistem startup Indonesia.

---

## 🧠 Tujuan Penelitian

- Menganalisis siapa saja investor yang paling aktif melakukan co-investment.
- Mengidentifikasi cluster investor yang sering berkolaborasi.
- Mengungkap apakah investor seperti **East Ventures** lebih condong berkolaborasi dengan investor lokal atau asing.
- Memberikan wawasan strategis dalam dunia ventura dan pembiayaan startup.

---

## 📁 Struktur Dataset

### `investment_data.csv`
Berisi data investasi untuk membangun jaringan investor.

| Field              | Deskripsi                                |
|--------------------|-------------------------------------------|
| `Startup_ID`       | ID unik startup                           |
| `Investor_Name`    | Nama investor / venture capital           |
| `Investment_Date`  | Tanggal investasi                         |
| `Investment_Stage` | Tahap pendanaan (Seed, Series A, dll)     |
| `Investment_Amount`| Nilai investasi (dalam angka dummy)       |

### `startup_data.csv`
Data profil startup yang dapat digunakan untuk analisis tambahan.

| Field            | Deskripsi                                 |
|------------------|--------------------------------------------|
| `Startup_ID`     | ID unik startup                            |
| `Startup_Name`   | Nama startup                               |
| `Founding_Date`  | Tahun berdiri                              |
| `HQ_Location`    | Lokasi kantor pusat startup                |

---

## ⚙️ Tools dan Library

- `pandas` untuk pembersihan dan manipulasi data
- `networkx` untuk analisis dan pembangunan graf
- `matplotlib` untuk visualisasi jaringan
- `Gephi` (opsional) untuk visualisasi lanjutan

---

## 🔍 Analisis Jaringan yang Dilakukan

- **Degree Centrality**: Mengukur siapa investor paling aktif.
- **Betweenness Centrality**: Menilai siapa penghubung antar kelompok investor.
- **Clustering Coefficient**: Seberapa erat kolaborasi antar node.
- **Community Detection**: Mengidentifikasi cluster investor (modularity class).
- **Visualisasi Graf**: Peta kolaborasi investor startup Indonesia.

---

## 📊 Contoh Output

- 📌 Daftar investor dengan degree centrality tertinggi
- 🧭 Cluster investor berdasarkan modularity
- 🔍 Temuan khusus: siapa saja mitra co-investasi East Ventures?
- 🕸️ Visualisasi jaringan kolaborasi antar investor

---
