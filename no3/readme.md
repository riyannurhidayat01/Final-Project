# Print Segitiga

Proyek ini berisi kode TypeScript untuk mencetak pola segitiga di konsol. Kode ini menggunakan fungsi `printTriangle` yang menerima parameter `height` untuk menentukan tinggi segitiga.

## Prasyarat

Sebelum menjalankan proyek ini, pastikan Anda telah menginstal:

- Node.js
- TypeScript

## Instalasi

1. **Install TypeScript Compiler (jika belum terinstal):**

   Buka terminal Anda dan jalankan perintah berikut:
   ```sh
   npm install -g typescript

    Clone Repository:

    Clone repository ini atau buat file segitiga.ts dan salin kode di bawah ini ke dalam file tersebut:

    typescript

    function printTriangle(height: number): void {
        for (let i = 1; i <= height; i++) {
            console.log(' '.repeat(height - i) + '* '.repeat(i).trim());
        }
    }

    const height = 10;
    printTriangle(height);

Cara Menjalankan

    Compile kode TypeScript:

    Buka terminal dan navigasikan ke direktori tempat file segitiga.ts disimpan. Jalankan perintah berikut:

tsc segitiga.ts

Perintah ini akan mengkompilasi file TypeScript menjadi file JavaScript dengan nama segitiga.js.

Jalankan kode JavaScript yang sudah dikompilasi:

Jalankan file JavaScript yang sudah dikompilasi menggunakan Node.js:

    node segitiga.js

    Perintah ini akan mencetak pola segitiga dengan tinggi yang ditentukan ke konsol.




