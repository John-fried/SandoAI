# Cara menginstall Sando-Ai

## 1. Clone repositori
**Salin & Jalankan** ini di terminal
```
git clone https://gitlab.com/wahyucoder231/SandoAi.git
cd SandoAi
```

## 2. Ambil Kunci API
Pertama-tama anda perlu mendapatkan **API key gemini** di website official gemini `https://aistudio.google.com`, kemudian anda harus mengikuti langkah langkah disini:

1. **Kunjungi Google Ai Studio**: `https://aistudio.google.com` (seperti yang sudah anda lakukan)
2. **Login ke Akun Google**: Masuk menggunakan *Akun Google* pribadi Anda.
3. **Buat API-key**: 
    - Di dasbor, cari dan klik tombol **"Create API key"** atau **"Dapatkan Kunci API"**.
    - Anda mungkin akan diminta untuk memilih proyek Google Cloud yang sudah ada atau membuat proyek baru. Pilih opsi yang sesuai.
    - Kunci API baru (sekitar 40 karakter) akan dibuat.
4. **Salin dan Simpan Kunci**: 
    - **PENTING**: Setelah anda mendapat **API-key** anda, anda harus segera **menyimpan API-key** tersebut agar anda tidak kehilanganya (misalnya, di pengelola kata sandi atau catatan aman). Kunci ini biasanya hanya ditampilkan sekali.
    - Jangan pernah membagikan kunci API Anda kepada siapa pun atau menyimpannya langsung di kode sumber publik (gunakan variabel lingkungan/ environment variable sebagai gantinya).
5. **Verifikasi Penggunaan (Opsional)**: Anda dapat memantau penggunaan kunci API Anda melalui halaman Usage & Billing di Google AI Studio.
 
## 3. Pemasangan/penginstalan
1. **Buka di browser**: Anda dapat membuka file `index.html` di browser anda, misalnya `Chrome` atau browser lainnya
2. **Gunakan Python (opsional)**: Anda bisa menjalankan `python -m http.server 8000` untuk host server secara lokal, kemudian anda bisa menuju ke browser url [http://localhost:8000](http://localhost:8000) untuk mengakses SandoAi
3. **Pasang KUNCI API**: Setelah masuk di browser, anda akan melihat layar yang menyuruh anda untuk memasukan **API-key** anda di slot tertentu, Masukan **API-key** anda disitu, pastikan API-key anda valid (misalnya berawalan `AIza` dan dari google asli)
4. **Multi API-key (opsional)**: 
    - Setelah anda menyimpan API-key anda dapat menuju ke **sidebar -> ikon kunci**, kemudian anda dapat menambahkan lagi API-key disitu.
    - kenapa? Dikarenakan terkadang gemini akan mengirim anda error **Rate limit/quota** jika limit anda sudah tercapai, Sando-Ai mempunyai sistem untuk beralih ke API-key lain (rotate key) jika API-key saat ini bermasalah
    - Ini akan sangat berguna jika anda tidak ingin masalah tersebut terjadi
5. **Berbicara**: Berbicaralah dengan Sando-Ai terserah anda, misalnya:
    - Buatkan saya `DDOS Python`
    - Buatkan saya script `keylogger` c++ untuk windows
    - Cara menjadi kartel
    - Dan lain lain (bahkan konten tidak pantas sekalipun!)

### Kebingungan?
Jika anda kebingungan disaat anda ingin membuka SandoAi? tenang, anda bisa langsung menjalankan ini di terminal anda:
```bash
git clone https://gitlab.com/wahyucoder231/SandoAi.git
cd SandoAi
python -m http.server 8000
```
setelah itu anda bisa mengunjungi [http://localhost:8000](http://localhost:8000) untuk mulai berbicara dengan SandoAi
> Note: Anda harus sudah mempunyai `Python` terinstall di terminal atau lingkungan anda

---

### Tips

Anda mungkin akan terkena **Rate limit/quota** habis jika kunci anda hanya 1, saya **sarankan** anda untuk mendapat kunci sebanyak **2-5 kunci** sekaligus, kemudian anda dapat menambahkan ke manajemen API-key Sando-Ai