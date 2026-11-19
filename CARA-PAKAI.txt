BACA INGGRIS - cara pakai
=========================

Seluruh menu di aplikasi memakai bahasa Inggris. Nama tombol di panduan ini
ditulis sama persis seperti di aplikasi.

1. PASANG
   - Ekstrak zip ini di HP. Hasilnya satu folder "baca-inggris" berisi:
     index.html, manifest.json, sw.js, folder icons, dan folder stories.
   - Di aplikasi web server kamu, pilih folder "baca-inggris" sebagai root, lalu Start.
   - Buka Chrome, ketik http://localhost:PORT (port lihat di aplikasi server).
     Pakai "localhost", jangan alamat IP, supaya bisa diinstal.
   - Menu titik tiga -> Instal aplikasi / Tambahkan ke layar utama.
   - Setelah terinstal, aplikasi tetap bisa dibuka walau servernya mati.

2. TAMBAH / UPDATE CERITA
   - Taruh file .md baru di folder "stories", lalu buka aplikasinya.
     Daftar cerita diperbarui otomatis setiap kali halaman daftar dibuka
     (atau tekan "Reload stories").
   - Ganti isi file .md yang sudah ada = cerita ikut berubah.
   - Hapus file .md = cerita hilang dari daftar.
   - Kalau cerita baru tidak muncul, server kamu kemungkinan tidak
     menampilkan daftar isi folder. Solusinya: buat file stories/index.json
     berisi daftar nama file, contoh:
         ["the-lost-key.md", "cerita-baru.md"]
   - Cara lain tanpa folder: tombol "Add" di aplikasi. Tempel teks
     (atau "Paste from clipboard", atau "Choose .md / .txt file"), tekan
     "Save story", dan cerita langsung masuk daftar. Tiap cerita punya nomor
     (No. 1, 2, 3...) sesuai urutan ditambahkan, dan nomor tidak dipakai ulang
     walau ada yang dihapus. Disimpan di browser HP saja.
   - Teks tempelan biasa (tanpa format) juga bisa: tiap baris jadi satu paragraf.

3. EDIT, DOWNLOAD, HAPUS CERITA YANG TERSIMPAN DI BROWSER
   - Cerita hasil tombol "Add" punya tiga tombol di bawah judulnya:
     Edit, Download, Delete.
   - Edit: buka kembali judul dan teksnya, ubah, lalu "Save changes".
     Posisi baca dan skor kuis tetap ada.
   - Download: menyimpan cerita sebagai file .md (dengan judul di bagian atas
     file) agar bisa masuk ke folder "stories" dan ikut terbaca server.
       * Chrome di komputer: tekan "Choose stories folder" di bagian bawah
         daftar (atau tekan Download pertama kali), pilih folder "stories".
         Setelah itu file langsung tertulis ke folder tersebut. Kalau ada
         stories/index.json, nama file ikut ditambahkan otomatis.
       * Chrome di Android belum mendukung pilih-folder. File akan terunduh
         ke folder Download. Pindahkan ke folder "stories" lewat aplikasi File.
   - Di dialog Add / Edit ada tombol "Save & download": simpan di browser
     sekaligus unduh file .md-nya.
   - Setelah file ada di folder "stories", salinan di browser boleh dihapus
     (Delete) supaya cerita tidak muncul dua kali.
   - Halaman "My words": tiap kata punya tombol Listen, Edit (ubah arti), Delete.

4. FORMAT FILE CERITA (.md)
   ---
   title: Judul Cerita
   level: Intermediate
   ---

   Paragraf pertama...

   Paragraf kedua...

   ## Vocab
   kata: arti
   kata lain: arti lain

   ## Quiz
   Q: Pertanyaan?
   - [ ] Pilihan salah
   - [x] Pilihan benar
   - [ ] Pilihan salah

   Catatan:
   - level: isi Beginner / Intermediate / Advanced. Tulisan lama (Pemula,
     Menengah, Lanjut) tetap terbaca dan otomatis tampil dalam bahasa Inggris.
   - Vocab dan Quiz boleh dihilangkan. Kalau Quiz kosong tapi Vocab ada
     minimal 4 kata, kuis arti kata dibuat otomatis.
   - Hindari singkatan bertitik seperti "p.m." karena dianggap akhir kalimat.

5. DAFTAR CERITA
   - Kolom "Search by title" menyaring daftar sesuai judul (tanda X untuk
     menghapus pencarian).
   - Daftar ditampilkan 10 cerita per halaman. Pakai tombol Previous / Next
     di bawah daftar untuk pindah halaman.

6. FITUR
   - Teks berjalan: tombol putar. Kecepatan diatur dengan tombol - Normal +
     (tiap tap 10 kata/menit; tap "Normal" untuk kembali ke 150).
   - Tombol "Highlight" menampilkan atau menyembunyikan sorotan kata.
   - Baris tombol putar: Cerita sebelumnya (kiri), kalimat sebelumnya, putar/jeda,
     kalimat berikutnya, Cerita berikutnya (kanan). Urutan cerita sama dengan daftar.
   - Tab ikon kecil di atas panel kontrol: ikon panah bawah menyembunyikan
     pengaturan, ikon penggeser (sliders) menampilkannya lagi.
   - Tombol ikon panah di pojok atas: layar penuh (keluar dengan tombol yang sama
     atau gestur kembali).
   - Tiga mode: Voice (dibacakan, highlight mengikuti), Silent (highlight saja),
     Scroll (layar menggulir sendiri pelan-pelan, highlight di garis baca).
     Geser layar dengan jari kapan saja, scroll akan lanjut dari posisi baru.
   - Tombol "Aa": ukuran huruf dan rata teks (Left / Center).
   - Tap kata: arti di cerita (Vocab), definisi dan terjemahan otomatis
     (butuh internet; kata yang pernah dibuka tersimpan untuk offline).
   - Simpan kata lewat "Save word", lihat di "My words".
   - Di akhir bacaan: "Start quiz" dan "Read from start".
   - Posisi baca dan skor kuis tersimpan otomatis.

7. MASALAH UMUM
   - Tidak ada suara: pastikan "Text-to-speech" bahasa Inggris aktif di
     Pengaturan Android (Google Text-to-speech). Aplikasi otomatis pindah
     ke mode Silent kalau suara gagal.
   - Tombol Instal tidak muncul: pastikan alamatnya localhost, bukan IP.
   - Perubahan aplikasi tidak terlihat: tutup aplikasi sepenuhnya lalu buka lagi.
