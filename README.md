# Tugas-Kriptografi
============================================
Aplikasi Kriptografi AES-256 (CBC)
Tugas Mata Kuliah Keamanan Data
============================================

Program ini adalah aplikasi CLI sederhana untuk mengenkripsi dan mendekripsi
file menggunakan algoritma AES-256 dengan mode CBC.

1. Prasyarat (Requirements)
   - Python 3.x
   - Library `cryptography`
   
   Untuk instalasi library, jalankan:
   pip install cryptography

2. Cara Menjalankan Program
   Jalankan file Python melalui terminal:
   
   python kripto_app.py

3. Cara Penggunaan
   Program akan menampilkan menu:
   
   - Pilih '1' untuk Enkripsi:
     - Masukkan nama file input (misal: data.csv)
     - Masukkan nama file output (misal: data.enc)
     - Masukkan password (akan tersembunyi)
   
   - Pilih '2' untuk Dekripsi:
     - Masukkan nama file input (misal: data.enc)
     - Masukkan nama file output (misal: data_hasil.csv)
     - Masukkan password yang sama saat enkripsi
   
   - Pilih '0' untuk Keluar.

4. Alur Kerja Kriptografi
   - Algoritma: AES-256 (Kunci 256-bit)
   - Mode: CBC (Cipher Block Chaining)
   - Padding: PKCS#7
   - Key Derivation: PBKDF2 (SHA-256) dengan Salt 16-byte
     untuk mengubah password menjadi kunci 256-bit.
   
   Format file terenkripsi:
   [ SALT (16 bytes) | IV (16 bytes) | CIPHERTEXT ]

5. Catatan Penggunaan AI (Refleksi)
   [Jelaskan di sini bagaimana Anda menggunakan AI, misal:
   "Saya menggunakan Google Gemini untuk:
   - Membantu mengubah pseudocode ke kode Python `cryptography` yang fungsional.
   - Mendapatkan penjelasan tentang praktik terbaik penyimpanan Salt dan IV.
   - Membantu membuat skenario pengujian (edge case) sesuai KAK."]
