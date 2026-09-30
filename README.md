# LAPORAN PRAKTIKUM DESAIN WEB A
## Pertemuan 1 & 2: Dasar-Dasar HTML

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Status](https://img.shields.io/badge/Status-Selesai-success)

---

## 📋 Identitas Praktikan

| | |
|---|---|
| **Nama** | Ilham Baihaqi |
| **NIM** | 4525210029 |
| **Program Studi** | Teknik Informatika |
| **Fakultas** | Teknik |
| **Universitas** | Universitas Pancasila |
| **Mata Kuliah** | Praktikum Desain Web A |
| **Pertemuan** | 1 & 2 |
| **Dosen / Asisten** | _(isi nama dosen/asisten)_ |

---

## 📑 Daftar Isi

1. [Tujuan Praktikum](#1-tujuan-praktikum)
2. [Dasar Teori](#2-dasar-teori)
3. [Alat dan Bahan](#3-alat-dan-bahan)
4. [Struktur Proyek](#4-struktur-proyek)
5. [Pembahasan dan Hasil](#5-pembahasan-dan-hasil)
6. [Rekap Tag HTML yang Digunakan](#6-rekap-tag-html-yang-digunakan)
7. [Cara Menjalankan](#7-cara-menjalankan)
8. [Kendala dan Evaluasi](#8-kendala-dan-evaluasi)
9. [Kesimpulan](#9-kesimpulan)
10. [Referensi](#10-referensi)

---

## 1. Tujuan Praktikum

Setelah melaksanakan praktikum ini, praktikan diharapkan mampu:

1. Memahami struktur dasar dokumen HTML5.
2. Menggunakan tag heading, paragraf, dan pemformatan teks.
3. Membuat berbagai jenis list (ordered, unordered, dan description list).
4. Menyisipkan gambar beserta atribut `alt`, `width`, dan `height`.
5. Membuat hyperlink internal (anchor), eksternal, dan `mailto`.
6. Menggunakan karakter khusus (HTML entities).
7. Menyusun sebuah halaman profil organisasi yang terstruktur dan mudah dinavigasi.

---

## 2. Dasar Teori

### 2.1 HTML
**HTML (HyperText Markup Language)** adalah bahasa markup standar untuk membuat halaman web. HTML menggunakan *tag* untuk menandai struktur dan makna dari konten, seperti judul, paragraf, gambar, dan tautan.

### 2.2 Struktur Dasar Dokumen HTML5
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Judul Halaman</title>
</head>
<body>
    <!-- Konten halaman -->
</body>
</html>
```

| Elemen | Fungsi |
|---|---|
| `<!DOCTYPE html>` | Menandakan bahwa dokumen menggunakan HTML5 |
| `<html lang="id">` | Elemen root, atribut `lang` menentukan bahasa dokumen |
| `<head>` | Berisi metadata (judul, encoding, viewport) |
| `<meta charset="UTF-8">` | Menentukan encoding karakter |
| `<body>` | Berisi seluruh konten yang tampil di browser |

### 2.3 Heading dan Teks
Heading `<h1>` sampai `<h6>` menyatakan tingkat judul, dengan `<h1>` yang terpenting. Paragraf ditulis dengan `<p>`, sedangkan pemformatan teks memakai `<strong>`, `<em>`, `<b>`, dan `<u>`.

### 2.4 List
- **Ordered list** (`<ol>`): daftar berurutan.
- **Unordered list** (`<ul>`): daftar tidak berurutan.
- **Description list** (`<dl>`, `<dt>`, `<dd>`): daftar istilah beserta deskripsinya.

### 2.5 Gambar
Gambar disisipkan dengan `<img src="..." alt="...">`. Atribut `alt` penting untuk aksesibilitas dan sebagai teks pengganti bila gambar gagal dimuat.

### 2.6 Hyperlink
- **Link internal (anchor)**: `<a href="#id">` menuju elemen ber-`id` di halaman yang sama.
- **Link eksternal**: `<a href="https://...">` menuju halaman lain.
- **Link email**: `<a href="mailto:alamat@email.com">` membuka aplikasi email.

### 2.7 Karakter Khusus (HTML Entities)
Karakter yang punya arti khusus di HTML ditulis dengan entity, misalnya `&lt;` (<), `&gt;` (>), `&copy;` (©), `&amp;` (&), dan `&mdash;` (—).

---

## 3. Alat dan Bahan

| Kategori | Keterangan |
|---|---|
| **Bahasa** | HTML5 |
| **Text Editor** | Visual Studio Code _(sesuaikan)_ |
| **Browser** | Google Chrome / Microsoft Edge _(sesuaikan)_ |
| **Version Control** | Git dan GitHub |
| **Aset Gambar** | `gedungtek.jpg`, `imatika.jpg`, `p.jpg` |

---

## 4. Struktur Proyek

```
Pertemuan1/
├── contohprogram.html   # Contoh program: profil mahasiswa
├── quiz.html            # Quiz: kontak & media sosial
├── tugasprak.html       # Tugas praktikum: profil organisasi IMATIKA
├── README.md            # Laporan praktikum
└── img/
    ├── gedungtek.jpg
    ├── imatika.jpg
    └── p.jpg
```

---

## 5. Pembahasan dan Hasil

### 5.1 Contoh Program: `contohprogram.html`

**Deskripsi:** Halaman profil mahasiswa sederhana untuk mengenal tag-tag dasar HTML.

**Potongan kode:**
```html
<h1>Profil Mahasiswa</h1>
<h2>Nama mahasiswa</h2>
<p>Saya mahasiswa yang sedang mempelajari <strong>Desain Web</strong>.</p>
<p>Minat saya adalah <em>UI Design</em>, HTML, dan CSS.</p>
<p>HTML menggunakan tag seperti &lt;p&gt; dan &lt;h1&gt;.</p>
<p>Hak cipta &copy; 2026 Fakultas Teknik Universitas Pancasila.</p>
```

**Penjelasan:**
| Bagian | Penjelasan |
|---|---|
| `<h1>`, `<h2>`, `<h3>` | Hierarki judul halaman |
| `<strong>` dan `<em>` | Teks tebal (penting) dan miring (penekanan) |
| `<b>` dan `<u>` | Teks tebal dan bergaris bawah (tampilan) |
| `<br>` | Pindah baris tanpa membuat paragraf baru |
| `&lt;` `&gt;` `&copy;` | Menampilkan karakter khusus sebagai teks biasa |

**Hasil tampilan:**

![Hasil contohprogram.html](screenshots/contohprogram.png)

---

### 5.2 Quiz: `quiz.html`

**Deskripsi:** Halaman kontak yang memuat tautan media sosial, alamat email, dan alamat kantor.

**Potongan kode:**
```html
<h1>Kontak &amp; Media Sosial</h1>
<h2>Media Sosial</h2>
<ul>
    <li><a href="https://github.com/IlhamBaihaqi24/">github : IlhamBaihaqi24</a></li>
</ul>

<h3>Email</h3>
<p>Kirim pertanyaan Anda ke email:
   <a href="mailto:ilhambhq378@gmail.com">ilhambhq378@gmail.com</a></p>
```

**Penjelasan:**
| Bagian | Penjelasan |
|---|---|
| `<ul>` + `<li>` | Daftar tautan media sosial (Instagram, GitHub, YouTube) |
| `<a href="https://...">` | Link eksternal ke profil media sosial |
| `<a href="mailto:...">` | Link yang membuka aplikasi email dengan alamat tujuan terisi |
| `<h4>` + `<p>` | Bagian alamat kantor |

**Hasil tampilan:**

![Hasil quiz.html](screenshots/quiz.png)

---

### 5.3 Tugas Praktikum: `tugasprak.html` (Profil Organisasi IMATIKA)

**Deskripsi:** Halaman profil organisasi **IMATIKA (Ikatan Mahasiswa Teknik Informatika)** yang terdiri dari empat bagian utama: Profil Organisasi, Bidang Keahlian, Cara Bergabung, dan Kontak & Media Sosial.

#### a. Navigasi Anchor Internal
```html
<nav>
  <a href="#profil">Profil</a> |
  <a href="#bidang-keahlian">Bidang Keahlian</a> |
  <a href="#cara-bergabung">Cara Bergabung</a> |
  <a href="#kontak">Kontak</a>
</nav>

<h2 id="profil">Profil Organisasi</h2>
```
Atribut `id` pada heading menjadi tujuan dari link `#...` di menu navigasi, sehingga pengunjung bisa berpindah bagian tanpa memuat ulang halaman.

#### b. Gambar dengan Atribut `alt`
```html
<img src="img/imatika.jpg" alt="Logo IMATIKA" width="300" height="300">
<img src="img/gedungtek.jpg" alt="Gedung Teknik" width="400" height="250">
```

#### c. Description List (`<dl>`)
```html
<dl>
  <dt>Nama Organisasi</dt>
  <dd>Ikatan Mahasiswa Teknik Informatika (IMATIKA)</dd>
  <dt>Status Akreditasi Program Studi</dt>
  <dd>A (Unggul)</dd>
</dl>
```

#### d. Ordered List (`<ol>`)
Digunakan untuk daftar bidang keahlian dan tahapan cara bergabung yang harus berurutan.
```html
<ol>
  <li>Mengisi formulir pendaftaran yang dibagikan melalui panitia</li>
  <li>Mengunggah KTM atau bukti registrasi ulang</li>
  <li>Mengikuti wawancara minat dan bakat</li>
  <li>Mengikuti masa orientasi anggota baru</li>
  <li>Penempatan bidang berdasarkan hasil wawancara</li>
  <li>Pelantikan sebagai anggota resmi IMATIKA</li>
</ol>
```

#### e. Unordered List (`<ul>`)
Digunakan untuk aktivitas rutin dan ketentuan umum calon anggota, yang tidak memerlukan urutan.

#### f. Link Eksternal dan Email
```html
<a href="https://www.instagram.com/imatika_ftkmup/" target="_blank">@imatika_ftkmup</a>
<a href="mailto:imatikaftkmup@gmail.com">imatikaftkmup@gmail.com</a>
```
Atribut `target="_blank"` membuka link eksternal di tab baru.

#### Ringkasan Pemenuhan Ketentuan Tugas

| Ketentuan | Implementasi | Status |
|---|---|---|
| Minimal 2 gambar dengan `alt` | Logo IMATIKA dan Gedung Teknik | ✅ |
| Link anchor internal | Menu navigasi ke 4 bagian halaman | ✅ |
| Link eksternal | Instagram dan website program studi | ✅ |
| Link email (`mailto`) | Email IMATIKA (di bagian kontak dan footer) | ✅ |
| 3 tipe list | `<ol>`, `<ul>`, dan `<dl>` | ✅ |

**Hasil tampilan:**

![Hasil tugasprak.html](img/ss1.png)

---

## 6. Rekap Tag HTML yang Digunakan

| Kategori | Tag |
|---|---|
| **Struktur** | `<!DOCTYPE>`, `<html>`, `<head>`, `<meta>`, `<title>`, `<body>` |
| **Heading** | `<h1>` – `<h4>` |
| **Teks** | `<p>`, `<br>`, `<hr>`, `<strong>`, `<em>`, `<b>`, `<u>`, `<small>` |
| **List** | `<ol>`, `<ul>`, `<li>`, `<dl>`, `<dt>`, `<dd>` |
| **Media** | `<img>` (`src`, `alt`, `width`, `height`) |
| **Link** | `<a>` (`href`, `target`, `id`) |
| **Navigasi** | `<nav>` |
| **Entity** | `&lt;` `&gt;` `&copy;` `&amp;` `&mdash;` |

---

## 7. Cara Menjalankan

1. **Clone repositori**
```bash
   git clone https://github.com/IlhamBaihaqi24/Prak_DW_A-Pertemuan-1-2.git
```
2. **Masuk ke folder proyek**
```bash
   cd Prak_DW_A-Pertemuan-1-2
```
3. **Buka file HTML di browser**, misalnya `tugasprak.html`, dengan klik dua kali atau memakai ekstensi *Live Server* di VS Code.

> ⚠️ Folder `img/` harus berada satu level dengan file HTML agar gambar tampil dengan benar.

