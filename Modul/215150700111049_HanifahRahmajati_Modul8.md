# Modul 8 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 8 Pemrograman Integratif TI-A - Register, Authentication dan Authorization</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## Register
### Langkah 1
Memastikan terdapat tabel users yang dibuat menggunakan migration pada bab 3 Basic Routing dan Migration. <br /><br />
![ss langkah 1](../Screenshot/Modul8/ss01.png) <br /><br />

### Langkah 2
Memastikan terdapat model User.php yang digunakan pada bab 5 Model, Controller dan Request-Response Handler. <br /><br />
![ss langkah 2](../Screenshot/Modul8/ss02.png) <br /><br />

### Langkah 3
Membuat file AuthController.php. <br /><br />
![ss langkah 3](../Screenshot/Modul8/ss03.png) <br /><br />

### Langkah 4
Menambahkan baris berikut pada routes/web.php. <br /><br />
![ss langkah 4](../Screenshot/Modul8/ss04.png) <br /><br />

### Langkah 5
Jalankan aplikasi pada endpoint /auth/register. <br /><br />
![ss langkah 5](../Screenshot/Modul8/ss05.png) <br /><br />

## Authentication
### Langkah 1
Membuat fungsi login(Request $request) pada file AuthController.php. <br /><br />
![ss langkah 6](../Screenshot/Modul8/ss06.png) <br /><br />

### Langkah 2
Menambahkan baris berikut pada routes/web.php. <br /><br />
![ss langkah 7](../Screenshot/Modul8/ss07.png) <br /><br />

### Langkah 3
Jalankan aplikasi pada endpoint /auth/login. <br /><br />
a. Email dan password benar. <br /><br />
![ss langkah 8](../Screenshot/Modul8/ss08.png) <br /><br />
b. Email benar, password salah. <br /><br />
![ss langkah 9](../Screenshot/Modul8/ss09.png) <br /><br />

## Token
### Langkah 1
Membuat migrasi baru. <br /><br />
![ss langkah 10](../Screenshot/Modul8/ss10.png) <br /><br />

### Langkah 2
Menambahkan kode pada migrasi yang sudah dibuat. <br /><br />
![ss langkah 11](../Screenshot/Modul8/ss11.png) <br /><br />

### Langkah 3
Menambahkan atribut token di $fillable pada User.php. <br /><br />
![ss langkah 12](../Screenshot/Modul8/ss12.png) <br /><br />

### Langkah 4
Menambahkan baris kode pada file AuthController.php. <br /><br />
![ss langkah 13](../Screenshot/Modul8/ss13.png) <br /><br />

### Langkah 5
Menjalankan php artisan migrate untuk menjalankan migrasi terbaru. <br /><br />
![ss langkah 14](../Screenshot/Modul8/ss14.png) <br /><br />

### Langkah 6
Menjalankan aplikasi pada endpoint /auth/login. <br /><br />
![ss langkah 15](../Screenshot/Modul8/ss15.png) <br /><br />

## Authorization
### Langkah 1
Membuat file Authorization.php pada folder App/Http/Middleware. <br /><br />
![ss langkah 16](../Screenshot/Modul8/ss16.png) <br /><br />

### Langkah 2
Menambahkan middleware yang baru dibuat pada bootstrap/app.php. <br /><br />
![ss langkah 17](../Screenshot/Modul8/ss17.png) <br /><br />

### Langkah 3
Membuat fungsi home() pada HomeController.php. <br /><br />
![ss langkah 18](../Screenshot/Modul8/ss18.png) <br /><br />

### Langkah 4
Menambahkan baris kode pada file routes/web.php. <br /><br />
![ss langkah 19](../Screenshot/Modul8/ss19.png) <br /><br />

### Langkah 5
Menjalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat setelah login pada header. <br /><br />
![ss langkah 20](../Screenshot/Modul8/ss20.png) <br /><br />
