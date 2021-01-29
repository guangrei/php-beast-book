untuk mengenkripsi script php dengan php-beast adalah sangat mudah, kita dapat menggunakan tools yang sudah disediakan [disini](https://github.com/liexusong/php-beast/tree/master/tools).

### encode_file.php

berfungsi untuk mengenkripsi satu file, cara menggunakannya adalah lewat  `cmd` atau  `terminal`  dengan perintah:

```

php encode_file.php --oldfile old_file_path --newfile new_file_path --encrypt DES --expire "2016-10-10 10:10:10"

```

keterangan :

-  `--oldfile`: adalah lokasi file yang akan dienkripsi 

-  `--newfile`: adalah lokasi tempat penyimpanan hasil enkripsi. 

-  `--encrypt`: pilihan ini menunjukkan algorithm yang digunakan untuk mengenkripsi.

-  `--expire`: mengatur waktu kapan file yang dienkripsi kadaluarsa (pilihan ini optional).

### encode_files.php

berfungsi untuk mengenkripsi batch file php yang berada dalam suatu folder, cara penggunaannya dapat melalui  `terminal`  atau  `cmd`  dengan perintah  `php encode_files.php`. 

> sebelum menjalankan encode_files.php pastikan sudah mengubah file  `configure.ini` terlebih dahulu. 

Author : github.com/guangrei
