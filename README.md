# Tugas Pengganti Mata Kuliah Sistem Operasi – IT-06-01

## Identitas

- **Nama**: Muhammad Habibie Ebham
- **NIM**: 1202210017
- **Kelas**: IT-06-01

---

## Deskripsi Umum

Repositori ini berisi tugas pengganti mata kuliah Sistem Operasi yang dikembangkan menggunakan Bash Script. Program ini menyediakan menu interaktif untuk menampilkan berbagai informasi sistem dan pengguna. Tampilan terminal dibuat lebih menarik dengan penggunaan warna, ASCII art, dan loading bar.

---

## Menu yang Diimplementasikan

Seluruh 7 menu utama berhasil diimplementasikan:

### 1. Waktu Saat Ini + Greetings

Menampilkan waktu real-time berdasarkan zona sistem (WIB/WITA/WIT) lengkap dengan hari, tanggal, jam, serta sapaan otomatis seperti “Selamat pagi”, “Selamat malam”, dll.

### 2. Isi Direktori

Menampilkan daftar isi direktori aktif dalam bentuk tabel (`ls -lah`) dengan pewarnaan terminal yang memudahkan identifikasi file.

### 3. Informasi Jaringan

Menyediakan informasi seperti:

- IP lokal
- Gateway dan subnet mask
- DNS server
- Status internet (`ping`)
- Koneksi aktif (via `nmcli`, opsional)
- Lokasi IP publik (via API `ipinfo.io`)

### 4. Detail Sistem Operasi

Informasi sistem lengkap:

- Distro Linux (`lsb_release`)
- Kernel & arsitektur (`uname`)
- CPU usage (`top`)
- RAM usage (`free`)
- Disk usage (`df`)

### 5. Estimasi Waktu Install OS

Menampilkan waktu filesystem root dibuat dengan `tune2fs` (butuh `sudo`), sebagai estimasi waktu instalasi OS pertama kali.

### 6. Informasi Pengguna

Detail pengguna saat ini:

- Username
- UID & GID
- Nama lengkap
- Shell default
- Home directory

### 0. Keluar Program

Menampilkan animasi penutup dan pesan pamit sebelum program keluar dengan aman.

---

## Cara Menjalankan

```bash
chmod +x sys_info.sh
./sys_info.sh
```

**Catatan:**

- Sebagian menu seperti waktu install OS memerlukan `sudo`.
- Pastikan `jq` dan `curl` tersedia untuk informasi IP publik.

---

## Dokumentasi Menu 
Daftar Isi – Daftar Menu & Keterangan Menu

![Cuplikan layar 2025-06-21 230907](https://github.com/user-attachments/assets/95264da5-e2a2-44bf-8873-a8b4c08b7857)


Menu 1 – Cek Waktu dan Tanggal System

![Cuplikan layar 2025-06-21 231156](https://github.com/user-attachments/assets/51baea1a-3fb0-4f9d-8e5b-1cb36e795054)


Menu 2 – Lihat isi Direktori saat ini

![Cuplikan layar 2025-06-21 231349](https://github.com/user-attachments/assets/48bb3bde-08d6-43ae-920f-7c687fffc3de)


Menu 5 – Estimasi tanggal instalasi OS

![image](https://github.com/user-attachments/assets/b4bc9cca-b32b-4877-9e04-cffa924ed225)


Menu 6 – Detail akun pengguna

![image](https://github.com/user-attachments/assets/c01345dd-e757-411b-822b-e022b33f799a)


Menu 0 – Keluar dari Aplikasi

![image](https://github.com/user-attachments/assets/cbca8fb2-01ef-4bd5-809d-59255295c71f)

Menu 3 – Analisa Jaringan & koneksi

![image](https://github.com/user-attachments/assets/637df254-cd83-4112-9f86-baa6899c1710)



---

## Deadline

Sabtu, 21 Juni 2025 pukul 23:59 WIB

---

## Terima Kasih

Program ini dibuat sebagai bentuk tanggung jawab akademik dan latihan penggunaan Bash di dunia nyata. Semoga bermanfaat dan inspiratif bagi pengembangan tugas lainnya.
