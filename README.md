# 🚀 Universal Clustering & Segmentation Toolkit

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)

## 📋 Overview (Gambaran Umum)

**Universal Clustering Toolkit** adalah kerangka kerja (*framework*) analisis data berbasis Python yang dirancang untuk melakukan segmentasi bisnis secara otomatis. 

Berbeda dengan skrip analisis biasa, toolkit ini dilengkapi dengan fitur **Auto-Adapter** yang mampu mendeteksi struktur dataset secara cerdas—baik itu data Transaksi Ritel (*E-Commerce*) maupun data Performa Iklan (*Marketing Ads*)—dan menerapkan algoritma *Machine Learning* yang sesuai tanpa perlu konfigurasi manual yang rumit.

### 🌟 Key Features (Fitur Utama)

* **🧠 Smart Auto-Adapter:** Otomatis mengenali kolom dataset (misal: membedakan `Transaction ID` vs `InvoiceNo`).
* **🛒 Automated RFM Analysis:** Menghitung *Recency, Frequency, Monetary* secara instan untuk data transaksi.
* **📊 Marketing Performance Mode:** Mendeteksi data iklan dan melakukan klasterisasi berdasarkan *Cost vs Revenue*.
* **📈 Hybrid Clustering Engine:** Menggunakan algoritma **K-Means** untuk segmentasi utama dan **DBSCAN** untuk deteksi *noise*.
* **🖥️ Interactive GUI:** Jendela *File Picker* interaktif (berbasis Tkinter) untuk kemudahan penggunaan.
* **🏷️ Auto-Labeling:** Memberikan label bisnis otomatis (misal: *Platinum, Gold, Silver*) berdasarkan data statistik.

---

## 🛠️ Installation (Instalasi)

Pastikan Anda telah menginstal Python 3.x. Ikuti langkah berikut untuk menjalankan toolkit di komputer lokal Anda:

1.  **Clone Repository ini:**
    ```bash
    git clone [https://github.com/username-anda/universal-clustering-toolkit.git](https://github.com/username-anda/universal-clustering-toolkit.git)
    cd universal-clustering-toolkit
    ```

2.  **Install Library yang Dibutuhkan:**
    ```bash
    pip install -r requirements.txt
    ```

---

## 🚀 How to Use (Cara Penggunaan)

1.  Jalankan file utama melalui terminal atau VS Code:
    ```bash
    python main.py
    ```

2.  Akan muncul menu interaktif di terminal. Ketik **'y'** untuk memulai.

3.  **Jendela Pop-up** akan muncul. Pilih file CSV Anda (mendukung format Ritel maupun Marketing).

4.  Sistem akan memproses data dan menampilkan:
    * Status deteksi mode (RFM / Marketing).
    * Grafik **Scatter Plot** interaktif.
    * File hasil (`RESULT_namafile.csv`) akan tersimpan otomatis.

---

## 📂 Supported Datasets (Dataset yang Didukung)

Toolkit ini telah diuji dan valid untuk struktur data berikut:

| Tipe Data | Contoh Struktur Kolom | Metode Analisis |
| :--- | :--- | :--- |
| **Transaksi E-Commerce** | `InvoiceNo`, `Date`, `CustomerID`, `Price` | RFM Analysis + K-Means |
| **Penjualan Ritel** | `Transaction ID`, `Qty`, `Total Amount` | RFM Analysis + K-Means |
| **Marketing Ads** | `Ad Group`, `Impressions`, `Clicks`, `Cost` | Performance Clustering |

---

## 📸 Screenshots (Tangkapan Layar)

### 1. Antarmuka GUI & Terminal
*(Masukkan screenshot terminal Anda yang ada ASCII Art di sini)*
![Terminal Interface](<img width="768" height="357" alt="image" src="https://github.com/user-attachments/assets/c5fb5ee1-30fa-4dfe-b735-520af8f140d9" />
)

### 2. Hasil Segmentasi Pelanggan (RFM)
*(Masukkan screenshot grafik scatter plot OnlineRetail.csv)*
![Customer Segmentation](<img width="941" height="589" alt="image" src="https://github.com/user-attachments/assets/a282668c-289c-46b4-b3b8-ffe4645a16f4" />)(<img width="797" height="511" alt="image" src="https://github.com/user-attachments/assets/d4dd4e6d-8195-4eba-aaaf-8f9cddbd5bcf" />)

### 3. Hasil Segmentasi Iklan (Marketing)
*(Masukkan screenshot grafik scatter plot final_shop_6modata.csv)*
![Ads Performance](<img width="769" height="486" alt="image" src="https://github.com/user-attachments/assets/880d193c-e758-428b-940b-a24cd57fe2f9" />)

---

## 🧠 Project Structure

```text
universal-clustering-toolkit/
├── data/                   # Folder untuk menyimpan file CSV (Opsional)
├── output/                 # Folder hasil (Result.csv)
├── main.py                 # Source code utama (Toolkit)
├── requirements.txt        # Daftar library python
└── README.md               # Dokumentasi Proyek
