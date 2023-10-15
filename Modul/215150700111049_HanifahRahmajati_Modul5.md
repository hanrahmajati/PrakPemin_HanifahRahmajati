# Modul 5 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 5 Pemrograman Integratif TI-A - Dynamic Route dan Middleware</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## Dynamic Route
### Langkah 1
Menambahkan baris kode untuk dynamic routes pada file "web.php" pada folder "routes" seperti berikut. <br /><br />
![ss langkah 1](../Screenshot/Modul5/ss1.png) <br /><br />

### Langkah 2
Buka browser dan akses path ```http://localhost:8000/user/1``` <br /><br />
![ss langkah 2](../Screenshot/Modul5/ss2.png) <br /><br />
Buka browser dan akses path ```http://localhost:8000/user/2``` <br /><br />
![ss langkah 3](../Screenshot/Modul5/ss3.png) <br /><br />

### Langkah 3
Tambahkan paramater pada file "web.php" pada folder "routes" dengan baris kode seperti berikut. <br /><br />
![ss langkah 4](../Screenshot/Modul5/ss4.png) <br /><br />

### Langkah 4
Buka browser dan akses path ```http://localhost:8000/post/2/comments/2``` <br /><br />
![ss langkah 5](../Screenshot/Modul5/ss5.png) <br /><br />

### Langkah 5
Tambahkan optional routes pada file "web.php" pada folder "routes" dengan baris kode seperti berikut. <br /><br />
![ss langkah 6](../Screenshot/Modul5/ss6.png) <br /><br />

### Langkah 6
Buka browser dan akses path ```http://localhost:8000/users``` <br /><br />
![ss langkah 7](../Screenshot/Modul5/ss7.png) <br /><br />
Buka browser dan akses path ```http://localhost:8000/users/id``` <br /><br />
![ss langkah 8](../Screenshot/Modul5/ss8.png) <br /><br />

## Aliases Route
### Langkah 1
Menambahkan baris kode untuk aliases routes pada file "web.php" pada folder "routes" seperti berikut. <br /><br />
![ss langkah 9](../Screenshot/Modul5/ss9.png) <br /><br />

### Langkah 2
Buka browser dan akses path ```http://localhost:8000/auth/login``` <br /><br />
![ss langkah 10](../Screenshot/Modul5/ss10.png) <br /><br />

### Langkah 3
Menambahkan baris kode untuk group routes pada file "web.php" pada folder "routes" seperti berikut. <br /><br />
![ss langkah 11](../Screenshot/Modul5/ss11.png) <br /><br />

### Langkah 4
Buka browser dan akses path ```http://localhost:8000/auth/users``` <br /><br />
![ss langkah 12](../Screenshot/Modul5/ss12.png) <br /><br />

## Middleware
### Langkah 1
Copy file "ExampleMiddleware" pada "app/Http/Middleware", ubah nama file menjadi "AgeMiddleware", kemudian memasukkan baris kode berikut. <br /><br />
![ss langkah 13](../Screenshot/Modul5/ss13.png) <br /><br />

### Langkah 2
Daftarkan "AgeMiddleware" pada aplikasi dengan menambahkan baris kode berikut di dalam file bootstrap/app.php <br /><br />
![ss langkah 14](../Screenshot/Modul5/ss14.png) <br /><br />

### Langkah 3
Tambahkan route middleware dengan memasukkan baris kode berikut pada file routes/web.php <br /><br />
![ss langkah 15](../Screenshot/Modul5/ss15.png) <br /><br />

### Langkah 4
Buka browser dan akses path ```http://localhost:8000/auth/home```. Halaman akan dialihkan ke ```/fail``` karena parameter umur tidak dimasukkan pada route. <br /><br />
![ss langkah 16](../Screenshot/Modul5/ss16.png) <br /><br />