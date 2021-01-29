extensions  `php-beast`  diperlukan baik untuk mengenkripsi script php maupun menjalankan script yang telah dienkripsi.

berikut langkah untuk menginstall php-beast di Linux:

1. buka terminal lalu jalankan perintah: 
```
$ wget https://github.com/liexusong/php-beast/archive/master.zip
$ unzip master.zip
$ cd php-beast-master
$ phpize
$ ./configure
$ sudo make && make install
```
2. tambahkan  `extension=beast.so` pada  `php.ini` lalu restart server.

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

Jika terjadi kesalahan 502, biasanya hal itu disebabkan oleh versi GCC yang terlalu rendah. coba tingkatkan versi GCC nya dan lakukan instalasi ulang extension php-beast. 

Author : github.com/guangrei