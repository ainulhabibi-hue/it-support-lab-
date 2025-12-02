# Day 04 - Basic Troubleshooting Lab (Windows)

Tanggal: 29 November 2025

---

## Tujuan
Melatih kemampuan mendeteksi dan memperbaiki masalah sistem Windows menggunakan tools bawaan serta mendokumentasikan proses troubleshooting secara rapi.

---

## Environment
- Guest OS: Windows 10 (VirtualBox)
- RAM: 4 GB
- CPU: 2 core

---

## Tools yang Digunakan
- Event Viewer (`eventvwr.msc`)
- Device Manager (`devmgmt.msc`)
- Services (`services.msc`)
- Command Prompt / PowerShell
- Task Manager

---

## Langkah Praktik

### 1. Cek Log Sistem (Event Viewer)
- Buka: `Run -> eventvwr.msc`
- Periksa: Windows Logs → System / Application
- Cari: Error / Warning dengan timestamp terbaru
- Catat Event ID dan deskripsi singkat

---
