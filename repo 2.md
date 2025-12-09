# Solusi Upload File Besar (>25MB)

**Masalah:**
Anda mendapat error *"Yowza, that’s a big file"* saat upload lewat website GitHub.
*   **Penyebab**: Website GitHub membatasi upload maksimal **25MB per file**.
*   **Solusi**: Gunakan **Terminal**. Lewat terminal, batasnya jauh lebih besar (**100MB per file**).

---

## Panduan Upload Lewat Terminal

Karena file audio Anda besar (WAV kualitas tinggi), Anda **WAJIB** menggunakan terminal.

### Langkah 1: Pastikan File Ada di Folder
Pastikan file audio (0a.wav, dst) sudah ada di dalam folder komputer Anda:
`c:\Users\Administrator\Desktop\app\rainflow\public\audio\...`

### Langkah 2: Edit .gitignore (PENTING)
Agar Git mau membaca file audio tersebut, kita harus "mengizinkan" file `.wav`.
1.  Buka file `.gitignore` di folder `rainflow`.
2.  Cari baris bertuliskan `*.wav`.
3.  **Hapus** baris tersebut.
4.  Simpan file.

### Langkah 3: Upload via Terminal
Buka terminal di folder `rainflow`, lalu ketik perintah ini:

```bash
# 1. Masukkan semua file (termasuk yang besar) ke antrean
git add .

# 2. Bungkus file (Proses ini mungkin agak lama jika filenya banyak)
git commit -m "Add High Quality Audio Files"

# 3. Kirim ke GitHub
git push
```

### Hasilnya
Tunggu proses upload selesai (tergantung kecepatan internet Anda).
Setelah selesai, cek di website GitHub. File audio Anda pasti sudah masuk, meskipun ukurannya lebih dari 25MB.

---

## Catatan Tambahan: Jika File > 100MB
Jika ada **SATU file** yang ukurannya lebih dari **100MB** (misal video panjang 1 jam), Git biasa akan menolak juga.
Anda harus menggunakan fitur khusus bernama **Git LFS (Large File Storage)**.

Tapi untuk file audio WAV durasi 5-10 menit (biasanya 50-80MB), cara terminal di atas **SUDAH PASTI BERHASIL**.

---

## ⚡ Template Script (One-Click Copy)

Salin kode di bawah ini, lalu paste ke terminal (Klik Kanan) untuk upload file audio sekaligus.

```bash
# 1. Masuk ke folder rainflow
cd rainflow

# 2. Masukkan semua file (termasuk audio) ke antrean
git add .

# 3. Bungkus dengan pesan commit
git commit -m "Add Audio Assets (Manual Upload)"

# 4. Kirim ke GitHub
git push
```

