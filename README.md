# Rating Movie Analysis

Analisis rating film adalah suatu proses evaluasi yang melibatkan pemahaman dan penilaian terhadap berbagai aspek yang memengaruhi atau mencirikan tingkat kepuasan atau penerimaan suatu film oleh penonton atau kritikus

## Penjelasan

- Dataset
Dataset yang di gunakan adalah dataset yang berasal dari kaggle. Dataset IMDB berisi ulasan film beserta sentimen (positive/negative) dari penontonnya.
Jumlah total data dalam dataset adalah 50.000 baris dan 2 kolom: 'review' (ulasan film) dan 'sentiment' (sentimen).
Dataset ini memiliki dua kelas sentimen, yaitu 'positive' dan 'negative', yang masing-masing berisi 25.000 ulasan

- Permasalahan dan Tujuan Eksperimen
Permasalahan: membangun model klasifikasi sentimen yang dapat memprediksi apakah suatu ulasan film bersifat positif atau negatif
Tujuan eksperimen: mengembangkan model klasifikasi sentimen yang memiliki tingkat akurasi yang tinggi dalam memprediksi sentimen suatu ulasan film
- Model dan Alur Tahapan Eksperimen
Model yang Digunakan:

Dalam eksperimen ini, beberapa model klasifikasi digunakan untuk membandingkan performa. Model yang digunakan meliputi:
1. Logistic Regression
2. Random Forest Classifier
3. Gaussian Naive Bayes
4. K-Nearest Neighbors
5. XGBoost Classifier

Alur Tahapan Eksperimen:
1. Load Dataset: Memuat dataset IMDB yang berisi ulasan film dan sentimen.
2. Text Pre-processing: Melakukan pre-processing pada data teks, termasuk membersihkan teks, 3. mengonversi teks menjadi lowercase, menghapus tanda baca, dan lemmatisasi kata-kata.
4. Data Visualization: Visualisasi kata-kata yang paling umum dalam ulasan positif dan negatif menggunakan WordCloud dan barplot.
5. Splitting Dataset: Membagi dataset menjadi data pelatihan dan data pengujian.
6. Feature Extraction: Menggunakan metode TF-IDF untuk mengonversi teks menjadi vektor fitur yang dapat digunakan oleh model.
7. Model Selection: Memilih beberapa model klasifikasi yang berbeda untuk diuji.
8. Training and Testing Models: Melatih dan menguji model-model yang dipilih menggunakan data pelatihan dan pengujian.
9. Model Evaluation: Evaluasi performa model dengan menggunakan matriks konfusi, visualisasi heatmap, dan laporan klasifikasi.

Uji Performa Model
1. Model yang dipilih untuk digunakan adalah Logistic Regression berdasarkan hasil uji performa.
2. Performa model diukur menggunakan matriks konfusi, heatmap, dan laporan klasifikasi.
3. Hasil evaluasi menunjukkan akurasi model sekitar 86% dengan baik dalam memprediksi sentimen positif dan negatif.
