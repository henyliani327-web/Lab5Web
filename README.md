# PRAKTIKUM 5: JAVASCRIPT
## Nama  : Lola Seftyliani
## Kelas  : TI.24.A.4
## NIM  : 312410339
## Matkul  : Pemograman Web 1

##  Pengenalan JavaScript
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

## JavaScript Dasar
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

## Dasar Pemrograman di JavaScript
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

## Pembuatan Formulir Dan Tombol
file: form_button.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pembuatan Form dan Button</title>
    <script>
        // Fungsi untuk menampilkan hasil input
        function tampilkanNama() {
            let nama = document.getElementById("nama").value;
            document.getElementById("hasil").innerHTML = "Halo, " + nama + "!";
        }
    </script>
</head>
<body>
    <h2>Form Input dan Button</h2>

    <!-- Form Input -->
    <form>
        <label for="nama">Nama:</label>
        <input type="text" id="nama" placeholder="Masukkan nama kamu">
        <button type="button" onclick="tampilkanNama()">Tampilkan</button>
    </form>

    <!-- Hasil tampil di sini -->
    <p id="hasil"></p>
</body>
</html>
```

Membuat file di VSCode dengan nama `form_button.html`. Pada file ini halaman HTML sederhana yang berisi form(input teks + tombol) dan skrip Javascript di elemen <head>. File ini terdapat dua elemen yaitu:
- elemen `<input type="text">` untuk meminta pengguna memasukkan nama, di dalam elemen ini terdapat atribut `id="nama"` digunakan agar javascript bisa mengambil nilainya.
- elemen `<button>` memiliki atribut `onclick="tampilkanNama()"`, yang berarti saat tombol di klik, fungsi tampilanNama()" akan dijalankan.

<img width="1919" height="335" alt="Cuplikan layar 2025-10-24 085930" src="https://github.com/user-attachments/assets/04663fd8-d681-47e5-ab84-388d4de67e2a" />
<img width="1919" height="399" alt="Cuplikan layar 2025-10-24 085953" src="https://github.com/user-attachments/assets/6ad1a71c-b1dc-4544-8641-b1f920554830" />

## HTML DOM (Kotak Ceklis Otomatis)
file: checkbox_total.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Perhitungan Otomatis dengan Checkbox</title>
    <script>
        function hitungTotal() {
            let total = 0;

            // Ambil semua checkbox
            let item1 = document.getElementById("item1");
            let item2 = document.getElementById("item2");
            let item3 = document.getElementById("item3");

            // Cek apakah dipilih
            if (item1.checked) total += parseInt(item1.value);
            if (item2.checked) total += parseInt(item2.value);
            if (item3.checked) total += parseInt(item3.value);

            // Tampilkan hasil
            document.getElementById("total").innerHTML = "Total harga: Rp " + total.toLocaleString();
        }
    </script>
</head>
<body>
    <h2>Perhitungan Otomatis (Checkbox)</h2>

    <form>
        <input type="checkbox" id="item1" value="15000" onclick="hitungTotal()"> Bakso (Rp 15.000)<br>
        <input type="checkbox" id="item2" value="10000" onclick="hitungTotal()"> sempol (Rp 10.000)<br>
        <input type="checkbox" id="item3" value="10000" onclick="hitungTotal()"> Cireng (Rp 10.000)<br><br>
    </form>

    <p id="total">Total harga: Rp 0</p>
</body>
</html>
```

Membuat file di VSCode dengan nama `checkbox_total` pada file ini menampilkan daftar menu makanan dengan checkbox dan menghitung total harga otomatis setiap kali pengguna mencentang atau menghapus pilihan. Perhitungan ini dilakukan menggunakan Javascript tanpa perlu menekan tombol apapun. Di file ini terdapat elemen `<input type="checkbox">` setiap makanan memiliki nilai harga di atribut value. Event `onclick="hitungTotal()"` digunakan agar fungsi dijalankan setiap kali checkbox diklik.

<img width="1915" height="397" alt="Cuplikan layar 2025-10-24 090750" src="https://github.com/user-attachments/assets/c3dc5028-38c2-4b70-861a-57845e8f2bfc" />
<img width="1915" height="391" alt="Cuplikan layar 2025-10-24 090810" src="https://github.com/user-attachments/assets/2771b3b0-b56c-4577-980e-b0821ec7149d" />

## PERTANYAAN DAN TUGAS 
file: validasi_from.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Validasi Form</title>
    <script>
        function validasiForm() {
            let nama = document.getElementById("nama").value;
            let email = document.getElementById("email").value;
            let password = document.getElementById("password").value;

            // Mengecek apakah kolom kosong
            if (nama == "" || email == "" || password == "") {
                alert("Semua kolom harus diisi!");
                return false;
            }

            // Validasi format email
            let polaEmail = /^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
            if (!email.match(polaEmail)) {
                alert("Format email tidak valid!");
                return false;
            }

            // Validasi panjang password
            if (password.length < 6) {
                alert("Password harus minimal 6 karakter!");
                return false;
            }

            alert("Form berhasil dikirim!");
            return true;
        }
    </script>
</head>
<body>
    <h2>Form Registrasi (Validasi dengan JavaScript)</h2>

    <form onsubmit="return validasiForm()">
        <label for="nama">Nama:</label><br>
        <input type="text" id="nama" placeholder="Masukkan nama kamu"><br><br>

        <label for="email">Email:</label><br>
        <input type="text" id="email" placeholder="contoh@email.com"><br><br>

        <label for="password">Password:</label><br>
        <input type="password" id="password" placeholder="Minimal 6 karakter"><br><br>

        <input type="submit" value="Kirim">
    </form>
</body>
</html>
```

<img width="1399" height="487" alt="Cuplikan layar 2025-10-24 091302" src="https://github.com/user-attachments/assets/6de6f2e0-96a1-42d9-9095-93b9db73c129" />
<img width="1917" height="471" alt="Cuplikan layar 2025-10-24 091352" src="https://github.com/user-attachments/assets/957d6f59-2aa8-4674-942e-ad4df000aee3" />
<img width="1919" height="488" alt="Cuplikan layar 2025-10-24 091413" src="https://github.com/user-attachments/assets/75aa9b15-7efe-4ce6-869e-2f672870b9a4" />




