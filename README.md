# Catatan Keuangan

Aplikasi pencatatan keuangan dengan dua akun:

- **Work** (operasional): Vianos (futsal), Seven Dragon BL (billiard), Cafe Reservasi. Ada kas, piutang, pembayaran, dan riwayat.
- **Personal**: uang masuk dan keluar, piutang, target tabungan, dan kalkulator perencanaan tabungan.

Aplikasi ini berupa satu halaman web (PWA) tanpa server. Semua data tersimpan di browser perangkat kamu.

## Isi folder

| File | Fungsi |
|---|---|
| `index.html` | Seluruh aplikasi |
| `manifest.webmanifest` | Nama, warna, dan ikon aplikasi saat diinstal |
| `sw.js` | Membuat aplikasi tetap bisa dibuka tanpa internet |
| `icons/` | Logo dan ikon aplikasi |
| `.nojekyll` | Supaya GitHub Pages menampilkan file apa adanya |

## Cara memasang di GitHub Pages

1. Ekstrak file zip ini.
2. Di GitHub, buat repository baru (misalnya `keuangan`), pilih **Public**.
3. Klik **Add file > Upload files**, lalu tarik **semua isi folder hasil ekstrak** (termasuk folder `icons` dan file `.nojekyll`). File harus berada di halaman paling atas repository, bukan di dalam folder lain. Klik **Commit changes**.
4. Buka **Settings > Pages**. Pada **Build and deployment**, pilih **Deploy from a branch**, branch **main**, folder **/ (root)**, lalu **Save**.
5. Tunggu 1 sampai 3 menit. Alamatnya akan tampil di halaman yang sama: `https://USERNAME.github.io/NAMA-REPO/`.

## Cara menginstal di HP

- **Android (Chrome):** buka alamatnya, ketuk menu titik tiga, lalu **Instal aplikasi** atau **Tambahkan ke layar utama**.
- **iPhone (Safari):** buka alamatnya, ketuk tombol **Bagikan**, lalu **Tambah ke Layar Utama**.
- **Komputer (Chrome atau Edge):** klik ikon instal di kanan kolom alamat.

## Hal yang perlu diketahui

- **Data tersimpan per perangkat dan per browser.** Data di HP tidak otomatis muncul di komputer. Data dari versi yang kamu pakai di Claude juga tidak ikut pindah karena alamatnya berbeda, jadi aplikasi ini mulai dari kosong.
- **Jangan menghapus data situs** di pengaturan browser, karena itu ikut menghapus catatan keuangan.
- **Memperbarui aplikasi:** ganti `index.html` di GitHub, lalu naikkan angka versi di baris pertama `sw.js` (misalnya `keuangan-v2`). Buka aplikasi dua kali supaya versi baru terpasang.
- Font (Plus Jakarta Sans) dimuat dari Google Fonts saat pertama kali online. Kalau offline sebelum itu, aplikasi memakai font bawaan perangkat.
