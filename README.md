# ⚡ IqPOS Professional Edition

### `OFFLINE POINT OF SALE • RETAIL MANAGEMENT • LAN MULTI-CASHIER`

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&duration=2800&pause=900&color=00FF9C&center=true&vCenter=true&width=760&lines=IqPOS+Professional+Edition;Offline+POS+System;LAN+Multi-Cashier+Architecture;Sales+%7C+Inventory+%7C+Purchasing+%7C+Reports;Fast+%E2%80%A2+Lightweight+%E2%80%A2+Reliable+%E2%80%A2+Offline" alt="IqPOS Typing Animation" />

![Status](https://img.shields.io/badge/SYSTEM-READY-00ff9c?style=for-the-badge)
![Edition](https://img.shields.io/badge/EDITION-PROFESSIONAL-00e5ff?style=for-the-badge)
![Mode](https://img.shields.io/badge/MODE-100%25%20OFFLINE-9b5cff?style=for-the-badge)
![LAN](https://img.shields.io/badge/LAN-MULTI--CASHIER-ff00cc?style=for-the-badge)
![License](https://img.shields.io/badge/LICENSE-V3-00ff9c?style=for-the-badge)

**Aplikasi kasir offline untuk toko dan bisnis retail yang membutuhkan kecepatan, kontrol stok, transaksi yang tertib, dan operasional multi-kasir melalui jaringan LAN.**

</div>

---

## 🟢 SYSTEM STATUS

| Component | Status |
|---|---|
| 🧠 POS Core | `READY` |
| 💾 Database | `OFFLINE / LOCAL` |
| 🌐 LAN Server | `READY` |
| 🖥️ Multi-Cashier | `READY` |
| 🔐 License System | `V3` |
| 📦 Inventory | `READY` |
| 🛒 Sales | `READY` |
| 🛍️ Purchasing | `READY` |
| 📊 Reporting | `READY` |
| 💾 Backup / Restore | `READY` |

> **IqPOS dirancang untuk tetap dapat digunakan tanpa ketergantungan terhadap internet.**

---

# ⚡ ABOUT IQPOS

**IqPOS Professional Edition** adalah aplikasi **Point of Sale (POS) offline** yang dirancang untuk membantu toko dan bisnis retail mengelola aktivitas operasional sehari-hari.

IqPOS menggabungkan kebutuhan utama toko dalam satu sistem:

```text
┌──────────────────────────────────────────────────────────────┐
│                         IqPOS PRO                            │
├──────────────────────────────────────────────────────────────┤
│  🛒 PENJUALAN       → Transaksi & pembayaran                 │
│  📦 STOK            → Persediaan & mutasi                   │
│  🛍️ PEMBELIAN       → Supplier & pembelian                 │
│  👥 PELANGGAN       → Data customer                         │
│  🏭 SUPPLIER        → Data pemasok                          │
│  👨‍💼 USER           → Admin, kasir & hak akses              │
│  🕐 SHIFT           → Kontrol aktivitas kasir               │
│  📊 LAPORAN         → Monitoring & analisis                 │
│  🧮 STOCK OPNAME    → Penyesuaian stok                      │
│  🧾 FAKTUR          → Cetak & cetak ulang                   │
│  💾 BACKUP          → Backup & restore database             │
│  🌐 LAN             → Multi-terminal                       │
└──────────────────────────────────────────────────────────────┘
```

---

# 🚀 CORE FEATURES

## 🛒 01 — PENJUALAN

Fitur utama:

- Scan / input kode barang
- Pencarian barang
- Keranjang transaksi
- Perhitungan otomatis
- Harga jual
- Potongan harga pada transaksi
- Pelanggan
- Pembayaran dan kembalian
- Cetak faktur
- Riwayat transaksi
- Cetak ulang faktur
- Pembatalan sesuai hak akses
- Hold / Resume transaksi

### 🔥 Transaction Flow

```text
CUSTOMER
   │
   ▼
PILIH BARANG
   │
   ▼
SHOPPING CART
   │
   ▼
HARGA / DISKON
   │
   ▼
PAYMENT
   │
   ▼
SAVE TRANSACTION
   │
   ▼
INVOICE / STRUK
```

---

# ⏸️ HOLD / RESUME TRANSACTION

Saat toko ramai, kasir dapat menyimpan transaksi sementara dan melayani pelanggan lain.

```text
CUSTOMER A
    │
    ▼
┌───────────────┐
│   CART A      │
└───────┬───────┘
        │ HOLD
        ▼
┌──────────────────┐
│ PENDING TRANSACT │
└────────┬─────────┘
         │
         ├──────────────► CUSTOMER B
         │                    │
         │                    ▼
         │               TRANSACTION B
         │                    │
         │                    ▼
         │                   PAY
         │
         └──────────────► RESUME A
                              │
                              ▼
                            PAY A
```

Data transaksi tertunda dapat mempertahankan:

- Cabang / gudang
- Barang
- Qty
- Harga transaksi
- Pelanggan
- Waktu
- Kasir
- Isi keranjang

---

# 📦 02 — INVENTORY / STOCK MANAGEMENT

Modul stok mencakup:

- Master barang
- Kategori
- Satuan
- Harga jual
- Harga beli
- Stok
- Minimum stok
- Mutasi stok
- Penyesuaian stok
- Stock opname
- Pergerakan barang
- Riwayat perubahan stok

```text
             ┌──────────────┐
             │   BARANG     │
             └──────┬───────┘
                    │
       ┌────────────┼────────────┐
       ▼            ▼            ▼
   PEMBELIAN     PENJUALAN    MUTASI
       │            │            │
       ▼            ▼            ▼
    STOCK IN     STOCK OUT    ADJUSTMENT
       │            │            │
       └────────────┼────────────┘
                    ▼
             ┌──────────────┐
             │ STOCK AKHIR  │
             └──────────────┘
```

---

# 🧮 03 — STOCK OPNAME

```text
STOK SISTEM
     │
     ▼
STOK FISIK
     │
     ▼
SELISIH
     │
     ▼
PENYESUAIAN
```

Stock opname membantu mencocokkan jumlah stok pada sistem dengan kondisi fisik barang.

---

# 🛍️ 04 — PEMBELIAN

```text
SUPPLIER
   │
   ▼
PEMBELIAN
   │
   ▼
KERANJANG PEMBELIAN
   │
   ├── Barang
   ├── Qty
   ├── Harga Beli
   └── Supplier
   │
   ▼
SIMPAN PEMBELIAN
   │
   ▼
STOCK IN
   │
   ▼
DATABASE
```

Fitur:

- Supplier
- Pencarian barang
- Keranjang pembelian
- Qty pembelian
- Harga beli
- Total pembelian
- Riwayat pembelian
- Laporan pembelian
- Update stok

---

# 👥 05 — CUSTOMER MANAGEMENT

Data pelanggan dapat dikaitkan dengan transaksi sehingga histori transaksi lebih mudah ditelusuri.

```text
CUSTOMER
   │
   ├── Nama
   ├── Kontak
   └── Informasi pelanggan
          │
          ▼
      TRANSAKSI
          │
          ▼
    RIWAYAT BELANJA
```

---

# 🏭 06 — SUPPLIER MANAGEMENT

```text
SUPPLIER
   │
   ├── Identitas
   ├── Kontak
   └── Informasi supplier
          │
          ▼
       PEMBELIAN
          │
          ▼
       STOCK IN
```

---

# 👨‍💼 07 — USER & ACCESS CONTROL

```text
                    ┌──────────────┐
                    │    ADMIN     │
                    └──────┬───────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
         MASTER        LAPORAN       SETTINGS
             │
             ▼
        ┌───────────┐
        │   KASIR   │
        └─────┬─────┘
              ▼
          PENJUALAN
```

Hak akses membantu membatasi menu dan tindakan tertentu sesuai role pengguna.

---

# 🕐 08 — CASHIER / SHIFT

```text
LOGIN KASIR
     │
     ▼
BUKA SHIFT
     │
     ▼
TRANSAKSI
     │
     ├── Penjualan
     ├── Pembayaran
     └── Aktivitas kasir
     │
     ▼
TUTUP SHIFT
     │
     ▼
REKAP
```

---

# 🧾 09 — INVOICE & REPRINT

Fungsi:

- Cetak faktur
- Cetak ulang faktur
- Informasi toko
- Nomor faktur
- Detail barang
- Qty
- Harga
- Diskon
- Total
- Pembayaran
- Kembalian
- Informasi pelanggan

```text
RIWAYAT TRANSAKSI
        │
        ▼
   PILIH TRANSAKSI
        │
        ▼
  DETAIL TRANSAKSI
        │
        ▼
   CETAK ULANG
        │
        ▼
      FAKTUR
```

---

# 📜 10 — TRANSACTION HISTORY

Informasi yang dapat ditelusuri:

- Nomor transaksi
- Tanggal
- Kasir
- Pelanggan
- Detail barang
- Qty
- Total
- Pembayaran
- Status transaksi

```text
TODAY
 │
 ├── 08:01 → INV-0001
 ├── 08:13 → INV-0002
 ├── 08:25 → INV-0003
 ├── 09:02 → INV-0004
 └── ...
```

---

# 📊 11 — REPORTING

```text
                  ┌──────────────┐
                  │   REPORTS    │
                  └──────┬───────┘
                         │
       ┌─────────────────┼─────────────────┐
       ▼                 ▼                 ▼
   PENJUALAN         PEMBELIAN           STOK
       │                 │                 │
       └─────────────────┼─────────────────┘
                         ▼
                  ANALISIS BISNIS
```

Contoh laporan:

- Penjualan
- Pembelian
- Stok
- Riwayat transaksi
- Rugi / laba
- Arus kas
- Kas kecil
- Mutasi stok

---

# 💰 12 — FINANCIAL REPORT

### Rugi / Laba

```text
PENJUALAN
    │
    ▼
PENDAPATAN
    │
    ├── HPP
    ▼
LABA KOTOR
    │
    ├── BIAYA
    ▼
LABA / RUGI
```

### Arus Kas

```text
             CASH FLOW
                 │
       ┌─────────┴─────────┐
       ▼                   ▼
    CASH IN             CASH OUT
       │                   │
       └─────────┬─────────┘
                 ▼
            SALDO KAS
```

---

# 💵 13 — KAS KECIL

```text
KAS KECIL
   │
   ├── ATK
   ├── Transport
   ├── Operasional
   ├── Keperluan toko
   └── Pengeluaran lain
```

---

# 🌐 LAN MULTI-CASHIER

IqPOS Professional Edition mendukung beberapa terminal kasir melalui jaringan LAN lokal.

Tidak diperlukan koneksi internet untuk komunikasi antara server dan terminal selama perangkat berada pada jaringan lokal yang sama.

## 🖥️ SERVER → TERMINAL ARCHITECTURE

```text
                         ┌─────────────────────────────┐
                         │        IQPOS SERVER          │
                         │                             │
                         │  Flask / Python             │
                         │  Database                   │
                         │  Business Logic             │
                         │  License                    │
                         │  API                        │
                         └──────────────┬──────────────┘
                                        │
                           ┌────────────┴────────────┐
                           │        LOCAL LAN        │
                           └────────────┬────────────┘
                                        │
              ┌─────────────────────────┼─────────────────────────┐
              ▼                         ▼                         ▼
      ┌───────────────┐        ┌───────────────┐        ┌───────────────┐
      │   TERMINAL 01 │        │   TERMINAL 02 │        │   TERMINAL 03 │
      │     KASIR     │        │     KASIR     │        │     KASIR     │
      └───────────────┘        └───────────────┘        └───────────────┘
              │                         │                         │
              └─────────────────────────┼─────────────────────────┘
                                        ▼
                              ┌───────────────────┐
                              │  CENTRAL DATA     │
                              │  & TRANSACTION    │
                              └───────────────────┘
```

---

# ⚡ MULTI-TERMINAL FLOW

```text
                  ╔════════════════════════╗
                  ║      IQPOS SERVER      ║
                  ║        :PORT           ║
                  ╚═══════════╤════════════╝
                              │
                     ╔════════╧════════╗
                     ║       LAN       ║
                     ╚════════╤════════╝
                              │
          ┌───────────────────┼───────────────────┐
          ▼                   ▼                   ▼
     ┌─────────┐         ┌─────────┐         ┌─────────┐
     │ KASIR 1 │         │ KASIR 2 │         │ KASIR 3 │
     └────┬────┘         └────┬────┘         └────┬────┘
          │                   │                   │
          └───────────────────┼───────────────────┘
                              ▼
                    ┌────────────────────┐
                    │ CENTRAL DATABASE   │
                    └────────────────────┘
```

---

# 🟢 SERVER STATUS

Status server dapat dipantau melalui:

```text
Setting
   │
   ▼
Status Server
```

Panel status server memisahkan informasi teknis server dari pengaturan toko dan nota.

```text
┌────────────────────────────────────────────┐
│              STATUS SERVER                 │
├────────────────────────────────────────────┤
│ STATUS SERVER       ● SERVER AKTIF         │
│ ALAMAT LAN          192.168.x.x             │
│ PORT                xxxx                    │
│ TERMINAL AKTIF      x / x                   │
├────────────────────────────────────────────┤
│              STATUS LISENSI                │
│ PLAN                PROFESSIONAL            │
│ LICENSE ID          ****************        │
│ TERMINAL            x                       │
│ EXPIRY              YYYY-MM-DD              │
└────────────────────────────────────────────┘
```

---

# 🔐 LICENSE SYSTEM V3

IqPOS Professional Edition menggunakan sistem **License V3** dengan digital signature **Ed25519**.

```text
LICENSE
   │
   ├── Product
   ├── Edition
   ├── License ID
   ├── Customer
   ├── Machine ID
   ├── License Type
   ├── Plan
   ├── Terminal Limit
   ├── Expiry
   └── Application Version
```

## 🛡️ License Architecture

```text
                 DEVELOPER
                     │
                     │ PRIVATE KEY
                     ▼
              ┌──────────────┐
              │   LICENSE    │
              │   GENERATOR  │
              └──────┬───────┘
                     │
                     ▼
              ┌──────────────┐
              │   iqpos.lic  │
              └──────┬───────┘
                     ▼
              ┌──────────────┐
              │ IQPOS SERVER │
              │  PUBLIC KEY  │
              │    VERIFY    │
              └──────┬───────┘
                     ▼
                LICENSE OK
```

### Prinsip keamanan

```text
PRIVATE KEY
    │
    └── HANYA UNTUK DEVELOPER

PUBLIC KEY
    │
    └── DIGUNAKAN APLIKASI UNTUK VERIFIKASI

LICENSE FILE
    │
    └── DIGUNAKAN SERVER
```

> **Private key generator tidak boleh dibagikan kepada pelanggan.**

---

# 💻 MACHINE ID

Lisensi server dikaitkan dengan identitas perangkat server.

```text
┌─────────────────────┐
│     SERVER PC       │
├─────────────────────┤
│ Machine Identity    │
│        ↓            │
│     MACHINE ID      │
└──────────┬──────────┘
           ▼
      LICENSE V3
           ▼
      VALID / INVALID
```

---

# 🖥️ LICENSE & TERMINALS

Lisensi berlaku pada **server**.

Terminal kasir yang terhubung ke server melalui LAN tidak perlu memiliki file lisensi sendiri.

```text
                 LICENSE
                    │
                    ▼
            ┌───────────────┐
            │ IQPOS SERVER  │
            └───────┬───────┘
                    │
          ┌─────────┼─────────┐
          ▼         ▼         ▼
       KASIR 1   KASIR 2   KASIR 3
          │         │         │
          └─────────┼─────────┘
                    ▼
              LICENSE SERVER
                 AUTHORITY
```

Jumlah terminal mengikuti batas terminal pada lisensi.

---

# 📁 APPLICATION DATA

Contoh lokasi data Windows:

```text
C:\ProgramData└── IqPOS    │
    ├── data    │   └── iqpos.db
    │
    └── license        ├── iqpos.lic
        ├── trial.dat
        ├── .trial_integrity
        └── .session_secret
```

Data aplikasi dipisahkan dari folder instalasi agar lebih mudah dikelola dan tetap tersedia ketika aplikasi diperbarui.

---

# 💾 BACKUP & RESTORE

```text
┌──────────────────────┐
│       DATABASE       │
└──────────┬───────────┘
           ▼
     ┌─────┴─────┐
     ▼           ▼
   BACKUP      SQL DUMP
     │           │
     └─────┬─────┘
           ▼
       STORAGE
           ▼
        RESTORE
```

Rekomendasi:

- Backup sebelum upgrade
- Backup setelah perubahan besar
- Backup sebelum restore
- Backup secara berkala

> **Data toko lebih penting daripada aplikasi.**

---

# 🛠️ MAINTENANCE

```text
DATABASE
   │
   ├── BACKUP
   ├── RESTORE
   ├── SQL DUMP
   └── MAINTENANCE
```

Akses maintenance sebaiknya dibatasi untuk administrator.

---

# 🏪 STORE & RECEIPT SETTINGS

```text
┌──────────────────────────────┐
│       INFORMASI TOKO         │
├──────────────────────────────┤
│ Nama Toko                    │
│ Alamat                       │
│ Telepon                      │
│ Informasi Nota               │
│ Format Cetak                 │
└──────────────────────────────┘
```

Pengaturan toko dan nota dipisahkan dari **Status Server** agar informasi operasional dan teknis tidak bercampur.

---

# 🧩 SYSTEM MODULE MAP

```text
                         IQPOS PRO
                             │
       ┌─────────────────────┼─────────────────────┐
       ▼                     ▼                     ▼
    TRANSAKSI              MASTER               REPORT
       │                     │                     │
 ┌─────┼─────┐       ┌──────┼──────┐       ┌──────┼──────┐
 ▼     ▼     ▼       ▼      ▼      ▼       ▼      ▼      ▼
SALE  HOLD  REPRINT ITEM CATEGORY SUPPLIER SALES STOCK FINANCE
       │
       ▼
   PURCHASING
       │
       ▼
     STOCK
       │
       ▼
 STOCK OPNAME
```

---

# 🧠 SYSTEM CONCEPT

```text
        SIMPLE
          │
          ▼
       FAST
          │
          ▼
       STABLE
          │
          ▼
       OFFLINE
          │
          ▼
     OPERATIONAL
```

IqPOS diarahkan menjadi sistem operasional toko yang tetap ringan dan mudah digunakan.

---

# ⚙️ TECHNOLOGY STACK

```text
┌────────────────────────────────────┐
│             IQPOS STACK            │
├────────────────────────────────────┤
│ Backend       Python / Flask       │
│ Frontend      HTML / CSS / JS      │
│ Database      SQLite               │
│ Network       Local LAN            │
│ Packaging     PyInstaller          │
│ Installer     Inno Setup           │
│ License       Ed25519 / V3         │
└────────────────────────────────────┘
```

---

# 🖥️ WINDOWS DEPLOYMENT

```text
SOURCE CODE
     │
     ▼
PYTHON BUILD
     │
     ▼
PYINSTALLER
     │
     ▼
IqPOS.exe
     │
     ▼
INSTALLER
     │
     ▼
IqPOS_Setup.exe
     │
     ▼
WINDOWS CLIENT
```

---

# 🔨 BUILD IQPOS

```text
BUILD_IQPOS
     │
     ▼
Python 3.8 x86
     │
     ▼
Virtual Environment
     │
     ▼
Dependencies
     │
     ▼
PyInstaller
     │
     ▼
IqPOS.exe
     │
     ▼
Inno Setup
     │
     ▼
IqPOS_Setup.exe
```

Output:

```text
dist└── IqPOS.exe

output└── IqPOS_Setup.exe
```

---

# 🔑 BUILD LICENSE GENERATOR

```text
genlic.py
    │
    ▼
PyInstaller
    │
    ▼
GenLic.exe
```

Output:

```text
developer_output└── GenLic.exe
```

### ⚠️ SECURITY WARNING

`GenLic.exe` mengandung **private key** yang digunakan untuk menandatangani lisensi.

```text
┌──────────────────────────────────────────────┐
│                  WARNING                     │
├──────────────────────────────────────────────┤
│ GenLic.exe TIDAK untuk diberikan kepada      │
│ pelanggan.                                   │
│                                              │
│ Private key harus tetap berada pada           │
│ lingkungan developer.                        │
└──────────────────────────────────────────────┘
```

---

# 📦 PROJECT BUILD OUTPUT

```text
PROJECT
│
├── dist│   └── IqPOS.exe
│
├── developer_output│   └── GenLic.exe
│
└── output    └── IqPOS_Setup.exe
```

Installer pelanggan **tidak perlu memasukkan `GenLic.exe`**.

---

# 🚀 INSTALLATION FLOW

```text
                  IqPOS_Setup.exe
                         │
                         ▼
                ┌────────────────┐
                │ INSTALL IQPOS  │
                └───────┬────────┘
                        ▼
                 START APPLICATION
                        ▼
                 MACHINE ID SERVER
                        ▼
                  LICENSE CHECK
                        │
             ┌──────────┴──────────┐
             ▼                     ▼
          LICENSE OK           TRIAL MODE
             │
             ▼
           SERVER
             │
             ▼
        CONNECT LAN
             │
       ┌─────┼─────┐
       ▼     ▼     ▼
     POS 1 POS 2 POS 3
```

---

# 🧪 TRIAL MODE

```text
INSTALL
   │
   ▼
TRY IQPOS
   │
   ├── Penjualan
   ├── Stok
   ├── Pembelian
   ├── Laporan
   └── Multi-Terminal
   │
   ▼
EVALUASI
   │
   ▼
ACTIVATE LICENSE
```

---

# 🔐 LICENSE TYPES

```text
┌──────────────────────────────┐
│          LICENSE             │
├──────────────────────────────┤
│ TRIAL                        │
│ PROFESSIONAL / PRO           │
│ LIFETIME                     │
└──────────────────────────────┘
```

---

# 🧱 SECURITY MODEL

```text
                    LICENSE FILE
                         │
                         ▼
                 FORMAT VALIDATION
                         │
                         ▼
                 SIGNATURE VERIFY
                         │
                         ▼
                   MACHINE ID
                         │
                         ▼
                  PRODUCT CHECK
                         │
                         ▼
                  EDITION CHECK
                         │
                         ▼
                 VERSION RANGE
                         │
                         ▼
                 TERMINAL LIMIT
                         │
                         ▼
                    EXPIRY
                         │
                         ▼
                    LICENSE OK
```

---

# 📡 SERVER MONITORING

```text
TERMINAL
   │
   │ heartbeat / server info
   ▼
SERVER
   │
   ├── Server status
   ├── LAN address
   ├── Port
   ├── Active terminals
   └── License status
```

---

# 🎯 DESIGN PHILOSOPHY

### ⚡ FAST
Antarmuka dibuat untuk aktivitas kasir yang cepat.

### 🪶 LIGHTWEIGHT
Tidak diarahkan menjadi sistem yang terlalu berat untuk toko kecil dan menengah.

### 📴 OFFLINE FIRST
Operasional dasar tidak bergantung pada koneksi internet.

### 🌐 LAN READY
Beberapa terminal dapat menggunakan server lokal melalui LAN.

### 🔐 CONTROLLED
Hak akses, user, shift dan lisensi membantu menjaga kontrol operasional.

### 💾 DATA OWNERSHIP
Database lokal memberikan kontrol langsung terhadap data operasional toko.

---

# 📈 OPERATIONAL WORKFLOW

```text
                    STORE
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
       SUPPLIER     CUSTOMER     ADMIN
          │           │           │
          ▼           ▼           ▼
      PEMBELIAN    PENJUALAN    CONTROL
          │           │
          ▼           ▼
       STOCK IN    STOCK OUT
          │           │
          └───────────┼───────────┘
                      ▼
                  DATABASE
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
       REPORTS     FINANCE     STOCK OPNAME
```

---

# 🗺️ FEATURE MATRIX

| Module | Function |
|---|---|
| 🛒 Penjualan | Transaksi kasir |
| ⏸️ Hold | Menyimpan transaksi sementara |
| ▶️ Resume | Melanjutkan transaksi tertunda |
| 🧾 Faktur | Cetak dokumen transaksi |
| 🔁 Reprint | Cetak ulang transaksi |
| 📜 History | Riwayat transaksi |
| 📦 Barang | Master inventory |
| 🧮 Stock Opname | Penyesuaian stok fisik |
| 🛍️ Pembelian | Barang masuk |
| 👥 Pelanggan | Customer management |
| 🏭 Supplier | Supplier management |
| 👨‍💼 User | User & access control |
| 🕐 Shift | Kontrol shift kasir |
| 💰 Kas Kecil | Pengeluaran operasional |
| 📊 Laporan | Reporting |
| 📈 Rugi/Laba | Financial analysis |
| 💵 Arus Kas | Cash flow |
| 💾 Backup | Database backup |
| ♻️ Restore | Database restore |
| 🌐 LAN | Multi-terminal |
| 🔐 License V3 | License verification |
| 🖥️ Server Status | Monitoring server |

---

# 🏆 WHY IQPOS?

```text
                    ┌─────────────────┐
                    │     IQPOS       │
                    └────────┬────────┘
                             │
          ┌──────────────────┼──────────────────┐
          ▼                  ▼                  ▼
       OFFLINE             LAN              LIGHTWEIGHT
          │                  │                  │
          └──────────────────┼──────────────────┘
                             ▼
                       STORE READY
```

IqPOS cocok untuk kebutuhan toko yang membutuhkan:

- Sistem kasir offline
- Pengelolaan stok
- Pengelolaan pembelian
- Beberapa kasir
- Kontrol user
- Laporan operasional
- Database lokal
- Backup mandiri
- Sistem lisensi terkontrol

---

# 🔮 DEVELOPMENT ROADMAP

```text
        CURRENT
           │
           ▼
   ┌────────────────┐
   │ CORE POS       │
   └───────┬────────┘
           ▼
   ┌────────────────┐
   │ INVENTORY      │
   └───────┬────────┘
           ▼
   ┌────────────────┐
   │ MULTI-CASHIER  │
   └───────┬────────┘
           ▼
   ┌────────────────┐
   │ FINANCIAL      │
   └───────┬────────┘
           ▼
   ┌────────────────┐
   │ OPERATIONAL    │
   │ RETAIL SYSTEM  │
   └────────────────┘
```

Fokus pengembangan:

- Stabilitas
- Kecepatan transaksi
- Keamanan data
- Kemudahan penggunaan
- Kontrol stok
- Kontrol kasir
- Reporting
- Multi-terminal
- Kemudahan maintenance

---

# 🧑‍💻 FOR DEVELOPERS

## Development Environment

```text
Windows
   │
   ├── Python 3.8 x86
   ├── Virtual Environment
   ├── Flask
   ├── SQLite
   ├── Cryptography
   ├── PyInstaller
   └── Inno Setup
```

## Conceptual Project Structure

```text
IqPOS/
│
├── app.py
├── genlic.py
│
├── templates/
│   └── index.html
│
├── data/
│   └── iqpos.db
│
├── license/
│   └── iqpos.lic
│
├── dist/
│   └── IqPOS.exe
│
├── developer_output/
│   └── GenLic.exe
│
└── output/
    └── IqPOS_Setup.exe
```

---

# 🛡️ BACKUP STRATEGY

```text
                    DATABASE
                       │
                       ▼
                 ┌───────────┐
                 │   BACKUP  │
                 └─────┬─────┘
                       │
              ┌────────┼────────┐
              ▼        ▼        ▼
            LOCAL    EXTERNAL   NAS
              │        │        │
              └────────┼────────┘
                       ▼
                  SAFE STORAGE
```

---

# ⚠️ IMPORTANT NOTES

1. Jangan menghapus database sembarangan.
2. Backup sebelum upgrade.
3. `GenLic.exe` bersifat developer-only.
4. Simpan private key dengan aman.
5. Gunakan server yang stabil untuk mode LAN.

---

# 🧪 QUALITY CHECK

```text
[✓] Application startup
[✓] Login
[✓] License validation
[✓] Machine ID
[✓] Server status
[✓] LAN connection
[✓] Cashier login
[✓] Sales transaction
[✓] Payment
[✓] Invoice printing
[✓] Reprint invoice
[✓] Hold transaction
[✓] Resume transaction
[✓] Purchase
[✓] Stock update
[✓] Stock opname
[✓] Transaction history
[✓] Reports
[✓] Backup
[✓] Restore
[✓] User permissions
[✓] Multi-terminal
```

---

# 🚀 QUICK START

### 1. Install

```text
IqPOS_Setup.exe
```

### 2. Jalankan IqPOS

```text
IqPOS.exe
```

### 3. Login

Gunakan user yang tersedia pada instalasi.

### 4. Konfigurasi toko

```text
Setting
   └── Pengaturan Nota & Toko
```

### 5. Cek server

```text
Setting
   └── Status Server
```

### 6. Hubungkan terminal

Pastikan komputer kasir berada pada jaringan LAN yang sama dengan server.

### 7. Mulai transaksi

```text
PENJUALAN
   ↓
BARANG
   ↓
KERANJANG
   ↓
PEMBAYARAN
   ↓
CETAK FAKTUR
```

---

# 🌐 LAN DEPLOYMENT EXAMPLE

```text
                   ROUTER / SWITCH
                         │
             ┌───────────┼───────────┐
             ▼           ▼           ▼
       ┌──────────┐ ┌──────────┐ ┌──────────┐
       │ SERVER   │ │ KASIR 01 │ │ KASIR 02 │
       │ IQPOS    │ │          │ │          │
       └────┬─────┘ └──────────┘ └──────────┘
            │
            ▼
       ┌──────────┐
       │ KASIR 03 │
       └──────────┘
```

---

# 🔥 THE IQPOS ECOSYSTEM

```text
                    ╔══════════════════╗
                    ║      IQPOS       ║
                    ║  PROFESSIONAL    ║
                    ╚════════╤═════════╝
                             │
          ┌──────────────────┼──────────────────┐
          ▼                  ▼                  ▼
      TRANSACTION         INVENTORY          FINANCE
          │                  │                  │
          ├── SALES          ├── STOCK         ├── P&L
          ├── HOLD           ├── OPNAME        ├── CASH FLOW
          ├── RESUME         ├── MUTATION       └── CASH
          └── REPRINT        └── PURCHASE
                             │
                             ▼
                         REPORTING
                             │
                             ▼
                         DATABASE
                             │
                             ▼
                            LAN
                             │
              ┌──────────────┼──────────────┐
              ▼              ▼              ▼
           TERMINAL 1     TERMINAL 2     TERMINAL 3
```

---

# 💚 CORE PRINCIPLE

<div align="center">

```text
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║                    KEEP IT SIMPLE.                           ║
║                    KEEP IT FAST.                             ║
║                    KEEP IT LOCAL.                            ║
║                    KEEP DATA SAFE.                           ║
║                                                              ║
║                         IQPOS                                ║
║               OFFLINE • FAST • CONTROLLED                    ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

</div>

---

# 👨‍💻 DEVELOPED BY

<div align="center">

### **Muhamad Thoriq**

`IqPOS Professional Edition`

![Developer](https://img.shields.io/badge/DEVELOPER-MUHAMAD%20THORIQ-00ff9c?style=for-the-badge)
![Year](https://img.shields.io/badge/RELEASE-2026-00e5ff?style=for-the-badge)

**Built for real-world retail operations.**

</div>

---

# 📜 COPYRIGHT

```text
© 2026 Muhamad Thoriq
IqPOS Professional Edition

All rights reserved.
```

---

<div align="center">

## ⚡ IQPOS PRO

```text
[ SYSTEM ONLINE ]
[ DATABASE READY ]
[ SERVER READY ]
[ LAN READY ]
[ LICENSE V3 ]
[ POS READY ]
```

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=16&duration=3000&pause=1000&color=00FF9C&center=true&vCenter=true&width=650&lines=SYSTEM+READY...;READY+FOR+RETAIL+OPERATIONS;OFFLINE+%E2%80%A2+FAST+%E2%80%A2+RELIABLE;IQPOS+PROFESSIONAL+EDITION" alt="IqPOS Footer Animation" />

<br>

`████████████████████████████████████████████████████████`

### `END OF README`

</div>
