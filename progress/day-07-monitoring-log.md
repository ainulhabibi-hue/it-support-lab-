# Day 07 – Monitoring & Log Analysis (Windows)

Tanggal: 02 Desember 2025

---

## Tujuan
Mempelajari cara memantau aktivitas sistem dan menganalisis log keamanan di Windows menggunakan Event Viewer dan tools bawaan.

---

## Tools
- Event Viewer
- Task Manager
- Resource Monitor
- Command Prompt

---

## Aktivitas Praktik

---

### 1. Buka Event Viewer
Langkah:
- Tekan `Win + R`
- Ketik: `eventvwr.msc`
- Masuk ke:
  - Windows Logs
    - Application
    - Security
    - System

Tujuan:
- Melihat aktivitas sistem dan keamanan OS.

---

### 2. Analisis Log Security
Buka:
- Windows Logs → Security

Fokus ke Event ID:
- 4624 → Login berhasil
- 4625 → Login gagal
- 4634 → Logout
- 4720 → User dibuat
- 4722 → Akun diaktifkan
- 4725 → Akun dinonaktifkan
- 4732 → User ditambahkan ke group Administrator

Tujuan:
- Mengenali aktivitas berisiko.

---

### 3. Simulasi Error Login (Testing)
Langkah:
- Logout
- Login menggunakan password salah 2-3 kali
- Cek kembali log Event ID 4625

Hasil:
- Sistem mencatat percobaan login gagal

---

### 4. Monitoring Real-Time System
Buka:
- Task Manager → Performance
- Resource Monitor

Pantau:
- CPU usage
- Memory
- Disk activity
- Network usage

Tujuan:
- Deteksi aktivitas abnormal.

---

### 5. Filter Log Keamanan
Langkah:
- Klik kanan Security
- Filter Current Log
- Masukkan Event ID: `4625`

Tujuan:
- Fokus ke insiden login gagal.

---

### 6. Export Log
Langkah:
- Klik kanan → Save All Events As
- Simpan file sebagai:
  `security-log-day07.evtx`

Tujuan:
- Dokumentasi insiden.

---

### 7. Command Line Log Inspection
Perintah:
cmd
'wevtutil qe Security /f:text /c:10'

Tujuan:
- Melihat 10 log terakhir melalui CLI.

---

## Masalah yang Ditemui

Saat menjalankan perintah:
wevtutil qe Security /f:text /c:10

Muncul error:
Access is denied.

Penyebab:
Command Prompt tidak dijalankan sebagai Administrator sehingga tidak memiliki izin membaca Security Log.

Solusi:
Menutup CMD lalu menjalankannya kembali dengan:
Right Click → Run as Administrator

Setelah CMD dijalankan sebagai Administrator, perintah berhasil dijalankan dan log dapat ditampilkan.

---

### Hasil

✅ Event log terbaca
✅ Misconfig/login error terdeteksi di Event Viewer
✅ Log berhasil difilter dan diekspor

---

### Catatan Pribadi

- Log adalah bukti utama aktivitas sistem.
- Security log penting bagi SOC.
- Event ID mempermudah investigasi.

---
