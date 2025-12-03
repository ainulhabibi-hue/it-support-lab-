# Day 06 - Basic Security Lab (Windows)

Tanggal: 01 Desember 2025

---

## Tujuan
Memahami pengamanan dasar Windows mencakup antivirus, firewall, update, dan kebijakan akun.

---

## Tools
- Windows Security
- Windows Defender Firewall
- Local Security Policy
- Command Prompt / PowerShell

---

## Aktivitas Praktik

### 1. Antivirus Check (Windows Defender)
Langkah:
- Settings → Update & Security → Windows Security → Virus & threat protection
- Pastikan Real-time protection = ON
- Jalankan Quick Scan

Tujuan:
- Memastikan sistem terlindungi malware.

---

### 2. Firewall Status
Langkah:
- Control Panel → Windows Defender Firewall
- Pastikan semua profile aktif:
  - Domain
  - Private
  - Public

---

### 3. Windows Update
Langkah:
- Settings → Windows Update
- Cek update terbaru

Tujuan:
- Menutup celah keamanan.

---

### 4. Password Policy
Langkah:
- Run → `secpol.msc`
- Account Policies → Password Policy
  - Minimum length: 8
  - Password must meet complexity: Enabled

Tujuan:
- Mencegah password lemah.

---

### 5. Account Lockout Policy
Langkah:
- Account Policies → Account Lockout Policy
  - Lockout after: 5 attempts

Tujuan:
- Mencegah brute force.

---

### 6. UAC (User Account Control)
Langkah:
- Control Panel → User Accounts → Change User Account Control settings
- Set minimal di level default

Tujuan:
- Mencegah eksekusi tanpa izin.

---

### 7. Cek Port Aktif
Perintah:
```cmd
netstat -an

Tujuan:
- Mengetahui port terbuka.

---

8. Disable Guest Account
Langkah:
Local Users and Groups → Guest → Disable

Tujuan:
- Mengurangi celah keamanan.

---
