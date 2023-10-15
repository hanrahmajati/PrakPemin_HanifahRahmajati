# Modul 4 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 4 Pemrograman Integratif TI-A - Basic Routing dan Migration</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## GET
### Langkah 1
Membuka file "web.php" pada folder "routes" dan menambahkan kode berikut. Jalankan aplikasi menggunakan command ```php -S localhost:8000 -t public``` pada terminal VS CODE <br /><br />
![ss langkah 1](../Screenshot/Modul4/ss1.png) <br /><br />

### Langkah 2
Buka browser dan akses path ```http://localhost:8000/get``` <br /><br />
![ss langkah 2](../Screenshot/Modul4/ss2.png) <br /><br />

## POST, PUT, PATCH, DELETE, dan OPTIONS
### Langkah 1
Tambahkan method POST, PUT, PATCH, DELETE, dan OPTIONS pada file "web.php" di folder "routes" dengan code berikut <br /><br />
![ss langkah 3](../Screenshot/Modul4/ss3.png) <br /><br />

### Langkah 2
Install ekstensi Thunder Client di VS CODE <br /><br />
![ss langkah 4](../Screenshot/Modul4/ss4.png) <br /><br />

### Langkah 3
Klik icon petir pada sidebar kiri di VS CODE kemudian klik button "New Request" untuk membuat request baru. <br /><br />
![ss langkah 5](../Screenshot/Modul4/ss5.png) <br /><br />

### Langkah 4
Masukkan method dan URL yang sesuai. <br /><br />
GET <br /><br />
![ss langkah 6](../Screenshot/Modul4/ss6.png) <br /><br />
POST <br /><br />
![ss langkah 7](../Screenshot/Modul4/ss7.png) <br /><br />
PUT <br /><br />
![ss langkah 8](../Screenshot/Modul4/ss8.png) <br /><br />
DELETE <br /><br />
![ss langkah 9](../Screenshot/Modul4/ss9.png) <br /><br />
PATCH <br /><br />
![ss langkah 10](../Screenshot/Modul4/ss10.png) <br /><br />
OPTIONS <br /><br />
![ss langkah 11](../Screenshot/Modul4/ss11.png) <br /><br />

## Migrasi Database
### Langkah 1
Akses server database melalui ```localhost/phpmyadmin``` dan buat database baru bernama "lumenapi". <br /><br />
![ss langkah 12](../Screenshot/Modul4/ss12.png) <br /><br />

### Langkah 2
Ubah konfigurasi database pada file .env sesuai server yang digunakan. Pada percobaan ini, database menggunakan port 3306 dan tidak menggunakan password sehingga password di-set kosong. <br /><br />
![ss langkah 13](../Screenshot/Modul4/ss13.png) <br /><br />

### Langkah 3
Aktifkan library bawaan Lumen pada file "app.php" di folder "bootstrap" dengan menghapus tanda comment yang ada. <br /><br />
![ss langkah 14](../Screenshot/Modul4/ss14.png) <br /><br />

### Langkah 4
Jalankan command ```php artisan make:migration create_users_table``` untuk membuat migrasi tabel users serta command ```php artisan make:migration create_products_table``` untuk membuat migrasi tabel produts pada terminal. <br /><br />
![ss langkah 15](../Screenshot/Modul4/ss15.png) <br /><br />

### Langkah 5
Ubah fungsi up pada file migrasi create_users_table. <br /><br />
![ss langkah 16](../Screenshot/Modul4/ss16.png) <br /><br />

### Langkah 6
Ubah fungsi up pada file migrasi create_products_table. <br /><br />
![ss langkah 17](../Screenshot/Modul4/ss17.png) <br /><br />

### Langkah 7
Jalankan command ```php artisan migrate``` pada terminal untuk melakukan migrasi tabel yang sudah dibuat. <br /><br />
![ss langkah 18](../Screenshot/Modul4/ss18.png) <br /><br />