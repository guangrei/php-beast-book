extensions  `php-beast`  diperlukan baik untuk mengenkripsi script php maupun menjalankan script yang telah dienkripsi.

berikut langkah untuk menginstall php-beast diwindows:

1. download  **php-beast.dll**  binary untuk windows [disini](https://github.com/imaben/php-beast-binaries). 

2. pilih binary sesuai dengan versi php yang digunakan dan pindahkan binary yg telah didownlod ke folder extension, misalnya  `C:\xampp\php\ext\`. 

3. tambahkan  `extension=beast.dll` pada  `php.ini` lalu restart server.

4. konfigurasi lanjutan juga dapat ditambahkan pada php.ini untuk meningkatkan performa dll

beriku ini konfigurasinya:

```

beast.cache_size = size

beast.log_file = "path_to_log"

beast.log_user = "user"

beast.log_level = "debug"

beast.enable = On

```

- **beast.cache_size**: adalah variabel yg menentukan ukuran cache.

-  **beast.log_file**: adalah variabel dimana lokasi untuk menulis log file.

-  **beast.log_level**: level log, pilihan yang dapat digunakan  **DEBUG**,  **NOTIFICATION** ,  **ERROR**.

-  **beast.enable**: variable ini digunakan untuk mengaktifkan fungsi  `php-beast`  jika tidak diatur maka php-beast tidak aktif namun dapat diaktifkan secara dynamic dengan fungsi php  `ini_set()`.

## troubleshooting

jika terjadi error Proses FastCGI keluar secara tidak normal di lingkungan IIS maka ubah  `ApplicationPoolIdentity`  ke  `LocalSystem`.

Author : github.com/guangrei
