# Day 02 - Network Basic Lab (Windows)

Tanggal: 27 November 2025

---

## Tujuan
Memahami konfigurasi jaringan dasar di Windows dan melakukan pengecekan koneksi jaringan.

---

## Tools
- Windows 10 (VirtualBox)
- Command Prompt / PowerShell

---

## Masalah yang Ditemui

Saat mencoba koneksi awal:
Beberapa request mengalami RTO (Request Timed Out).

Namun setelah menjalankan:
- ipconfig
- ping ke IPv4 dan gateway

Koneksi kembali normal.

---

## Analisis

Masalah terjadi kemungkinan karena:
- Adapter jaringan VM belum sinkron
- DHCP lease belum refresh
- DNS transient issue

Setelah perintah ping dijalankan, koneksi kembali stabil.

---

## Solusi

Menjalankan:
- ipconfig
- ping gateway
- ping internet

Tidak diperlukan reset network.

---

## Catatan

Ping dapat membantu "memancing" refresh koneksi.
RTO tidak selalu berarti jaringan mati total.

---

## Aktivitas Praktik

### 1. Cek IP Address
Perintah:
```cmd
ipconfig
