# Bootstrap Clone 2

Latihan kolaborasi Git dan GitHub pada praktikum Pengembangan Aplikasi Web, Modul 6.
Halaman ini meniru tampilan beranda Bootstrap dengan memanfaatkan framework Bootstrap
5.3.0-alpha2 serta Bootstrap Icons yang dimuat dari CDN.

> Nama repository "bootsrap-clone-2" memang typo, sesuai pembahasan di laporan praktikum.

## Menjalankan

Tidak diperlukan build tool maupun instalasi. Cukup buka `index.html` di browser.

Bila ingin memakai server lokal (opsional):

```bash
python -m http.server 8000
```

lalu buka <http://localhost:8000>.

## Struktur Berkas

```
index.html              Halaman utama
assets/css/style.css    Gaya kustom (warna navbar, ukuran logo, footer)
assets/images/          Aset gambar
```

## Branch

| Branch          | Keterangan                          |
| --------------- | ----------------------------------- |
| `master`        | Branch utama, hasil penggabungan    |
| `yahdi-branch`  | Inisialisasi proyek dan finishing   |
| `adam-branch`   | Struktur main dan Bootstrap Icons   |
| `kenmada-branch`| Footer                              |
| `damba-branch`  | Perbaikan bug dan perapian kode     |

## Alur Kontribusi

1. `git clone https://github.com/yahdee2702/bootsrap-clone-2.git`
2. `git checkout -b <nama>-branch`
3. Lakukan perubahan, lalu `git commit`
4. `git push origin <nama>-branch`
5. Buat Pull Request ke branch `master`

## Masalah yang Diketahui

- `assets/images/bs-themes.png` masih berupa placeholder berisi teks
  "Gotcha, this is empty" (21 byte), sehingga ilustrasi pada bagian
  "Bootstrap Official Themes" tampil rusak dan perlu diganti dengan gambar asli.
  Logo `logo-white.svg` dan `logo-black.svg` sudah diperbaiki.
- `assets/images/bs-icons.png` dan `assets/images/main.svg` belum dipakai di `index.html`.
- Versi Bootstrap pada CDN masih `5.3.0-alpha2`. Pembaruan sengaja belum dilakukan
  agar tampilan yang sudah disepakati tidak berubah.

## Lisensi Aset

Logo pada `assets/images/logo-white.svg` dan `assets/images/logo-black.svg`
menggunakan logo resmi Bootstrap (lisensi MIT, proyek twbs/bootstrap).
