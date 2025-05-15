Dokumentasi  **Markdown (`README.md`)** notebook `analisisCovid.ipynb` Project Python Pengantar Statistika:

---

## Analisis Data COVID-19 Indonesia

Notebook ini berisi analisis data COVID-19 di Indonesia menggunakan Python, pandas, dan visualisasi data dengan matplotlib.

---

### Teknologi dan Library yang Digunakan

* Python 3.x
* Jupyter Notebook
* `pandas` – untuk manipulasi dan analisis data
* `matplotlib.pyplot` – untuk visualisasi grafik
* `numpy` – (optional, jika digunakan untuk manipulasi numerik)

---

### Struktur File

* `analisisCovid.ipynb` – Notebook utama berisi proses analisis data
* (Opsional) `data.csv` atau `covid_data.csv` – File data yang digunakan (belum ditemukan pada notebook, diasumsikan sudah tersedia)

---

### Langkah Analisis

1. **Import Library**
   Notebook mengimpor pustaka utama seperti `pandas` dan `matplotlib.pyplot`.

2. **Load Dataset**
   Menggunakan `pd.read_csv()` untuk membaca data kasus COVID-19 di Indonesia.

3. **Melihat Data**
   Menampilkan data awal dengan `head()` dan memeriksa informasi dengan `info()`.

4. **Membersihkan Data**

   * Menghapus kolom tidak relevan jika ada
   * Menangani nilai kosong atau duplikat

5. **Analisis Tren**

   * Visualisasi kasus harian
   * Perbandingan antara kasus sembuh, positif, dan meninggal

6. **Visualisasi**
   Menggunakan `matplotlib` untuk membuat grafik:

   * Grafik garis tren kasus
   * Grafik batang perbandingan

---

### 📈 Contoh Visualisasi

```python
plt.plot(df['tanggal'], df['kasus_baru'], label='Kasus Baru')
plt.plot(df['tanggal'], df['sembuh'], label='Sembuh')
plt.legend()
plt.title('Tren Harian Kasus COVID-19')
plt.xlabel('Tanggal')
plt.ylabel('Jumlah')
plt.show()
```

---

### 💡 Insight yang Didapat

* Terlihat fluktuasi jumlah kasus harian di Indonesia.
* Grafik membantu dalam mengidentifikasi puncak dan penurunan kasus.
* Perbandingan antar kasus positif, sembuh, dan meninggal mempermudah pemantauan dampak pandemi.

---

### 📝 Catatan

* Pastikan dataset terbaru tersedia agar analisis tetap relevan.
* Tambahkan pengecekan anomali data seperti outlier jika dibutuhkan.
* Perhatikan format tanggal dan urutan data saat memplot grafik.

---
