# Praktikum 5
# Pemrograman Web
```
Muhammad Rizkiansyah
311910071
TI.19.C.1
Universitas Pelita Bangsa
```
## Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```
![P 5 1](https://user-images.githubusercontent.com/81758407/116433285-8d48dc80-a873-11eb-9cb3-be7915b63a35.PNG)
## Javascrip Dasar
Pemakaian Alert sebagai property window.
```
<html>
<head>
    <title>Alert box</title>
</head>
<body>
<script language = "javascript">
<!-- 
window.alert("Ini merupakan pesan untuk anda");
//-->
    </script>
</body>
</html>
```
![p 5 2](https://user-images.githubusercontent.com/81758407/116435868-05180680-a876-11eb-825d-b0579cd92de6.PNG)
Pemakaian method dalam objek
```
<html>
<head>
    <title>skrip javascript</title>
</head>
<body>
    Percobaan memakai javascript:<br>
<script language = "javascript">
<!-- 
 document.write("selamat mencoba javascript<br>");
 document.write("semoga sukses!");
//-->
    </script>
</body>
</html>
```
![p 5 3](https://user-images.githubusercontent.com/81758407/116436960-1e6d8280-a877-11eb-85a5-e01909b60497.PNG)
Pemakaian Prompt
```
<html>
<head>
    <title>Pemasukan data</title>
</head>
<body>
<script language = "javascript">
<!-- 
 var nama = prompt("siapa nama anda?","masukkan nama anda");
 document.write("hai,"+ nama);
//-->
    </script>
</body>
</html>
```
![p 5 4](https://user-images.githubusercontent.com/81758407/116437556-c3885b00-a877-11eb-80e5-9ee5bdbf101c.PNG)
Pembuatan fungsi dan cara pemanggilannya
```
<html>
<head>
    <title>contoh program javascript</title>
    <script language = "javascript">
        function pesan(){
            alert ("memanggil javascript lewat body onload")
        }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```
![p 5 5](https://user-images.githubusercontent.com/81758407/116438357-912b2d80-a878-11eb-855e-f6b770442995.PNG)
## Dasar Pemrograman Di Javascript
Operasi dasar aritmatika
```
<html>
<head>
    <title>contoh program javascript</title>
    <script language = "javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2"+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2"+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2"+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-al2"+"<br>")
        document.write(val1-val2) 
        document.write("<br>"+"modulus : val1%val2"+"<br>")
        document.write(val1%val2)  
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="aritmetic" onclick=test(9,4)>
</body>
</html>
```
![p 5 6](https://user-images.githubusercontent.com/81758407/116441288-858d3600-a87b-11eb-9f10-cd66d5973212.PNG)
Seleksi kondisi (if..else)
```
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
        var nilai = prompt("nilai (0-100): ",0);
        var hasil = " ";
        if (nilai >= 60)
        hasil = "lulus";
        else hasil = "tidak lulus";
        document.write("hasil: " + hasil);
        //-->
    </script>
   </body>
</html>
```
![p 5 7](https://user-images.githubusercontent.com/81758407/116444347-d5b9c780-a87e-11eb-8224-1e93b0ed757e.PNG)
![p 5 8](https://user-images.githubusercontent.com/81758407/116444340-d3f00400-a87e-11eb-97f7-a4bf2a8eb12e.PNG)
Penggunaan operator switch untuk seleksi kondisi
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language = "javascript">
    function test ()
    {
        vall=window.prompt("input nilai (1-5):")
        switch (vall)
        {
            case "1" :
                document.write("bilangan satu")
                break
            case "2" :
                document.write("bilangan dua")
                break
            case "3" :
                document.write("bilangan tiga")
                break
            case "4" :
                document.write("bilangan empat")
                break
            case "5" :
                document.write("bilangan lima")
                break
            default :
                document.write("bilangan lainnya")
        }
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```
![p 5 9](https://user-images.githubusercontent.com/81758407/116697371-4da60000-a9ed-11eb-84ac-a8fa6df0d92c.PNG)
![p 5 10](https://user-images.githubusercontent.com/81758407/116697398-5696d180-a9ed-11eb-8990-44a98d81f2f3.PNG)
## Pembuatan Form
Form Input
```
<html>
<head>
    <script language = "javascript">
    function test ()
    {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```
![p 5 11](https://user-images.githubusercontent.com/81758407/116698692-d96c5c00-a9ee-11eb-845f-dadf80fe079b.PNG)
Form Button.
```
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language="javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
        document.fgColor = warna; 
    }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language="javascript">
    <!--
    document.write("Dimodifikasi terakhir pada " +
    document.lastModified);
    //-->
    </script>
</body>
</html>
```
![p 5 12](https://user-images.githubusercontent.com/81758407/116700714-484ab480-a9f1-11eb-992c-f44900999f68.PNG)
## HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;
            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br/>
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 5.00</label><br/>
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><br/>
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```
![p 5 13](https://user-images.githubusercontent.com/81758407/116704062-2f440280-a9f5-11eb-8360-762e6f90ceba.PNG)
## Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Form Validasi</title>
    <link rel="stylesheet" type="text/css" href="style.css">
    <script type="text/javascript">
        function validasiForm() {
            var nama = document.getElementById('nama').value;
            var email = document.getElementById('email').value;
            var alamat = document.getElementById('alamat').value;
            if (nama != "" && email != "" && alamat !="") {
                return true;
            } else {
                alert('Isi alamat anda dengan lengkap !');
                return false;
            }
        }
    </script>
</head>
<body>
    <header>
        <h1>Form Validasi</h1>
    </header>
   <div class="login">
       <form action="home.html" method="post" onsubmit="return validasiForm()">
        <fieldset>
            <legend>Daftar</legend>
            <div>
                <label>Nama Lengkap :</label>
                <input type="text" name="nama" id="nama" />
            </div>
            <div>
                <label>Email :</label>
                <input type="email" name="email" id="email" />
            </div>
            <div>
                <label>Alamat :</label>
                <textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
            </div>
            <div>
                <input type="submit" value="Daftar" class="tombol">
            </div>
        </fieldset>
    </form>
   </div>
</body>
</html>
```
Buat file baru dengan nama home.html
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-eidth, initial-scale=1,0">
        <title>Home</title>
        <link role="stylesheet" href="stylee.css">
        <script lang="javascript">
            function pesan() {
                alert ("Selamat datang")
            }
        </script>
    </head>
    <body onload=pesan()>    
        <center><h1>Terimakasih telah mendaftar!!!</h1></center>
    </body>
</html>
```
Tambahkan css
```
body {
    background: darkslategray;
    font-family: sans-serif;
    padding: 200px;
    }
header {
    min-height: 80px;
    }
h1 {
    font-size: 24px;
    color: #ffffff;
    text-align: center;
    padding: 20px 10px;
    }
h1 i {
    color:#6d6a6b;
    }
h2 {
    color: khaki;
    }
.loading {
    padding: 1em;
    margin: 2em auto;
    width: 17em;
    background: lightslategray;
    border-radius: 3px;
    }
label {
    font-size: 10pt;
    color: lightsteelblue;
    }
input[type="text"],
input[type="email"],
textarea {
    padding: 8px;
    width: 95%;
    background: lightgray;
    border: 0;
    font-size: 10pt;
    margin: 6px 0px;
    }
.tombol {
    background: white;
    color: rgb(2, 2, 2);
    border: 0;
    padding: 5px 8px;
    }
    
```
![p 5 14](https://user-images.githubusercontent.com/81758407/116764896-d7d18100-aa4c-11eb-8172-f455391254e9.PNG)
