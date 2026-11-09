# Kantong Berita 📱

**Aplikasi mobile berita berbasis Android yang terintegrasi dengan website Kantong Berita melalui WordPress REST API.**

Kantong Berita dikembangkan sebagai alternatif platform distribusi berita digital yang memungkinkan pengguna membaca berita melalui perangkat mobile, memilih kategori berita sesuai minat, menyimpan artikel, serta menerima notifikasi berita terbaru.

## 📌 Tentang Proyek

Proyek ini merupakan bagian dari tugas akhir (skripsi) Program Studi S-1 Teknik Informatika.

Aplikasi dikembangkan menggunakan Flutter dan Dart dengan memanfaatkan WordPress sebagai backend dan sistem pengelolaan konten yang sudah tersedia. Pengembangan dilakukan tanpa membangun backend baru, sehingga aplikasi mobile dan website tetap menggunakan sumber data yang sama.

## ✨ Fitur Utama

- **Authentication** — Registrasi dan login pengguna.
- **Guest Mode** — Mengakses berita tanpa login.
- **News Feed** — Menampilkan berita dari website Kantong Berita.
- **Category Preferences** — Memilih kategori berita sesuai minat pengguna.
- **News Detail** — Membaca detail artikel berita.
- **Bookmark** — Menyimpan berita untuk dibaca kembali.
- **Push Notification** — Menerima notifikasi berita terbaru.
- **Comments** — Berinteraksi melalui komentar pada artikel.
- **Dark Mode** — Mendukung tampilan terang dan gelap.
- **Search** — Mencari berita berdasarkan kata kunci.

## 🛠️ Tech Stack

| Teknologi | Penggunaan |
|---|---|
| Flutter | Framework pengembangan aplikasi mobile |
| Dart | Bahasa pemrograman |
| WordPress CMS | Pengelolaan konten berita |
| WordPress REST API | Komunikasi aplikasi dengan server |
| MySQL | Basis data yang digunakan oleh WordPress |
| Firebase Cloud Messaging (FCM) | Push notification |
| Git & GitHub | Version control dan pengelolaan kode |

## 🏗️ Arsitektur Sistem

```text
┌─────────────────────────────┐
│      Flutter Android       │
│        Kantong Berita      │
└──────────────┬──────────────┘
               │
               │ HTTPS / JSON
               ▼
┌─────────────────────────────┐
│     WordPress REST API     │
│       Custom Endpoint      │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│      WordPress CMS         │
│       MySQL Database       │
└─────────────────────────────┘

┌─────────────────────────────┐
│ Firebase Cloud Messaging   │
│       Push Notification    │
└─────────────────────────────┘
```

WordPress digunakan sebagai backend utama untuk pengelolaan berita dan data pengguna. Aplikasi mobile mengambil dan mengirimkan data melalui REST API, sedangkan Firebase Cloud Messaging mendukung fitur push notification.

## 🧪 Testing & Quality Assurance

Pengujian dilakukan untuk mengevaluasi fungsionalitas dan usability aplikasi.

### Black Box Testing

Pengujian dilakukan berdasarkan kebutuhan dan skenario penggunaan aplikasi tanpa melihat implementasi kode internal.

| Hasil Pengujian | Jumlah |
|---|---:|
| Total test case | 20 |
| Test case berhasil | 20 |
| Test case gagal | 0 |
| Tingkat keberhasilan | 100% |

### System Usability Scale (SUS)

Evaluasi usability dilakukan menggunakan System Usability Scale (SUS) dengan melibatkan 15 responden.

| Parameter | Hasil |
|---|---:|
| Jumlah responden | 15 |
| Skor SUS | 82,17 |
| Grade | A |
| Interpretasi | Excellent |

Hasil tersebut menunjukkan bahwa aplikasi memperoleh tingkat usability yang baik berdasarkan evaluasi SUS.

## 🔄 Development Methodology

Pengembangan aplikasi menggunakan metode **Agile Software Development**, dengan tahapan:

1. Planning
2. Design
3. Development
4. Testing
5. Deployment
6. Review
7. Launch

Metode ini digunakan untuk mendukung proses pengembangan secara bertahap dan menyesuaikan kebutuhan sistem.

## 🚀 Getting Started

### Prerequisites

Pastikan perangkat pengembangan telah memiliki:

- Flutter SDK
- Dart SDK
- Android Studio atau Visual Studio Code
- Android SDK
- Git

### Installation

1. Clone repository:

   ```bash
   git clone <repository-url>
   ```

2. Masuk ke direktori proyek:

   ```bash
   cd KantongBerita
   ```

3. Install dependencies:

   ```bash
   flutter pub get
   ```

4. Jalankan aplikasi:

   ```bash
   flutter run
   ```

> **Catatan:** Sesuaikan nama direktori dengan nama repository yang digunakan.

### Configuration

Aplikasi menggunakan WordPress REST API dan Firebase Cloud Messaging.

Sebelum menjalankan aplikasi, pastikan konfigurasi API dan Firebase telah disiapkan sesuai kebutuhan proyek.

**Jangan mengunggah API key, token autentikasi, file kredensial Firebase, atau informasi sensitif lainnya ke repository publik.**

## 👨‍💻 Project Information

| Informasi | Detail |
|---|---|
| Project | Kantong Berita |
| Platform | Android |
| Framework | Flutter |
| Language | Dart |
| Backend | WordPress REST API |
| Methodology | Agile Software Development |
| Project Type | Final Project / Undergraduate Thesis |

### Team

- Xavier Claudio Sianturi
- M. Abdi Sopansyah
- Yuda Tryangga

**My Contribution:**  
`[Tambahkan peran dan kontribusi pribadi pada proyek ini]`

## 📄 Documentation

Proyek ini dikembangkan sebagai bagian dari tugas akhir dengan judul:

**Pengembangan Aplikasi Mobile Kantong Berita Berbasis Android**

Dokumentasi penelitian mencakup analisis kebutuhan, perancangan sistem, implementasi aplikasi, serta pengujian menggunakan Black Box Testing, Software Testing Metrics, dan System Usability Scale (SUS).

*Developed as part of an undergraduate thesis project in Informatics Engineering.*
