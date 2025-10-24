
## Nama  : Lola Seftyliani
## Kelas  : TI.24.A.4
## NIM  : 312410339
## Matkul  : Pemograman Web 1

## Langkah 1- Pengenalan JavaScript
File:Lab5_Javasript.html
Menampilkan alert, document.write, dan console.log.
```
<script>
    alert("Javascript pada tag head.");
    document.write("Hello World");
    console.log("Hello World");
</script>
```

<img width="1906" height="517" alt="Cuplikan layar 2025-10-24 074706" src="https://github.com/user-attachments/assets/f84852cb-1823-48f4-9b5b-2e7c42708ea6" />


- Muncul alert “Javascript pada tag head.”
- Halaman menampilkan teks Hello World
- Console menampilkan Hello World

## Langkah 2 - JavaScript Dasar
File: dasar_javascript.html
Latihan penggunaan alert, prompt, dan function.
```
alert("Halo!");
  let nama = prompt("Siapa namamu?");
  function salam(nama) {
      return "Selamat datang, " + nama + "!";
  }
    document.write(salam(nama));
```

<img width="1797" height="375" alt="Cuplikan layar 2025-10-24 080915" src="https://github.com/user-attachments/assets/56bbd7b4-a7fc-4103-9039-ea7bb93ac8bc" />

- Alert muncul saat halaman dibuka.
- Prompt meminta nama pengguna.
- Output di halaman: “Selamat datang, [nama]!”

<img width="1919" height="319" alt="Cuplikan layar 2025-10-24 081035" src="https://github.com/user-attachments/assets/86292253-f60a-49aa-af9a-008b09dd5d86" />

## Langkah 3 – Dasar Pemrograman di JavaScript
File: dasar_pemrograman.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Dasar Pemrograman di JavaScript</title>
</head>
<body>
    <h2>Dasar Pemrograman di JavaScript</h2>

    <script>
        // --- Operasi Aritmatika ---
        let a = 10;
        let b = 5;

        document.write("<h3>Operasi Aritmatika</h3>");
        document.write("a = " + a + ", b = " + b + "<br>");
        document.write("Penjumlahan (a + b) = " + (a + b) + "<br>");
        document.write("Pengurangan (a - b) = " + (a - b) + "<br>");
        document.write("Perkalian (a * b) = " + (a * b) + "<br>");
        document.write("Pembagian (a / b) = " + (a / b) + "<br>");
        document.write("Sisa bagi (a % b) = " + (a % b) + "<br><br>");

        // --- Seleksi Kondisi if..else ---
        document.write("<h3>Seleksi Kondisi if..else</h3>");
        let nilai = prompt("Masukkan nilai ujianmu:");
        if (nilai >= 75) {
            document.write("Selamat, kamu lulus!<br>");
        } else {
            document.write("Maaf, kamu belum lulus.<br>");
        }

        // --- Operator Switch ---
        document.write("<h3>Seleksi Kondisi switch</h3>");
        let grade = prompt("Masukkan grade (A/B/C/D):");
        switch (grade) {
            case "A":
                document.write("Nilai kamu sangat baik!<br>");
                break;
            case "B":
                document.write("Nilai kamu baik.<br>");
                break;
            case "C":
                document.write("Nilai kamu cukup.<br>");
                break;
            case "D":
                document.write("Nilai kamu kurang.<br>");
                break;
            default:
                document.write("Grade tidak valid!<br>");
        }
    </script>
</body>
</html>
```

Membuat file di VSCode dengan nama `dasar_pemrograman.html`. Pada file ini membantu memahami cara kerja perhitungan, logika pengambilan keputusan, dan interaksi dengan pengguna menggunakan `prompt`, untuk melakukan operasi aritmatika atau koleksi kondisi menggunakan struktur sebagai berikut:
- Struktur Seleksi kondisi `if..else` pengguna diminta memasukkan nilai ujian melalui `prompt()`. Jika nilai lebih besar dari 75, maka akan muncul pesan "Selamat, kamu lulus!". dan jika kurang dari 75 akan muncul "Maaf, kamu belum lulu!".
- Struktur Seleksi kondisi `switch` program meminta pengguna memasukkan grade (A/B/C/D) berdasarkan input Javascript memampilakan pesan yang sesuai:
- A: Nilai sangat baik
- B: Nilai baik
- C: Nilai cukup
- D: Nilai kurang

Jika input tidak sesuai, muncul pesan "Grade tidak valid".

<img width="1837" height="394" alt="Cuplikan layar 2025-10-24 085257" src="https://github.com/user-attachments/assets/26091981-97e5-49a3-a5ac-e54dabe441df" />
<img width="1833" height="361" alt="Cuplikan layar 2025-10-24 085314" src="https://github.com/user-attachments/assets/b147180c-7af2-4bf2-a6f8-0df894bfba65" />
<img width="1339" height="858" alt="Cuplikan layar 2025-10-24 085333" src="https://github.com/user-attachments/assets/cfcb9dcc-b131-42dd-97ec-c2f5041fc399" />



