# Manipulasi Lirik Lagu

Proyek ini menunjukkan bagaimana cara memanipulasi dan mengekstrak data dari objek lirik lagu menggunakan JavaScript. Contoh yang digunakan adalah lagu "Little Piece of Heaven" oleh Avenged Sevenfold.

## Daftar Isi
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Penjelasan Kode](#penjelasan-kode)
- [Memodifikasi Data Menggunakan Spread Operator](#memodifikasi-data-menggunakan-spread-operator)
- [Mengekstrak Lirik Tertentu](#mengekstrak-lirik-tertentu)
- [Menjalankan Script](#menjalankan-script)
- [Output](#output)

## Instalasi

Untuk menjalankan proyek ini, pastikan Anda sudah menginstal Node.js. Anda bisa menggunakan `npx` untuk menjalankan TypeScript secara langsung:

```sh
npx tsc lirik.ts && node lirik.js

Penggunaan

Script ini menunjukkan dua fungsi utama:

    Memodifikasi data lirik lagu untuk mengubah artis dan judul lagu.
    Mengekstrak lirik tertentu dari array lirik lagu.

Penjelasan Kode
Memodifikasi Data Menggunakan Spread Operator

Bagian kode ini membuat objek baru newLirikLagu dengan menyalin objek lirik_lagu yang ada dan kemudian memodifikasi properti artist dan songTitle.

javascript

let newLirikLagu = {
  ...lirik_lagu,
  data: {
    ...lirik_lagu.data,
    artist: "Riyan Nurhidayat",
    songTitle: "Ingin menjadi Developer Sukses",
  },
};

Mengekstrak Lirik Tertentu

Bagian kode ini mencari lirik tertentu dalam array songLyricsArr dan menyimpannya dalam variabel targetLyric.

javascript

let targetLyric = "";
for (let i = 0; i < lirik_lagu.data.songLyricsArr.length; i++) {
  if (
    lirik_lagu.data.songLyricsArr[i].indexOf(
      "For me to take what's mine, until the end of time?"
    ) !== -1
  ) {
    targetLyric = lirik_lagu.data.songLyricsArr[i];
    break;
  }
}

Menjalankan Script

Untuk menjalankan script, gunakan perintah berikut:

npx tsc lirik.ts && node lirik.js

Output

Script akan mencetak objek lirik baru dan lirik yang diekstrak ke konsol:

Lirik Lagu Baru: { ... objek yang telah dimodifikasi ... }
Lirik yang diambil: For me to take what's mine, until the end of time?

arduino


File `README.md` ini memberikan panduan yang jelas dan ringkas untuk proyek ini, dengan menjelaskan instalasi, penggunaan, penjelasan kode, menjalankan script, dan output yang diharapkan.