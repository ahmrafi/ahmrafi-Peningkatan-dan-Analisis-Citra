### Peningkatan dan Analisis Citra

Skrip Python ini melakukan dua teknik utama peningkatan citra: Pemerataan Histogram dan Transformasi Fourier. Ini juga mencakup visualisasi citra asli, histogramnya, dan citra yang ditingkatkan.

#### Fitur:

1. **Pemerataan Histogram:**
   - Meningkatkan kontras citra keabuan dengan mendistribusikan ulang intensitas piksel.
   - Menormalisasi fungsi distribusi kumulatif (CDF) intensitas piksel.
   - Meningkatkan kejelasan detail di daerah gelap atau terang.

2. **Transformasi Fourier:**
   - Mengonversi citra domain spasial menjadi domain frekuensi.
   - Menggeser komponen frekuensi nol ke pusat untuk visualisasi.
   - Memvisualisasikan spektrum magnitudo menggunakan skala logaritmik.

#### Penggunaan:
1. **Citra Masukan:**
   - Sediakan jalur ke citra masukan (`image_path`) dalam skrip.
   - Skrip membaca citra dan mengonversinya ke citra keabuan.

2. **Pemerataan Histogram:**
   - Terapkan pemerataan histogram ke citra keabuan menggunakan fungsi `histogram_equalization`.
   - Menghasilkan histogram citra keabuan asli dan citra yang ditingkatkan.

3. **Transformasi Fourier:**
   - Melakukan Transformasi Fourier pada citra keabuan menggunakan fungsi `fourier_transform`.
   - Menggeser komponen frekuensi nol ke pusat untuk visualisasi yang lebih baik.

4. **Analisis Citra RGB:**
   - Memperluas pemerataan histogram dan Transformasi Fourier ke setiap saluran warna (Merah, Hijau, Biru) dari citra RGB.
   - Memvisualisasikan histogram dan citra yang ditingkatkan untuk setiap saluran warna.

#### Output:
   - Menampilkan citra asli, citra yang ditingkatkan (pemerataan histogram dan Transformasi Fourier), dan histogramnya yang sesuai.
   - Memberikan wawasan tentang efektivitas teknik peningkatan ini dalam meningkatkan kualitas citra dan analisis.