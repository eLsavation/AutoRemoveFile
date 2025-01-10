
# 🗑️ Script: Remove Files Older Than 3 Days

## Deskripsi 📜
Script ini digunakan untuk mencari dan menghapus file yang lebih tua dari 3 hari di direktori tertentu. Menggunakan perintah `find` untuk menemukan file berdasarkan waktu modifikasi, dan kemudian menghapusnya dengan perintah `rm`. 🧹

## Perintah 🔧

```bash
find /path/path/to/file* -mtime +3 -exec rm {} \;
```

## Penjelasan 👩‍💻👨‍💻

- `/path/path/to/file*`: Menentukan path direktori dan pola file yang akan dicari. Gantilah `/path/path/to/file*` dengan path direktori dan pola file yang sesuai. 📂
  
- `-mtime +3`: Menentukan bahwa hanya file yang memiliki waktu modifikasi **lebih dari 3 hari** yang akan ditemukan dan diproses. 🕒

- `-exec rm {} \;`: Perintah ini mengeksekusi perintah `rm` untuk menghapus setiap file yang ditemukan oleh `find`. `{}` mewakili file yang ditemukan, dan `\;` digunakan untuk menandakan akhir dari perintah `exec`. ❌

## Cara Penggunaan 🚀

1. Gantilah `/path/path/to/file*` dengan path dan pola file yang sesuai dengan kebutuhan Anda. 📍
2. Jalankan perintah di terminal. 💻
3. Semua file yang memenuhi kriteria (modifikasi lebih dari 3 hari) akan dihapus. ⚡

**Perhatian!** ⚠️: Script ini akan **menghapus file secara permanen**. Pastikan Anda sudah memeriksa file yang ingin dihapus sebelum menjalankan script ini. 🔍

## Catatan 📝
- Script ini **tidak dapat dipulihkan** setelah dijalankan. Gunakan dengan hati-hati! ⚠️
- Pastikan Anda memiliki izin yang sesuai untuk menghapus file di direktori yang ditentukan. 🔑
