Muhammad Farhan

Fasya Burhanis Syauqi

# 📰 AG News Classification with DistilBERT

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![HuggingFace](https://img.shields.io/badge/Transformers-4.30%2B-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

Proyek ini adalah implementasi **Deep Learning** untuk klasifikasi teks berita otomatis (Single-Label Classification) menggunakan model Transformer **DistilBERT**.

Model ini dilatih (fine-tuned) menggunakan dataset **AG News** untuk memprediksi kategori berita dengan akurasi tinggi.

## 📌 Tentang Dataset
Dataset yang digunakan adalah **AG News** yang terdiri dari artikel berita berita yang dikelompokkan menjadi 4 kelas utama:

| Label ID | Kategori | Deskripsi |
|----------|----------|-----------|
| **0** | 🌍 World | Berita internasional & politik global |
| **1** | ⚽ Sports | Berita olahraga |
| **2** | 💼 Business | Ekonomi, pasar saham, & industri |
| **3** | 🔬 Sci/Tech | Teknologi, sains, & gadget |

## 📂 Struktur Proyek
Berikut adalah susunan folder dalam repositori ini:

```text
project_agnews/
├── notebooks/
│   └── Task1_AGNews.ipynb    # Jupyter Notebook utama (Training & Eval)
├── reports/
│   └── report.md             # Laporan hasil analisis & metrik
├── requirements.txt          # Daftar library dependency
└── README.md                 # Dokumentasi proyek (File ini)
