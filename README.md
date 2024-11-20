#Capstone Voice Processing
Proyek ini bertujuan untuk memproses data suara dari dataset Common Voice untuk keperluan normalisasi audio dan penggunaan data teks (TSV) dalam analisis lanjutan. Proses normalisasi memastikan konsistensi suara sebelum digunakan dalam aplikasi InstaHelp.

Fitur Utama
- Normalisasi Audio: Mengubah amplitudo file audio agar memiliki skala yang konsisten.
- Ekstraksi Metadata: Menggunakan file TSV dari dataset untuk memahami struktur data suara.

Struktur Proyek
Capstone voice/
│
├── normalized_clips/
│   └── normalize_audio.py        # Script Python untuk normalisasi audio
│
├── cv-corpus-19.0-2024-09-13/
│   ├── id/
│   │   ├── clips/                # Folder berisi file audio mentah (tidak diunggah)
│   │   ├── validated.tsv         # Metadata tentang file audio
│   │   └── ...                   # File lain dari dataset
│
└── README.md                     # Penjelasan proyek ini

Cara Menjalankan
1. Persiapan Lingkungan
Instalasi Dependensi: Pastikan Anda telah menginstal pustaka yang diperlukan:
pip install librosa soundfile
2. Dataset: Letakkan dataset Common Voice ke dalam folder cv-corpus-19.0-2024-09-13/id/clips.


File README.md biasanya digunakan untuk memberikan penjelasan tentang proyek Anda di GitHub. Dalam kasus proyek Anda (normalisasi audio dan penggunaan file TSV), isi README dapat mencakup:

Deskripsi Proyek: Jelaskan tujuan proyek Anda.
Langkah-langkah Implementasi: Berikan gambaran cara kerja kode Anda.
Cara Menjalankan Kode: Tambahkan langkah-langkah untuk menjalankan script.
Struktur File: Sebutkan file penting dan kegunaannya.
Kebutuhan Sistem: Sebutkan pustaka atau dependensi yang diperlukan.
Berikut adalah template yang bisa Anda gunakan:

Capstone Voice Processing
Proyek ini bertujuan untuk memproses data suara dari dataset Common Voice untuk keperluan normalisasi audio dan penggunaan data teks (TSV) dalam analisis lanjutan. Proses normalisasi memastikan konsistensi suara sebelum digunakan dalam aplikasi InstaHelp.

Fitur Utama
Normalisasi Audio: Mengubah amplitudo file audio agar memiliki skala yang konsisten.
Ekstraksi Metadata: Menggunakan file TSV dari dataset untuk memahami struktur data suara.
Struktur Proyek
bash
Salin kode
Capstone voice/
│
├── normalized_clips/
│   └── normalize_audio.py        # Script Python untuk normalisasi audio
│
├── cv-corpus-19.0-2024-09-13/
│   ├── id/
│   │   ├── clips/                # Folder berisi file audio mentah (tidak diunggah)
│   │   ├── validated.tsv         # Metadata tentang file audio
│   │   └── ...                   # File lain dari dataset
│
└── README.md                     # Penjelasan proyek ini

Cara Menjalankan
1. Persiapan Lingkungan
Instalasi Dependensi: Pastikan Anda telah menginstal pustaka yang diperlukan:
pip install librosa soundfile
2. Dataset: Letakkan dataset Common Voice ke dalam folder cv-corpus-19.0-2024-09-13/id/clips.

Menjalankan Script Normalisasi
- Navigasikan ke folder proyek:
cd "C:\Users\amali\OneDrive\Documents\Capstone voice"

- Aktifkan virtual environment (opsional):
.\instahelp_env\Scripts\activate

- Jalankan script:
python normalized_clips/normalize_audio.py

- Hasil file normalisasi akan tersimpan di folder normalized_clips.

Kebutuhan Sistem
Python: Versi 3.11
Pustaka Python:
librosa
soundfile
os
