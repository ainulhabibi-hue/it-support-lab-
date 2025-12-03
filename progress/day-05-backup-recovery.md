# Day 05 - Backup & Recovery Lab (Windows)

Tanggal: 30 November 2025

---

## Tujuan
Memahami pentingnya backup data, membuat cadangan, dan melakukan restore data pada Windows.

---

## Tools
- File Explorer
- Command Prompt / PowerShell
- VirtualBox Snapshot

---

## Aktivitas Praktik

### 1. Simulasi Data Penting
Langkah:
- Buat folder `C:\DataUji`
- Isi beberapa file teks

Tujuan:
- Simulasi data penting karyawan

---

### 2. Backup Manual (Copy Data)
Langkah:
- Copy `C:\DataUji` ke `D:\Backup`

Tujuan:
- Membuat backup sederhana

---

### 3. Backup via Command Line
Perintah:
```cmd
xcopy C:\DataUji D:\Backup /E /I /H
