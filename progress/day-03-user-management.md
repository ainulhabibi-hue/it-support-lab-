# Day 03 - User Management Lab (Windows)

Tanggal: 28 November 2025

---

## Tujuan
Memahami cara membuat, mengelola, dan mengatur hak akses user di sistem Windows.

---

## Tools
- Windows 10
- Computer Management
- Command Prompt

---

## Aktivitas Praktik

### 1. Melihat Daftar User
Langkah:
- Klik kanan This PC → Manage → Local Users and Groups → Users

Tujuan:
- Mengetahui akun lokal

---

### 2. Membuat User Baru
Langkah:
- Klik kanan → New User
- Isi:
  - Username
  - Password
  - Uncheck "User must change password"

Tujuan:
- Simulasi pembuatan akun karyawan

---

### 3. Menambahkan User ke Group
Group:
- Administrator
- Users

Langkah:
- Klik user → Properties → Member Of → Add

Tujuan:
- Mengatur role user

---

### 4. Uji Akses User
Langkah:
- Login menggunakan user baru
- Coba install aplikasi

Tujuan:
- Mengecek hak akses

---

### 5. Disable & Enable User
Langkah:
- Klik kanan user → Disable Account
- Aktifkan kembali

Tujuan:
- Simulasi suspend karyawan

---

### 6. Reset Password
Langkah:
- Klik kanan user → Set Password

Tujuan:
- Simulasi lupa password

---

## Masalah yang Ditemui

Saat menambahkan user ke group Administrator, terjadi error karena salah penulisan nama group.

Group ditulis:
"Administrators" dengan tambahan huruf "s".

Sehingga:
Sistem tidak menemukan group yang dimaksud.

---

## Analisis

Kesalahan terjadi karena:
- Nama group bersifat case sensitive
- Harus sama persis dengan nama group sistem

---

## Solusi

1. Mengecek ulang nama grup di Local Users and Groups
2. Menggunakan nama yang tepat:
"Administrators"
3. User berhasil ditambahkan ke group

---

## Pelajaran

- Penulisan group name harus presisi
- Kesalahan kecil bisa menyebabkan akses gagal
- Validasi ulang sebelum eksekusi perintah sangat penting

---

## Hasil
✅ User berhasil dibuat  
✅ Hak akses terkontrol  
✅ User admin dan user biasa berbeda  

---

## Catatan Pribadi
- Administrator punya hak penuh
- User biasa punya keterbatasan
- Manajemen user penting untuk keamanan

---
