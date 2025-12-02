# Day 04 - Basic Troubleshooting Lab (Windows)

Tanggal: 29 November 2025

---

## Tujuan
Melatih kemampuan mendeteksi dan memperbaiki masalah sistem Windows menggunakan tools bawaan.

---

## Tools
- Event Viewer
- Device Manager
- Services
- Command Prompt

---

## Aktivitas Praktik

### 1. Event Viewer (Log Check)
Langkah:
- Run → `eventvwr.msc`
- Windows Logs → System

Tujuan:
- Menemukan error, warning, dan failure

---

### 2. Device Manager (Driver Check)
Langkah:
- Run → `devmgmt.msc`
- Cek icon kuning / error

Tujuan:
- Memastikan driver normal

---

### 3. Services (Service Status)
Langkah:
- Run → `services.msc`
- Cek:
  - Windows Update
  - DHCP Client
  - Windows Defender

Tujuan:
- Monitoring service penting

---

### 4. System File Checker
Perintah:
```cmd
sfc /scannow
