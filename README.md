<h1 align="center">Analisis Sentimen Ulasan Aplikasi Bilibli.com</h1>


##Overview Proyek
Proyek ini bertujuan untuk melakukan analisis sentimen pada ulasan pengguna aplikasi Bilibli.com menggunakan algoritma Naive Bayes Classifier. Proses analisis sentimen ini mencakup beberapa tahapan utama, dengan highlight pada penggunaan berbagai teknik spellchecking untuk meningkatkan kualitas data teks sebelum pemodelan.

# Analisis Sentimen Ulasan Aplikasi Bilibli.com

## Alur Kerja Proyek

**Pengumpulan dan Pemuatan Data:** Memuat dataset ulasan aplikasi Bilibli.com.

**Eksplorasi Data Awal (EDA):** Memahami karakteristik data ulasan, termasuk distribusi rating dan sebaran kelas sentimen.

**Preprocessing Teks Bahasa Indonesia:** Melakukan pembersihan dan normalisasi data teks. Tahap ini mencakup:

**Tokenisasi:** Memisahkan teks menjadi unit-unit kata.

**Pembersihan Token:** Menghilangkan karakter yang tidak diinginkan, angka, tanda baca, dan emoji, serta menangani kata slang.

**Spellchecking:** Menggunakan pendekatan berbasis probabilitas (Norvig) dan eksperimen dengan spellchecking untuk memperbaiki kesalahan ejaan pada ulasan berbahasa Indonesia.

**Penanganan Negasi:** Menggabungkan kata negasi dengan kata berikutnya untuk mempertahankan makna.

**Penghapusan Stopwords:** Menghilangkan kata-kata umum yang tidak memberikan makna signifikan.

**Stemming:** Mengubah kata menjadi bentuk dasarnya.

**Pembagian Dataset:** Membagi dataset yang sudah bersih menjadi data training dan testing.

**Pemodelan dengan Naive Bayes:** Menggunakan berbagai varian algoritma Naive Bayes (Multinomial, Bernoulli, Gaussian, Complement) untuk melatih model klasifikasi sentimen.

**Evaluasi Model:** Mengevaluasi performa model menggunakan metrik seperti Akurasi, Precision, Recall, F1-Score, dan ROC AUC, serta memvisualisasikan Confusion Matrix.

## Algoritma yang Digunakan

**Naive Bayes Classifier:** Algoritma klasifikasi probabilistik berdasarkan Teorema Bayes, dengan asumsi independensi antar fitur. Digunakan untuk mengklasifikasikan ulasan ke dalam sentimen Positif, Netral, atau Negatif. Variasi yang diuji meliputi:
- Multinomial Naive Bayes
- Bernoulli Naive Bayes
- Gaussian Naive Bayes
- Complement Naive Bayes

## Ekstraksi Fitur
**TF-IDF Vectorizer:** Digunakan untuk mengubah teks menjadi representasi numerik (vektor) berdasarkan frekuensi kata dan invers frekuensi dokumen.

**Word2Vec (Eksperimental):** Digunakan sebagai bagian dari eksperimen spellchecking untuk mencari kata-kata yang paling mirip berdasarkan konteks.

**Norvig's Spell Checker:** Algoritma spellchecking berbasis probabilitas yang menghitung kandidat koreksi ejaan.


## Hasil 
<img width="576" height="180" alt="image" src="https://github.com/user-attachments/assets/c2480016-bc49-4a97-a899-8fe74e12228c" />

