# Calculate Average and Grade

Saya membuat function dengan nama `calculateAverageAndGrade` yang memiliki parameter `webProgramming`, `computerProgramming`, `statistics`, dan `databaseSystems` yang memiliki tipe data `number`. Fungsi ini bertujuan untuk menghitung rata-rata nilai dari keempat parameter tersebut dan menentukan grade berdasarkan rata-rata yang diperoleh.

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

    Clone repository ini atau buat file nilai.ts dan salin kode di bawah ini ke dalam file tersebut:

    typescript

    function calculateAverageAndGrade(
      webProgramming: number,
      computerProgramming: number,
      statistics: number,
      databaseSystems: number
    ): void {
      // Validasi
      if (
        webProgramming === undefined ||
        computerProgramming === undefined ||
        statistics === undefined ||
        databaseSystems === undefined
      ) {
        console.error("Semua nilai harus diisi.");
        return;
      }

      const total =
        webProgramming + computerProgramming + statistics + databaseSystems;
      const average = total / 4;

      let grade: string;
      if (average >= 90 && average <= 100) {
        grade = "A";
      } else if (average >= 80 && average < 90) {
        grade = "B";
      } else if (average >= 70 && average < 80) {
        grade = "C";
      } else if (average >= 60 && average < 70) {
        grade = "D";
      } else if (average >= 0 && average < 60) {
        grade = "E";
      } else {
        console.error("Nilai tidak valid.");
        return;
      }

      // Hasil
      console.log(`Rata-rata: ${average}`);
      console.log(`Grade: ${grade}`);
    }

    const webProgramming = 85;
    const computerProgramming = 90;
    const statistics = 78;
    const databaseSystems = 88;

    calculateAverageAndGrade(
      webProgramming,
      computerProgramming,
      statistics,
      databaseSystems
    );

Cara Menjalankan

    Compile kode TypeScript:

    Buka terminal dan navigasikan ke direktori tempat file nilai.ts disimpan. Jalankan perintah berikut:

tsc nilai.ts

Perintah ini akan mengkompilasi file TypeScript menjadi file JavaScript dengan nama nilai.js.

Jalankan file JavaScript yang sudah dikompilasi menggunakan Node.js:

node nilai.js
