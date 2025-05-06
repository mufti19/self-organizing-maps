# Pemetaan Dampak Bencana Banjir Menggunakan Self Organizing Maps (SOM)

## Latar Belakang
Indonesia mengalami peningkatan bencana alam dalam tiga dekade terakhir, dengan lebih dari 4 miliar orang terdampak oleh peristiwa alam ekstrem antara tahun 1980-2010. Salah satu bencana yang paling sering terjadi adalah banjir, yang menyebabkan kerugian besar, baik dalam hal korban jiwa maupun kerusakan infrastruktur. Data bencana banjir yang bersumber dari Badan Nasional Penanggulangan Bencana (BNPB) untuk tahun 2021 digunakan dalam penelitian ini, dengan fokus pada 514 kabupaten/kota di Indonesia.

Dengan menggunakan metode **Self Organizing Maps (SOM)**, penelitian ini bertujuan untuk mengklasifikasikan kabupaten/kota yang terdampak banjir berdasarkan dampak yang ditimbulkan oleh bencana. SOM dipilih karena kemampuannya untuk menangani data berdimensi tinggi dan pencilan dalam data.

## Tujuan Penelitian
Penelitian ini bertujuan untuk:
1. Menyusun pemetaan dampak bencana banjir berdasarkan data dari 514 kabupaten/kota di Indonesia pada tahun 2021.
2. Menggunakan metode **Self Organizing Maps (SOM)** untuk mengelompokkan kabupaten/kota ke dalam beberapa gerombol (cluster).
3. Mengidentifikasi karakteristik masing-masing gerombol untuk memberikan rekomendasi mitigasi bencana yang lebih tepat.

## Data yang Digunakan
- **Sumber Data**: Data dampak bencana banjir pada tahun 2021 dari Badan Nasional Penanggulangan Bencana (BNPB).
- **Jumlah Data**: 514 kabupaten/kota di Indonesia, dengan 298 kabupaten/kota yang terdampak banjir pada tahun 2021.
- **Peubah**: Terdiri dari 10 peubah numerik, termasuk jumlah korban, kerusakan rumah, kerusakan fasilitas, dan dampak lainnya.

## Metode
Metode yang digunakan dalam penelitian ini adalah **Self Organizing Maps (SOM)**, yang termasuk dalam kategori algoritma **unsupervised learning**. SOM mengurangi dimensi data yang besar dengan cara memetakan data ke dalam ruang dua dimensi yang lebih mudah dipahami. Keunggulan metode SOM adalah kemampuannya untuk menangani data berdimensi tinggi dan mendeteksi pencilan, yang sangat berguna dalam konteks data bencana yang memiliki variasi besar.

### Proses Analisis:
1. **Pembersihan Data**: Data yang digunakan diolah untuk menghilangkan missing values dan pencilan, serta dilakukan standardisasi agar data lebih mudah dianalisis menggunakan SOM.
2. **Pembentukan Gerombol**: Dengan menggunakan SOM, data dari 514 kabupaten/kota dikelompokkan menjadi tujuh gerombol berdasarkan dampak bencana banjir yang ditimbulkan.
3. **Evaluasi Model**: Model SOM dievaluasi menggunakan beberapa indeks validasi gerombol, termasuk Indeks Dunn, Indeks Silhouette, dan Indeks Connectivity, untuk menentukan jumlah gerombol yang optimal.

## Hasil Penelitian
- **Jumlah Gerombol**: Berdasarkan analisis SOM, ditemukan tujuh gerombol yang menggambarkan karakteristik dampak bencana banjir di Indonesia.
  - **Gerombol 1, 4, dan 5**: Mengalami dampak terbesar, dengan korban jiwa, kerusakan rumah, dan fasilitas yang signifikan.
  - **Gerombol 2 dan 3**: Kabupatan/kota ini memiliki karakteristik yang lebih baik dalam menangani dampak bencana banjir.
  - **Gerombol 6 dan 7**: Daerah-daerah ini lebih tahan terhadap dampak bencana, dengan kerusakan yang lebih sedikit.

- **Pemetaan Wilayah**: Peta SOM yang dihasilkan menunjukkan distribusi dampak bencana banjir di seluruh wilayah Indonesia. Wilayah dengan gerombol 1, 4, dan 5 menunjukkan tingkat kerusakan yang tinggi, sementara gerombol 6 dan 7 menunjukkan ketahanan yang lebih baik terhadap banjir.

## Simpulan
Berdasarkan hasil analisis, penelitian ini menemukan bahwa sebagian besar kabupaten/kota di Indonesia sudah baik dalam menangani dampak bencana banjir, meskipun ada beberapa daerah yang masih memerlukan perhatian lebih. Gerombol 1, 4, dan 5 merupakan wilayah yang harus diperhatikan lebih serius, karena mengalami dampak yang sangat besar.

Pemetaan ini dapat digunakan oleh pemerintah dan lembaga terkait untuk mengambil langkah-langkah mitigasi yang lebih tepat, seperti pembangunan infrastruktur penahan banjir, sistem peringatan dini, dan perencanaan evakuasi yang lebih efektif.

## Teknologi yang Digunakan
- **Python**: Untuk pemrosesan data dan analisis menggunakan paket seperti pandas, numpy, dan scikit-learn.
- **Self Organizing Maps (SOM)**: Untuk analisis gerombol menggunakan neural network.
- **Matplotlib/Seaborn**: Untuk visualisasi data dan peta gerombol.
