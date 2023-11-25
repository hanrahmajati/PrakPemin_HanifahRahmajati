# Modul 9 Pemrograman Integratif TI-A

<div align="center">
<strong><p>Modul 9 Pemrograman Integratif TI-A - JSON Web Token (JWT)</p></strong>
<strong><p>Hanifah Rahmajati - 215150700111049</p></strong>
</div>  
  
## Penyesuaian Database
### Langkah 1
Melakukan perubahan pada length kolom token dengan menghapus parameter 72 di belakangnya. <br /><br />
![ss langkah 1](../Screenshot/Modul9/ss01.png) <br /><br />

### Langkah 2
Memperbaharui migrasi dan menghapus data yang lama. <br /><br />
![ss langkah 2](../Screenshot/Modul9/ss02.png) <br /><br />

### Langkah 3
Menjalankan aplikasi pada endpoint /auth/register. <br /><br />
![ss langkah 3](../Screenshot/Modul9/ss03.png) <br /><br />

## JWT Manual
### Langkah 1
Menambahkan ketiga fungsi berikut pada AuthController.php. <br /><br />
![ss langkah 4](../Screenshot/Modul9/ss04.png) <br /><br />

### Langkah 2
Melakukan perubahan pada fungsi login. <br /><br />
![ss langkah 5](../Screenshot/Modul9/ss05.png) <br /><br />

### Langkah 3
Menambahkan keempat fungsi berikut pada Middleware/Authorization.php. <br /><br />
![ss langkah 6](../Screenshot/Modul9/ss06.png) <br /><br />

### Langkah 4
Melakukan perubahan pada fungsi handle. <br /><br />
![ss langkah 7](../Screenshot/Modul9/ss07.png) <br /><br />

### Langkah 5
Menjalankan aplikasi pada endpoint /auth/login. <br /><br />
![ss langkah 8](../Screenshot/Modul9/ss08.png) <br /><br />

### Langkah 6
Menjalankan aplikasi pada endpoint /home dengan melampirkan nilai token yang didapat setelah login pada header. <br /><br />
![ss langkah 9](../Screenshot/Modul9/ss09.png) <br /><br />

## JWT Library
### Langkah 1
Generate jwt key secara online menggunakan website Djecrety ― Django Secret Key Generator. Setelah mendapatkan secret key kita akan memasukkan secret key tersebut pada file .env dengan membuat variable baru bernama JWT_SECRET.<br /><br />
![ss langkah 10](../Screenshot/Modul9/ss10.png) <br /><br />

### Langkah 2
Melakukan instalasi package jwt firebase. <br /><br />
![ss langkah 11](../Screenshot/Modul9/ss11.png) <br /><br />

### Langkah 3
Menambahkan fungsi berikut pada file AuthController. <br /><br />
![ss langkah 12](../Screenshot/Modul9/ss12.png) <br /><br />

### Langkah 4
Melakukan perubahan pada fungsi login. <br /><br />
![ss langkah 13](../Screenshot/Modul9/ss13.png) <br /><br />

### Langkah 5
Membuat file JwtMiddleware.php. <br /><br />
![ss langkah 14](../Screenshot/Modul9/ss14.png) <br /><br />

### Langkah 6
Daftarkan middleware yang telah dibuat pada bootstrap/app.php. <br /><br />
![ss langkah 15](../Screenshot/Modul9/ss15.png) <br /><br />

### Langkah 7
Menambahkan baris pada file web.php. <br /><br />
![ss langkah 16](../Screenshot/Modul9/ss16.png) <br /><br />

### Langkah 8
Menjalankan aplikasi pada endpoint /auth/login. <br /><br />
![ss langkah 17](../Screenshot/Modul9/ss17.png) <br /><br />