# PORRIDGE (Power Of Reading English)
> *"Every page, a spoonful of knowledge."*

=======================================================

Aplikasi latihan membaca bahasa Inggris interaktif dengan teks berjalan, pembacaan suara (Text-to-Speech), sorotan kata (highlight), terjemahan kosakata otomatis (Vocab), dan kuis pemahaman (Quiz). Seluruh menu di aplikasi memakai bahasa Inggris.

---

## 1. CARA PASANG
- Ekstrak zip ini di HP atau komputer. Hasilnya folder berisi: `index.html`, `manifest.json`, `sw.js`, `.nojekyll`, folder `icons`, dan folder `stories`.
- Di aplikasi web server kamu (misal XAMPP/Apache atau web server Android), pilih folder aplikasi ini sebagai root, lalu tekan **Start**.
- Buka Chrome, ketik `http://localhost:PORT` (port lihat di aplikasi server) atau buka lewat GitHub Pages. Pakai `localhost` (jangan alamat IP) agar bisa diinstal sebagai PWA.
- Buka Menu titik tiga Chrome -> **Instal aplikasi** / **Tambahkan ke layar utama**.
- Setelah terinstal, aplikasi tetap bisa dibuka secara offline walau servernya mati.

---

## 2. TAMBAH / UPDATE CERITA
- **Lewat Folder Stories**:
  - Taruh file `.md` baru di folder `stories/`, lalu buka aplikasinya (atau tekan **Reload stories**).
  - Ganti isi file `.md` yang sudah ada = cerita ikut terupdate otomatis.
  - Hapus file `.md` = cerita otomatis hilang dari daftar.
- **Lewat Tombol "Add" di Aplikasi**:
  - Tekan tombol **Add** di kanan atas.
  - Tempel teks (atau gunakan tombol *Paste from clipboard* / *Choose .md / .txt file*), lalu tekan **Save story**.
  - Cerita langsung masuk ke daftar cerita lokal browser.
  - Jika ingin menyimpan ke folder `stories/`, tekan **Save & download**.

---

## 3. EDIT, DOWNLOAD, HAPUS CERITA LOKAL
- Cerita hasil tombol **Add** memiliki 3 tombol aksi di bawah judulnya: **Edit**, **Download**, dan **Delete**.
- **Edit**: Mengubah judul atau isi teks cerita tanpa menghilangkan progres baca dan skor kuis.
- **Download**: Menyimpan cerita sebagai file `.md` ke folder komputer/HP.
- **Delete**: Menghapus cerita dari penyimpanan lokal browser.
- Halaman **My words**: Menyimpan daftar kata yang pernah Anda tandai/simpan beserta artinya.

---

## 4. FORMAT FILE CERITA (.md)
File markdown cerita menggunakan format berikut:

```markdown
---
title: Past Tense : Telaga Ngebel
level: Pemula
grammar: Simple Past Tense
---
Paragraf pertama cerita...

Paragraf kedua cerita...

## Vocab
long ago: dahulu kala
lived: tinggal (verb-2)
farmer: petani
prayed: berdoa (verb-2)

## Quiz
Q: Where did the farmer live?
- [x] In a village in Ponorogo
- [ ] In a big city
- [ ] On a high mountain

Q: Choose the correct past tense sentence:
- [ ] She pray for a child.
- [x] She prayed for a child.
- [ ] She praying for a child.
```

### Catatan Penulisan:
- **level**: Diisi `Pemula` (Beginner), `Menengah` (Intermediate), atau `Lanjut` (Advanced).
- **Gambar (Images)**: Anda dapat menyisipkan gambar di awal atau di antara paragraf cerita dengan sintaks Markdown:
  ```markdown
  ![Keterangan Gambar](stories/nama-gambar.jpg)
  ```
  atau menggunakan URL internet:
  ```markdown
  ![Keterangan Gambar](https://link-gambar.com/foto.jpg)
  ```
  Gambar akan otomatis tampil rapi di tengah dengan sudut melengkung dan keterangan (caption) di bawahnya, serta tidak akan dibaca keliru oleh TTS.
- **Vocab**: Kata-kata yang dicantumkan di bagian `## Vocab` akan **otomatis berwarna biru** pada teks cerita dan dapat diklik untuk melihat artinya langsung.
- **Quiz**: Gunakan tanda `- [x]` untuk kunci jawaban benar dan `- [ ]` untuk pilihan salah.
- **Penting**: Hindari singkatan bertitik seperti `p.m.`, `a.m.`, `Mr.`, atau `Dr.` agar pemotong kalimat otomatis tidak terputus keliru.

---

## 5. FITUR UTAMA APLIKASI
- **Paging & Sorting (DataTables Style)**:
  - Pilihan jumlah baris per halaman: **Show 5, 10, 25, All entries**.
  - Pengurutan instan: **Title (A-Z) ↑**, **Title (Z-A) ↓**, **Time (Newest) ↓**, dan **Time (Oldest) ↑**.
  - Navigasi halaman lengkap dengan nomor halaman dan nomor urut di setiap judul cerita.
- **Tombol "Copy prompt"**:
  - Salin prompt instruksi pembuatan cerita untuk ChatGPT, Claude, atau Gemini hanya dengan 1 klik.
- **Tiga Mode Membaca**:
  1. **Voice Mode**: Teks dibacakan dengan suara dan kata yang dibaca disorot kuning.
  2. **Silent Mode**: Sorotan kuning berjalan otomatis tanpa suara.
  3. **Scroll Mode**: Teks bergulir otomatis (*auto-scroll*). Jika kata diklik untuk melihat arti, guliran berhenti sementara dan **otomatis berjalan kembali saat pop-up ditutup**.
- **Pengaturan Teks**:
  - Tombol **Aa**: Pengaturan ukuran huruf (*Font size*) dan perataan teks (*Left / Center*).
  - Pengatur kecepatan baca (*WPM - Words Per Minute*).
- **Arti Kata Lengkap (Kamus & Terjemahan)**:
  - Sentuh kata mana saja untuk melihat arti dari cerita, definisi bahasa Inggris, jenis kata, fonetik, dan terjemahan otomatis bahasa Indonesia.

---

## 6. TRAKTIR / DONASI
Jika Anda merasa terbantu dengan program **PORRIDGE** dan ingin mentraktir, traktiran dapat ditransfer melalui:
- **BANK BRI**
- **NOMOR REKENING**: 0516 0101 7476 538
- **ATAS NAMA**: AGUS WALUYO
- **NO TLP / WA**: [+62 819-4613-5363](https://wa.me/6281946135363)
- **EMAIL**: agusw.com@gmail.com
