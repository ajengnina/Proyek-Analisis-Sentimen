# 📱 Sentiment Analysis of PlayStore Reviews

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna dari aplikasi Android di Google PlayStore. Data dikumpulkan melalui scraping, dilabeli secara manual ke dalam tiga kategori sentimen (positif, negatif, netral), dan digunakan untuk melatih model klasifikasi teks.

---

## 🧾 Deskripsi Proyek

Dalam era digital, ulasan pengguna menjadi indikator penting bagi kualitas dan kepuasan terhadap aplikasi. Dengan menggunakan teknik Natural Language Processing (NLP), proyek ini menganalisis ribuan ulasan untuk mengklasifikasikan sentimen pengguna secara otomatis.

---

## 🔍 Tujuan

- Mengklasifikasikan sentimen ulasan pengguna (positif, negatif, netral)
- Mengevaluasi performa beberapa model machine learning untuk klasifikasi teks
- Membangun antarmuka pengguna sederhana dengan Streamlit untuk mendemokan prediksi

---

## 🧰 Tools dan Teknologi

- **Bahasa Pemrograman**: Python
- **Web Scraping**: BeautifulSoup
- **Preprocessing NLP**: NLTK
- **Feature Extraction**: TF-IDF Vectorizer
- **Modeling**: Scikit-Learn (Logistic Regression, Naive Bayes, SVM)
- **Deployment**: Streamlit
- **Data Handling**: Pandas

---

## 🧪 Langkah-Langkah

1. **Data Collection**
   - Scraping ±900 ulasan dari masing-masing 5 aplikasi di Google PlayStore menggunakan BeautifulSoup
   - Menyimpan data dalam format CSV

2. **Preprocessing**
   - Lowercasing, stopword removal, dan tokenisasi
   - Optional: stemming dan lemmatization

3. **Labeling**
   - Manual labeling ke dalam 3 kelas sentimen: Positif, Negatif, dan Netral

4. **Feature Engineering**
   - TF-IDF vectorization untuk mengubah teks menjadi representasi numerik

5. **Modeling**
   - Melatih dan mengevaluasi beberapa model: Logistic Regression, Multinomial Naive Bayes, dan Support Vector Machine (SVM)
   - Evaluasi menggunakan metrik: accuracy, precision, recall, dan F1-score

6. **Deployment**
   - Membangun antarmuka interaktif menggunakan Streamlit untuk prediksi sentimen berbasis input teks

---

## 📊 Hasil

- Model terbaik menunjukkan akurasi di atas 85% pada data uji
- SVM dan Logistic Regression memberikan performa paling konsisten
- Streamlit app memungkinkan pengguna menguji prediksi sentimen secara real-time

---

## 🚀 Cara Menjalankan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/ajengnina/Proyek-Analisis-Sentimen.git
   cd Proyek-Analisis-Sentimen

2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3. Jalankan aplikasi Streamlit:
   ```bash
   streamlit run app.py
