# Neural Machine Translation: Indonesian – Javanese Translator

Neural Machine Translation: Indonesian – Javanese Translator adalah aplikasi penerjemah berbasis Recurrent Neural Network (RNN) dengan mekanisme Attention yang dikembangkan untuk melestarikan Bahasa Jawa dengan menyediakan terjemahan yang akurat dan efisien. Proyek ini merupakan bagian dari Tugas Akhir oleh Muhammad Raihan Khoirudin di Universitas Telkom Bandung, dengan pembimbing utama Dr. Arie Ardiyanti Suryani, S.T., M.T., dan pembimbing kedua Bunyamin, M.Kom.

## Deskripsi Proyek
Aplikasi ini menggunakan pendekatan RNN-LSTM dengan dua variasi mekanisme Attention, yaitu Bahdanau dan Luong. Dataset yang digunakan terdiri dari pasangan kalimat Bahasa Indonesia dan Bahasa Jawa dengan standar Ngoko, yang telah diaugmentasi menggunakan teknik back-translation. Proyek ini bertujuan untuk meningkatkan kualitas terjemahan antara Bahasa Indonesia dan Bahasa Jawa, yang dinilai menggunakan metrik BLEU dan METEOR.

### Fitur Utama
- **Model Penerjemah dengan Attention:** Mendukung mekanisme Attention untuk menangkap konteks bahasa secara lebih efektif.
- **Augmentasi Data:** Menggunakan teknik back-translation untuk memperkaya dataset dan meningkatkan performa model.
- **Evaluasi Komprehensif:** Menggunakan BLEU dan METEOR untuk mengukur kualitas terjemahan.
- **Dukungan Bahasa Jawa:** Memanfaatkan standar Ngoko Alus untuk menjaga kelestarian bahasa daerah.

## Teknologi yang Digunakan
- **Python:** Bahasa pemrograman utama untuk membangun aplikasi ini.
- **TensorFlow/Keras:** Library deep learning untuk membangun dan melatih model RNN-LSTM.
- **Pandas/Numpy:** Untuk pengelolaan dan manipulasi data.
- **Matplotlib/Seaborn:** Untuk visualisasi data selama proses pelatihan.

## Langkah-Langkah Augmentasi dan Pelatihan
- **Augmentasi Data:**
  - Menggunakan back-translation (Bahasa Indonesia → Bahasa Inggris → Bahasa Indonesia).
  - Dataset akhir memiliki 15,000 pasang kalimat.
- **Pelatihan Model:**
  - Menggunakan mekanisme Attention Luong dan Bahdanau.
  - Penyetelan hyperparameter dilakukan dengan kombinasi batch size (128) dan epoch (150).
- **Evaluasi Model:**
  - Model terbaik (Attention Luong) mencapai skor BLEU 70.17% dan METEOR 89.61%.

## Evaluasi
- Model dengan mekanisme Attention secara signifikan lebih baik dibandingkan model tanpa Attention.
- Augmentasi data terbukti meningkatkan performa dengan memperkaya variasi struktur kalimat.
- Tantangan utama adalah perulangan kata di akhir kalimat, yang perlu diatasi dengan penyempurnaan dataset dan mekanisme Attention.

## Kesimpulan
Proyek ini berhasil meningkatkan kualitas terjemahan antara Bahasa Indonesia dan Bahasa Jawa menggunakan model RNN-LSTM dengan mekanisme Attention. Penelitian ini menunjukkan pentingnya augmentasi data dan hyperparameter tuning dalam meningkatkan performa model. Untuk penelitian lebih lanjut, disarankan untuk:
- Menyempurnakan mekanisme Attention guna mengurangi kesalahan perulangan kata.
- Memperbaiki konsistensi dataset untuk hasil prediksi yang lebih baik.

## Lisensi
Program ini dilisensikan di bawah GNU General Public License v3.0. Anda bebas untuk menggunakan, memodifikasi, dan mendistribusikan ulang program ini selama mengikuti ketentuan lisensi.

## Kontributor
Muhammad Raihan Khoirudin - Mahasiswa Program Studi S1 Informatika, Universitas Telkom Bandung.
Dibimbingan oleh: Dr. Arie Ardiyanti Suryani, S.T., M.T. & Bunyamin, M.Kom.
