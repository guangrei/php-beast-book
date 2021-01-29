secara default script yang dienkripsi dengan php-beast tidak bisa atau tidak mudah untuk didekripsi kecuali menambahkan opsi  `--enable-beast-debug` pada saat mengcompile php-beast extension.

jika extension dicompile dengan opsi `--enable-beast-debug` kita dapat menambahkan konfigurasi baru pada  `php.ini` berupa variabel  `beast.debug_mode` dan  `beast.debug_path`, kemudian source code (code yang didekripsi) akan tersimpan pada lokasi yang diberikan pada `beast.debug_path` disana kita dapat memastikan apakah code didekripsi dengan baik atau tidak. 

> info lain tentang security dapat ditemukan pada bagian custom extension.

Author : github.com/guangrei
