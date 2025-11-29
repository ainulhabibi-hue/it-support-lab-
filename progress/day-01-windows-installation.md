# Day 01 - Windows Installation Practice

Tanggal: 26 November 2025

---

## Tujuan
Melakukan instalasi Windows 10 di VirtualBox dan memahami pembuatan partisi disk.

---

## Tools
- VirtualBox
- Windows 10 ISO

---

## Spesifikasi VM
- RAM: 4 GB
- CPU: 2 core
- Storage: 50 GB

---

## Langkah
1. Membuat VM baru di VirtualBox
2. Menonaktifkan Unattended Installation
3. Menjalankan ISO Windows
4. Memilih install manual
5. Skip product key
6. Membuat partisi:
   - C: 30 GB (System)
   - D: 20 GB (Data)
7. Install Windows hingga selesai

---

## Masalah yang Ditemui

### Error:
Windows cannot read the product key setting from the unattended answer file

VM juga memaksa input username & password.

---

## Analisis
Error terjadi karena fitur Automated Setup (Unattended Installation) aktif dan konfigurasi rusak.

---

## Solusi
1. Hapus VM lama (Delete all files)
2. Buat VM baru
3. Disable Unattended Installation
4. Install Windows secara manual

---

## Hasil
✅ Windows berhasil terinstal  
✅ Partisi dibuat dengan benar  
✅ Tidak ada error lanjutan

---

## Catatan Pribadi
- Install manual lebih stabil untuk lab
- Pembagian partisi mempermudah manajemen data
- VM aman untuk eksperimen tanpa risiko sistem utama

---

✅ Status: Lab berhasil


