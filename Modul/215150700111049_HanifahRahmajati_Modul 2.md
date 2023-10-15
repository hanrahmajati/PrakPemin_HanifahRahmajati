# Modul 2 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 2 Pemrograman Integratif TI-A - CRUD MongoDB Compass dan Shell</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## MongoDB Compass
### Langkah 1
Lakukan koneksi ke MongoDB menggunakan connection string. <br /><br />
![ss langkah 1](../Screenshot/Modul2/ss1.png) <br /><br />

### Langkah 2
Buat database dengan melakukan klik "Create Database". <br /><br />
![ss langkah 2](../Screenshot/Modul2/ss2.png) <br /><br />

### Langkah 3
Lakukan insert buku pertama dengan melakukan klik "Add Data", pilih "Insert Document", isi dengan data yang diinginkan dan klik "Insert". <br /><br />
![ss langkah 3](../Screenshot/Modul2/ss3.png) <br /><br />

### Langkah 4
Lakukan insert buku kedua dengan cara yang sama. <br /><br />
![ss langkah 4](../Screenshot/Modul2/ss4.png) <br /><br />
![ss langkah 4](../Screenshot/Modul2/ss4b.png) <br /><br />

### Langkah 5
Lakukan pencarian buku dengan author "Osamu Dazai" dengan mengisi filter yang diinginkan dan klik "Find". <br /><br />
![ss langkah 5](../Screenshot/Modul2/ss5.png) <br /><br />

### Langkah 6
Lakukan perubahan summary pada buku "No Longer Human" menjadi "Buku yang bagus (<NAMA>,<NIM>)" dengan melakukan klik "Edit Document" (berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik "Update". <br /><br />
![ss langkah 6](../Screenshot/Modul2/ss6.png) <br /><br />
![ss langkah 6](../Screenshot/Modul2/ss6b.png) <br /><br />

### Langkah 7
Lakukan penghapusan pada buku "Supernova: Partikel" dengan melakukan klik "Remove Document" (berlambang tong sampah) dan melakukan klik "Delete". <br /><br />
![ss langkah 7](../Screenshot/Modul2/ss7.png) <br /><br />

## MongoDB Shell
### Langkah 1
Lakukan koneksi ke MongoDB Server dengan menjalankan command ```mongosh``` bagi yang menggunakan terminal build in OS. Apabila menggunakan MongoDB atlas, copy connection string dari MongoDB atlas dan paste-kan di terminal. <br /><br />
![ss langkah 8](../Screenshot/Modul2/ss8.png) <br /><br />

### Langkah 2
Mencoba melihat list database yang ada di server dengan menjalankan command ```show dbs```. <br /><br />
![ss langkah 9](../Screenshot/Modul2/ss9.png) <br /><br />
Untuk berpindah ke database "bookstore" gunakan command ```use bookstore```, kalian dapat memastikan telah berpindah ke database yang benar dengan melihat tulisan sebelum tanda ">". <br /><br />
![ss langkah 9b](../Screenshot/Modul2/ss9b.png) <br /><br />
Cobalah untuk melihat collection yang ada pada database tersebut dengan menggunakan command ```show collections```. <br /><br /> 
![ss langkah 9c](../Screenshot/Modul2/ss9c.png) <br /><br />

### Langkah 3
Lakukan insert buku "Overlord I" dengan menggunakan command ```db.books.insertOne(<data kalian>)```. <br /><br />
![ss langkah 10](../Screenshot/Modul2/ss10.png) <br /><br />

### Langkah 4
Lakukan insert buku "The Setting Sun" dan "Hujan" dengan insert many dengan menggunakan command ```db.books.insertMany(<data kalian>)```. <br /><br />
![ss langkah 11](../Screenshot/Modul2/ss11.png) <br /><br />

### Langkah 5
Lakukan pencarian buku dengan menggunakan command ```db.books.find()``` untuk melakukan pencarian semua buku. <br /><br />
![ss langkah 12](../Screenshot/Modul2/ss12.png) <br /><br />

### Langkah 6
Tampilkan seluruh buku dengan author "Osamu Dazai" dengan mengisi argument pada find() dengan menggunakan command ```db.books.find({<filter yang ingin diisi>})```. <br /><br />
![ss langkah 13](../Screenshot/Modul2/ss13.png) <br /><br />

### Langkah 7
Lakukan perubahan summary pada buku "Hujan" menjadi "Buku yang bagus (<NAMA>,<NIM>)" dengan mengunakan command ```db.books.updateOne({<filter>}, {$set: {<data yang akan di update>}})```. <br /><br />
![ss langkah 14](../Screenshot/Modul2/ss14.png) <br /><br />

### Langkah 8
Lakukan perubahan publisher menjadi "Yen Press" pada semua buku "Osamu Dazai" dengan menggunakan command ```db.books.updateMany({<filter>}, {$set: {<data yang akan di update>}})```. <br /><br />
![ss langkah 15](../Screenshot/Modul2/ss15.png) <br /><br />

### Langkah 9
Lakukan penghapusan pada buku "Overlord I" dengan menggunakan command ```db.books.deleteOne({<argument>})```. <br /><br />
![ss langkah 16](../Screenshot/Modul2/ss16.png) <br /><br />

### Langkah 10
Lakukan penghapusan pada semua buku "Osamu Dazai" dengan menggunakan command ```db.books.deleteMany({<argument>})```. <br /><br />
![ss langkah 17](../Screenshot/Modul2/ss17.png) <br /><br />