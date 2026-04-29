# Seminar Registration App

**Nama**: Affari Rizky Febriansyah 
**NPM**: 24552011205  
**Kelas**: TIF RP 24C CID  
**Mata Kuliah**: Pemrograman Mobile – Android Studio  
**Minggu**: UTS – Pendaftaran Seminar  

---

## 📹 Link Video Penjelasan


Video berisi penjelasan:
- Halaman Login (validasi, kredensial hardcode)
- Halaman Utama / Home (sapaan user, tombol daftar seminar)
- Form Pendaftaran (semua field input)
- Validasi real-time (error langsung muncul saat mengetik)
- Dialog Konfirmasi (Ya / Tidak)
- Halaman Hasil (ringkasan data pendaftaran)

---

## 📱 Alur Aplikasi

```
Login / Register → Home → Form Pendaftaran → Dialog Konfirmasi → Halaman Hasil → Home
```

---

## 🔐 Akun Demo (Hardcode)

| Email | Password |
|---|---|
| admin@seminar.com | admin123 |
| mahasiswa@gmail.com | mahasiswa |
| user@test.com | password |

---

## ✅ Fitur yang Diimplementasikan

### 1. Halaman Login
- Validasi email (harus mengandung `@`)
- Validasi password (minimal 6 karakter)
- Real-time validation saat mengetik
- Autentikasi dengan data hardcode

### 2. Halaman Register
- Form registrasi (Nama, Email, Password)
- Real-time validation

### 3. Halaman Utama (Home)
- Menampilkan sapaan dengan nama user
- Tombol "Daftar Seminar"
- Tombol Logout

### 4. Form Pendaftaran
- **Nama Lengkap** – minimal 3 karakter
- **Email** – harus mengandung `@`
- **Nomor HP** – hanya angka, 10-13 digit, diawali `08`
- **Jenis Kelamin** – RadioButton (Laki-laki / Perempuan)
- **Pilihan Seminar** – Spinner dengan 7 pilihan seminar
- **Checkbox Persetujuan** – wajib dicentang
- **Real-time validation** di semua field teks

### 5. Dialog Konfirmasi
- Muncul setelah submit berhasil divalidasi
- Tombol "Ya" → lanjut ke halaman hasil
- Tombol "Tidak" → kembali ke form

### 6. Halaman Hasil
- Menampilkan: Nama, Email, No HP, Jenis Kelamin, Seminar
- Pesan "Pendaftaran Berhasil 🎉"
- Tombol kembali ke Home

---

## 🛠️ Tech Stack

- **Bahasa**: Kotlin
- **Min SDK**: 24 | **Target SDK**: 34
- **UI**: Material Design Components
- **ViewBinding**: ✅
- **Package**: `com.example.seminarapp`

---

## 📂 Struktur Project

```
app/src/main/
├── java/com/example/seminarapp/
│   ├── LoginActivity.kt
│   ├── RegisterActivity.kt
│   ├── HomeActivity.kt
│   ├── FormPendaftaranActivity.kt
│   └── HasilActivity.kt
└── res/
    ├── layout/
    │   ├── activity_login.xml
    │   ├── activity_register.xml
    │   ├── activity_home.xml
    │   ├── activity_form_pendaftaran.xml
    │   └── activity_hasil.xml
    ├── values/
    │   ├── colors.xml
    │   ├── strings.xml
    │   └── themes.xml
    └── drawable/
        └── spinner_background.xml
```
