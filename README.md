# Analisis-Sentimen

## Deskripsi Proyek
Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan yang diambil dari Aplikasi TikTok. Dengan menggunakan teknik pemrosesan bahasa alami (NLP), proyek ini membersihkan, memproses, dan menganalisis teks untuk mengidentifikasi sentimen positif, negatif, atau netral.

## Tahapan Proyek
a. Preprocessing Text
Proses ini mencakup:

- Import Library: Menggunakan pustaka seperti pandas, nltk, Sastrawi, dan scikit-learn.
- Load Data: Memuat dataset ulasan TikTok.
- Tokenisasi: Memecah teks menjadi kata-kata individu.
- Stopword Removal: Menghapus kata-kata umum yang tidak memiliki makna signifikan.
- Stemming: Mengubah kata menjadi bentuk dasarnya menggunakan Sastrawi.
- TF-IDF Vectorization: Mengubah teks menjadi representasi numerik.
b. Model Machine Learning
Dua model utama yang digunakan dalam klasifikasi sentimen:

Logistic Regression
Random Forest Classifier


## Hasil dan Kesimpulan
Hasil analisis sentimen ulasan TikTok menggunakan dua model, yaitu Random Forest dan Logistic Regression, menunjukkan perbedaan performa yang cukup signifikan. Model Random Forest menghasilkan akurasi 100% pada data latih, tetapi menurun menjadi sekitar 76% - 78% pada data uji, menunjukkan adanya indikasi overfitting. Sementara itu, model Logistic Regression memberikan akurasi yang lebih seimbang, yaitu sekitar 85% - 90% pada data latih dan 75% - 78% pada data uji.

Evaluasi dilakukan dengan menggunakan Confusion Matrix dan Classification Report. Hasil evaluasi menunjukkan bahwa Random Forest lebih cenderung menghafal pola pada data latih, sehingga performanya pada data uji menurun. Sebaliknya, Logistic Regression menunjukkan performa yang lebih konsisten antara data latih dan uji, sehingga lebih stabil dalam klasifikasi sentimen.

Dari segi visualisasi, Word Cloud digunakan untuk mengidentifikasi kata-kata yang paling sering muncul dalam ulasan TikTok, sementara Confusion Matrix membantu dalam memahami kesalahan klasifikasi model. Berdasarkan hasil ini, Logistic Regression lebih direkomendasikan untuk digunakan jika menginginkan model yang lebih generalisasi dengan performa yang stabil, sementara Random Forest dapat dioptimalkan lebih lanjut untuk mengurangi overfitting dan meningkatkan akurasi pada data uji.
