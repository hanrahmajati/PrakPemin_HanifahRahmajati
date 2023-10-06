# Modul 3 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 3 Pemrograman Integratif TI-A - Integrasi MongoDB dan Express</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## Percobaan instalasi NodeJS
### Langkah 1
> Buka halaman nodejs.org/en/ <br /><br />

### Langkah 2
> Download dan jalankan node setup. <br /><br />

### Langkah 3
> Setelah instalasi selesai jalankan command ```node -v``` untuk memeriksa apakah NodeJS sudah terinstall. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss01_3.png)  

## Inisiasi project Express dan pemasangan package
### Langkah 1
> Lakukan pembuatan folder dengan nama express-mongodb dan masuk ke dalam folder tersebut lalu buka melalui text editor masing-masing. <br /><br />

### Langkah 2
> Lakukan npm init untuk mengenerate file package.json dengan menggunakan command ```npm init -y``` <br /><br />
>![ss langkah 1](../Screenshot/Modul3/ss02_2.png)  

### Langkah 3
> Lakukan instalasi express, mongoose, dan dotenv dengan menggunakan command ```npm i express mongoose dotenv``` <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss02_3.png)  

## Koneksi Express ke MongoDB
### Langkah 1
> Buatlah file index.js pada root folder dan masukkan kode di bawah ini. Setelah itu coba jalankan aplikasi dengan command node index.js <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss03_1.png)  

### Langkah 2
> Lakukan pembuatan file .env dan masukkan baris berikut. Setelah itu ubahlah kode pada listening port menjadi berikut dan coba jalankan aplikasi kembali. Copy connection string yang terdapat pada compas atau atlas dan paste kan pada .env seperti berikut. <br /><br />
>![ss langkah 1](../Screenshot/Modul3/ss03_2.png)  

### Langkah 3
> Tambahkan baris kode berikut pada file index.js. Setelah itu coba jalankan aplikasi kembali. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss03_4.png)  
> ![ss langkah 3](../Screenshot/Modul3/ss03_4_2.png)  

## Pembuatan routing
### Langkah 1
> Lakukan pembuatan direktori routes di tingkat yang sama dengan index.js <br /><br />

### Langkah 2
> Buatlah file book.route.js di dalamnya. <br /><br />

### Langkah 3
> Tambahkan baris kode berikut untuk fungsi getAllBooks. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss04_3.png)  

### Langkah 4
> Lakukan hal yang sama untuk getOneBook, createBook, updateBook, dan deleteBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss04_4.png)  

### Langkah 5
> Lakukan import book.route.js pada file index.js dan tambahkan baris kode berikut. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss04_5.png)  

### Langkah 6
> Uji salah satu endpoint dengan Postman. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss04_6.png)  

## Pembuatan controller
### Langkah 1
> Lakukan pembuatan direktori controllers di tingkat yang sama dengan index.js <br /><br />

### Langkah 2
> Buatlah file book.controller.js di dalamnya. <br /><br />

### Langkah 3
> Buatlah file book.controller.js di dalamnya. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss05_3.png)  

### Langkah 4
> Lakukan hal yang sama untuk getOneBook, createBook, updateBook, dan deleteBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss05_4.png)  

### Langkah 5
> Lakukan import book.controller.js pada file book.route.js. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss05_5.png)  

### Langkah 6
> Lakukan perubahan pada fungsi agar dapat memanggil fungsi dari book.controller.js. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss05_6.png)  

### Langkah 7
> Lakukan pengujian kembali, pastikan response tetap sama. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss05_7.png)  

## Pembuatan model
### Langkah 1
> Lakukan pembuatan direktori models di tingkat yang sama dengan index.js <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss06_1.png)  

### Langkah 2
> Buatlah file book.model.js di dalamnya. <br /><br />

### Langkah 3
> Tambahkan baris kode berikut sesuai dengan tabel di atas. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss06_3.png)  

## Operasi CRUD
### Langkah 1
> Hapus semua data pada collection books. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_1.png)  

### Langkah 2
> Lakukan import book.model.js pada file book.controller.js. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_2.png)  

### Langkah 3
> Lakukan perubahan pada fungsi createBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_3.png)  

### Langkah 4
> Buatlah dua buah buku dengan data di bawah ini dengan Postman. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_4.png)  

### Langkah 5
> Lakukan perubahan pada fungsi getAllBooks. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_5.png)  

### Langkah 6
> Lakukan perubahan pada fungsi getOneBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_6.png)  

### Langkah 7
> Tampilkan semua buku dengan Postman. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_7.png)  

### Langkah 8
> Tampilkan buku Dilan 1990 dengan Postman. <br /><br />  

### Langkah 9
> Lakukan perubahan pada fungsi updateBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_9.png)  

### Langkah 10
> Ubah judul buku Dilan 1991 menjadi "<NAMA PANGGILAN> 1991" dengan Postman. <br /><br />

### Langkah 11
> Lakukan perubahan pada fungsi deleteBook. <br /><br />
>![ss langkah 3](../Screenshot/Modul3/ss07_11.png)  