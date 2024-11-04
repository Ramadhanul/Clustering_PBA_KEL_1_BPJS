# Clustering dan Analisis Sentimen Berita Layanan BPJS

## Deskripsi Proyek
Proyek ini bertujuan untuk menganalisis persepsi publik terhadap layanan BPJS Kesehatan di Indonesia dengan menggunakan metode pengelompokan (clustering) dan analisis sentimen pada artikel berita. Data dikumpulkan melalui web scraping dari berbagai portal berita terpercaya yang membahas topik BPJS, kemudian diproses untuk mengidentifikasi tren sentimen dan pengelompokan tema terkait BPJS.

## Anggota Kelompok
- Naura Jasmine Azzahra - 5026211005
- Ramadhanul Husna A. M. - 5026211059
- Fikri Septa Setiawan - 5026211109

## Struktur Proyek
Proyek ini meliputi beberapa langkah utama, yaitu:

1. **Akuisisi Data**
   - Data diperoleh melalui web scraping dari situs-situs berita terpercaya, menggunakan pustaka Python seperti `Selenium`, `Dateparser`, dan `Newspaper`.
   - Dataset yang terbentuk berisi informasi judul, tautan, tanggal publikasi, isi konten artikel, dan sumber media.

2. **Praproses Data**
   - Proses pembersihan dan normalisasi teks meliputi penghapusan teks pendek, pembersihan karakter yang tidak diperlukan, pengubahan teks menjadi lowercase, penghapusan stopwords, dan stemming.
   - Dataset hasil praproses kemudian disimpan dalam format CSV untuk keperluan analisis lebih lanjut.

3. **Definisi Dataset**
   - Dataset terdiri dari:
     - **Link Artikel Berita**: Tautan berita yang memuat informasi terkait BPJS.
     - **Konten Artikel Berita**: Berisi konten lengkap dari artikel berita yang telah dikumpulkan.
     - **Hasil Praproses**: Konten berita yang telah dibersihkan untuk keperluan analisis.

4. **Analisis Data dan Pemodelan**
   - **Clustering**: Menggunakan metode TF-IDF, Bag of Words (BoW), dan Cosine Similarity untuk mengelompokkan artikel berdasarkan konten.
   - **Analisis Sentimen**: Mengidentifikasi sentimen positif, negatif, atau netral pada artikel terkait BPJS.
   - **Evaluasi**: Penggunaan metode Silhouette Score, Calinski-Harabasz Score, dan Davies-Bouldin Score untuk mengukur kualitas clustering.

## Teknologi dan Library yang Digunakan
- **Python**: Untuk implementasi utama analisis dan pemodelan data.
- **Selenium, Dateparser, Newspaper**: Untuk scraping data artikel berita.
- **Pandas, Numpy, Scikit-learn, Matplotlib**: Untuk analisis data, pemodelan clustering, dan visualisasi hasil.

## Cara Menjalankan Proyek
1. Clone repositori ini.
2. Pastikan untuk menginstal semua library yang dibutuhkan:
   ```bash
   pip install -r requirements.txt
