Berikut adalah panduan untuk menginstal PostgreSQL dan Odoo di Windows, serta cara menjalankannya:

---

### **1. Menginstal PostgreSQL**
PostgreSQL adalah basis data yang digunakan Odoo untuk menyimpan data.

#### **Langkah-langkah:**
1. **Unduh PostgreSQL**
   - Kunjungi situs resmi PostgreSQL di [https://www.postgresql.org/download/](https://www.postgresql.org/download/).
   - Pilih versi untuk Windows dan unduh installer.

2. **Instal PostgreSQL**
   - Jalankan installer PostgreSQL yang telah diunduh.
   - Ikuti panduan instalasi:
     - Tentukan lokasi instalasi.
     - Atur username dan password untuk **user `postgres`** (penting untuk diingat karena akan digunakan untuk Odoo).
     - Pilih port default (5432).
   - Selesaikan instalasi.

3. **Verifikasi Instalasi**
   - Buka **pgAdmin** (GUI PostgreSQL) atau gunakan command prompt untuk memastikan PostgreSQL berjalan:
     ```bash
     psql -U postgres
     ```
   - Masukkan password yang telah dibuat sebelumnya.

---

### **2. Menginstal Odoo**
Odoo adalah aplikasi ERP yang dapat diinstal dan berjalan di atas PostgreSQL.

#### **Langkah-langkah:**
1. **Unduh Installer Odoo**
   - Kunjungi situs resmi Odoo di [https://www.odoo.com/page/download](https://www.odoo.com/page/download).
   - Pilih versi Odoo Community untuk Windows.

2. **Instal Odoo**
   - Jalankan installer Odoo yang telah diunduh.
   - Ikuti panduan instalasi:
     - Tentukan lokasi instalasi.
     - Masukkan detail PostgreSQL (host, port, username, password).
     - Selesaikan instalasi.

3. **Konfigurasi Odoo**
   - Setelah instalasi selesai, Odoo biasanya akan menginstal layanan yang dapat langsung dijalankan.

---

### **3. Menjalankan Odoo**
1. **Melalui Layanan Windows**
   - Tekan **Win + R**, ketik `services.msc`, lalu tekan **Enter**.
   - Cari layanan **Odoo Service**.
   - Klik kanan pada layanan, lalu pilih **Start**.

2. **Akses Odoo**
   - Buka browser dan akses:
     ```
     http://localhost:8069
     ```
   - Halaman Odoo akan muncul, dan Anda bisa mulai membuat database serta mengatur aplikasi Odoo.

---

### **Tips Tambahan**
- **Login Admin Default Odoo**: Ketika membuat database, Anda akan diminta membuat email dan password admin.
- **Plugin Tambahan**: Jika Anda membutuhkan modul tambahan, Anda bisa mendownloadnya dari Odoo Apps Store dan menambahkannya ke folder `addons`.

---

Jika Anda mengalami kendala, jangan ragu untuk bertanya lebih lanjut! 😊
