# Alat Analisis Review Google Play Store

## Gambaran Umum
Script Python ini melakukan analisis menyeluruh terhadap review aplikasi dari Google Play Store. Script ini melakukan scraping review, memproses data, dan menghasilkan berbagai visualisasi dan wawasan untuk membantu memahami pola sentimen dan umpan balik pengguna.

## Fitur
- Scraping review dari Google Play Store
- Analisis temporal pola review
- Analisis respon pengembang
- Analisis sentimen berdasarkan rating
- Visualisasi word cloud untuk review positif dan negatif
- Analisis panjang review
- Pelaporan statistik komprehensif

## Prasyarat
Paket Python berikut diperlukan:
```
google-play-scraper
pandas
matplotlib
seaborn
wordcloud
nltk
```

## Instalasi
1. Instal paket yang diperlukan:
```bash
pip install google-play-scraper pandas matplotlib seaborn wordcloud nltk
```

2. Unduh data NLTK yang diperlukan:
```python
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('punkt_tab')
```

## Cara Penggunaan
1. Atur ID aplikasi target dalam script:
```python
APP_ID = "your.app.id"
```

2. Jalankan script:
```python
python tugas_indi.py
```

## File Output
Script ini menghasilkan beberapa file output:
- `AkademiCrypto_reviews_[TANGGAL].csv`: Data review mentah
- `analisis_bulanan.csv`: Ringkasan analisis bulanan
- Berbagai plot visualisasi yang disimpan selama eksekusi

## Komponen Analisis

### 1. Analisis Temporal
- Melacak pola review dari waktu ke waktu
- Memvisualisasikan tren review bulanan

### 2. Analisis Respon Pengembang
- Menghitung tingkat respon
- Memvisualisasikan pola interaksi pengembang

### 3. Analisis Sentimen
- Mengkategorikan review sebagai Positif (≥4 bintang), Netral (3 bintang), atau Negatif (<3 bintang)
- Menghasilkan visualisasi distribusi sentimen

### 4. Analisis Word Cloud
- Membuat word cloud untuk review positif (hijau)
- Membuat word cloud untuk review negatif (merah)
- Menghapus stopwords bahasa Indonesia untuk visualisasi yang lebih bersih

### 5. Analisis Panjang Review
- Menganalisis distribusi panjang review berdasarkan rating
- Menyediakan visualisasi boxplot

### 6. Analisis Statistik
Menghasilkan statistik komprehensif termasuk:
- Jumlah total review
- Periode review
- Rating rata-rata
- Persentase review positif/negatif
- Tingkat respon pengembang

### 7. Rekomendasi Otomatis
Memberikan wawasan otomatis berdasarkan:
- Tren rating
- Pola respon pengembang
- Umpan balik negatif terbaru

## Contoh Output
Script ini menghasilkan berbagai visualisasi dan ringkasan statistik:
- Grafik tren review bulanan
- Diagram pie respon pengembang
- Plot distribusi sentimen
- Word cloud untuk review positif dan negatif
- Boxplot distribusi panjang review

## Rekomendasi
Script secara otomatis menghasilkan rekomendasi berdasarkan:
- Tren rating terbaru dibandingkan dengan rating keseluruhan
- Tingkat respon pengembang
- Analisis review negatif terbaru

## Penanganan Error
Script ini mencakup penanganan error untuk:
- Masalah scraping data
- Error pemrosesan data
- Data yang hilang atau tidak valid

## Catatan
- Script dikonfigurasi untuk review berbahasa Indonesia secara default
- Stopwords dikonfigurasi untuk bahasa Indonesia
- Timestamp dikonversi ke zona waktu Asia/Jakarta

## Kontribusi
Silakan fork repositori ini dan kirimkan pull request untuk perbaikan apapun.

## Lisensi
Proyek ini bersifat open-source dan tersedia di bawah Lisensi MIT.
