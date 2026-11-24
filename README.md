# 📊 Dynamic Operational Profitability & Marketing Efficiency Dashboard

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-0F172A?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-10B981?style=for-the-badge)

## 📌 Ringkasan Proyek (Project Overview)
Proyek ini merupakan **Dashboard Operasional berbasis Microsoft Excel** yang dirancang untuk memantau kesehatan profitabilitas pesanan, tingkat kerugian (*loss-making orders*), serta efisiensi biaya pemasaran (*marketing spend*) lintas kanal penjualan, *brand*, *region*, dan negara. 

Dengan memanfaatkan **kontrol filter dinamis** dan **conditional formatting**, dashboard ini membantu pemangku kepentingan mengidentifikasi kebocoran margin dan anomali kinerja secara cepat tanpa harus mengolah ulang data mentah secara manual.

---

## 🎯 Latar Belakang & Permasalahan Bisnis
Dalam operasional bisnis multi-segmen yang mencakup **18 brand**, **4 kanal penjualan** (*Distributor, Modern Trade, Online, Wholesale*), dan **18 negara**, pemantauan kinerja menggunakan angka rata-rata agregat sering kali menutupi masalah spesifik di lapangan:
* **Kebocoran Margin Tersembunyi:** Pesanan yang merugi (*loss-making orders*) dan pemberian diskon berlebih pada kombinasi *brand* dan *channel* tertentu tidak langsung terlihat pada laporan ringkasan umum.
* **Inefisiensi Anggaran Pemasaran:** Sulitnya membandingkan seberapa besar biaya iklan (*Marketing Spend*) yang dikeluarkan dibandingkan laba bersih (*Net Profit*) yang dihasilkan di tiap kanal dan wilayah.

---

## ⚙️ Fitur Utama & Arsitektur Dashboard
1. **Panel Filter Dinamis Multi-Dimensi:**
   * Pengguna dapat melakukan *slicing* data secara langsung berdasarkan **Channel**, **Brand**, **Year**, **Region**, dan **Customer Type**.
   * Seluruh kartu KPI utama dan matriks rincian otomatis diperbarui mengikuti kombinasi filter yang dipilih.
2. **Kartu Ringkasan KPI Eksekutif:**
   * Menampilkan indikator kesehatan utama secara sekilas: `Loss-making Rate (%)`, `Total Loss`, `Average Loss per Order`, `Discount Rate (%)`, `Gross Margin (%)`, dan `Net Profit Margin (%)`.
3. **Matriks Evaluasi Operasional & Margin per Brand:**
   * Membandingkan performa `Total Orders`, `Loss-making Orders`, `Loss-making Rate`, dan `Average Loss` antar kanal penjualan, dilengkapi rincian `Gross Sales`, `Discount Spend`, `COGS`, hingga `Net Profit`.
4. **Matriks Efisiensi Pemasaran Lintas Segmen:**
   * Mengevaluasi rasio `Marketing Spend` terhadap `Net Profit` (*Cost-to-Profit Ratio*) berdasarkan dimensi **Brand**, **Region**, dan **Country**.
5. **Visual Alert dengan Conditional Formatting:**
   * Skala warna **Hijau – Kuning – Merah** diterapkan secara otomatis untuk menandai performa sehat, area peringatan, dan titik kritis berisiko tinggi.

---

## 🔍 Temuan Utama (Key Insights)
Berdasarkan tampilan keseluruhan data (*All Segments*):
* **Anomali Kerugian Terkonsentrasi di Kanal Online:** Tingkat pesanan merugi keseluruhan berada di angka **4,31%** dengan total kerugian **-$1.969.747,00** (rata-rata **-$2.506,04** per pesanan rugi). Kanal **Online** menyumbang tingkat kerugian tertinggi, terutama pada *brand* **RoastTrail (49,16%)** dan **AquaGlow (48,65%)**.
* **Ketimpangan Efisiensi Biaya Pemasaran:**
  * Kanal **Wholesale** dan **Distributor** menunjukkan efisiensi tertinggi dengan *Cost-to-Profit Ratio* yang stabil di kisaran **30%–43%** lintas wilayah.
  * Kanal **Online** mencatat *Cost-to-Profit Ratio* di atas **100%** di seluruh wilayah (**138%–183%**), menandakan belanja pemasaran yang melampaui laba bersih yang dihasilkan.
* **Kesehatan Margin Kotor vs Tingkat Diskon:** Secara agregat, *Gross Margin* berada di level sehat (**40,54%**) dengan rata-rata tingkat diskon **15,40%**, namun beberapa *brand* seperti *PantryPeak* dan *SparkShield* memiliki *Gross Margin* di bawah 30% yang perlu diawasi.

---

## 💡 Rekomendasi Bisnis
1. **Audit Kebijakan Diskon & Struktur Biaya Online:** Melakukan peninjauan batas maksimum diskon dan biaya pemenuhan pesanan (*fulfillment*) di kanal Online, khususnya untuk *brand* **AquaGlow** dan **RoastTrail**.
2. **Realokasi Anggaran Pemasaran:** Mengalihkan sebagian alokasi *marketing spend* dari kampanye Online ber-ROI negatif ke kanal **Wholesale** dan **Distributor** yang terbukti menghasilkan rasio laba bersih lebih optimal.
3. **Monitoring Berkala Berbasis Filter:** Menggunakan dashboard ini dalam tinjauan operasional mingguan/bulanan untuk memantau perbaikan margin pada negara dan *brand* dengan indikator merah.

---

## 🛠️ Tools & Teknik yang Digunakan
* **Microsoft Excel:** Pemodelan data, agregasi dinamis, dan penyusunan tata letak dashboard.
* **Dynamic Formulas & Filtering:** Integrasi kontrol filter interaktif lintas dimensi (`Channel`, `Brand`, `Year`, `Region`, `Customer Type`).
* **Conditional Formatting:** Pemetaan ambang batas (*threshold*) berbasis warna untuk deteksi anomali cepat.

---

## 📸 Tangkapan Layar Dashboard
> *Catatan: Simpan gambar dashboard di folder `assets/` pada repositori Anda agar tampil otomatis di bawah ini.*

1. **Ringkasan KPI & Matriks Loss-Making Orders per Brand**
   ![Dashboard Overview](assets/dashboard_overview.png)

2. **Analisis Cost-to-Profit Ratio per Brand & Region**
   ![Marketing Efficiency Brand & Region](assets/marketing_brand_region.png)

3. **Analisis Cost-to-Profit Ratio per Country**
   ![Marketing Efficiency Country](assets/marketing_country.png)

---

## 🚀 Cara Menggunakan File
1. Unduh file `.xlsx` dari repositori ini.
2. Buka menggunakan **Microsoft Excel** (disarankan versi 2019 ke atas atau Microsoft 365).
3. Gunakan sel kontrol pada bagian **Click In Here** (`Channel`, `Brand`, `Year`, `Region`, `Customer Type`) untuk memfilter tampilan data sesuai kebutuhan analisis.
