# Association Rule Mining untuk Strategi Cross-Selling dan Bundling Produk Kosmetik

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/reproducibility-verified-brightgreen)

Repositori ini berisi dataset sintetis, kode pemrosesan Python, serta hasil rekapitulasi analisis **Association Rule Mining (Apriori & FP-Growth)** untuk perancangan strategi pemasaran *Cross-Selling* dan *Bundling* pada industri kosmetik.

Penelitian ini dipublikasikan pada **Jurnal Restikom (Riset Teknik Informatika dan Komputer)**.

---

## 👥 Penulis
* **Nabila Zakiyah Zahra** - Program Studi Sains Data, Institut Teknologi Sumatera
* **Renta Siahaan** - Program Studi Sains Data, Institut Teknologi Sumatera
* **Tessa Kania Sagala** - Program Studi Sains Data, Institut Teknologi Sumatera
* **M. Syamsuddin Wisnubroto** - Program Studi Sains Data, Institut Teknologi Sumatera (*Corresponding Author*)
* **Fajri Farid** - Program Studi Sains Data, Institut Teknologi Sumatera

---

## 📌 Ringkasan Hasil Analisis
* **Dataset:** 3.000 transaksi penjualan sintetis dengan 5 produk unik (*Face Wash, Toner, Moisturizer, Serum Vitamin C, Sunscreen*).
* **Frequent Itemsets:** Kedua algoritma (Apriori & FP-Growth) secara konsisten menghasilkan **17 frequent itemset** yang identik pada `min_support = 0.10`.
* **Efisiensi Komputasi:** Algoritma Apriori mencatatkan waktu eksekusi sebesar `0.0177 detik`, lebih cepat dibandingkan FP-Growth (`0.3632 detik`) pada dataset ini.
* **Aturan Asosiasi:** Terbentuk total **52 aturan** (14 aturan *cross-selling* dan 38 aturan *bundling*).
* **Konsistensi Lift:** Seluruh nilai *lift* telah diverifikasi dan terbukti **100% konsisten secara matematis**.

---

## 📁 Struktur Repositori
```text
├── README.md                           <- Dokumentasi utama repositori
├── requirements.txt                    <- Pustaka Python yang dibutuhkan
├── kosmetik_transactions.xlsx          <- Dataset 3.000 transaksi kosmetik
├── Association_Rule_Mining.ipynb       <- Jupyter Notebook analisis lengkap
│
├── results/                            <- Rekapitulasi hasil analisis (.csv)
│   ├── frequent_itemsets_apriori.csv
│   ├── association_rules.csv
│   ├── cross_selling_rules.csv
│   ├── bundling_rules.csv
│   └── lift_verification.csv
│
└── figures/                            <- Grafik visualisasi (300 DPI)
    ├── scatter_plot_rules.png
    ├── execution_time_comparison.png
    ├── network_graph_cross_selling.png
    └── network_graph_bundling.png
