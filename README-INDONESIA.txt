Cara Install:
1. Jalankan DDEPrinterServer.exe pada komputer server
2. Buka Tab "Setting" dan buat password master password untuk pertama kalinya
3. Pilih IP Server yang tersedia yang akan dikoneksikan dengan komputer klien,
4. Masukkan port (Default: 11111)
5. Tekan tombol "Create Client App" dan salin aplikasi klien yang telah dibuat (DDEPrinterClient.exe) ke komputer klien dimana perintah untuk mencetak akan dikirimkan.
6. Pada komputer klien, jalankan DDEPrinterClient.exe yang telah disalin dari server untuk pertama kalinya, jika sebelumnya komputer klien belum pernah terpasang DDEPrinter versi yang lama, maka tekan tombol "Install" pada kotak pesan yang muncul untuk mendaftarkan DDEPrinter pada protocol handler di dalam sistem. Lokasi dimana anda menjalankan DDEPrinterClient.exe akan direkam sebagai path/lokasi DDEPrinter.
7. Untuk memastikan Protocol Handler dari DDEPrinter telah terdaftar, silahkan melakukan pengujian dengan mengakses perintah dari browser komputer klien: "ddeprinter:test" atau mengklik file pintasan (Command-Test) yang telah disediakan

Informasi:
*Api Key adalah kode terenkripsi yang akan diset di dalam aplikasi klien, aplikasi klien hanya akan terkoneksi ke server tempat dimana dia dibuat, admin tidak perlu untuk melakukan konfigurasi pada aplikasi klien, admin hanya membuat aplikasi klien dengan menekan tombol "Create Client App" dan mendistribusikan aplikasi yang telah dibuat tersebut ke komputer klien.

Perintah tersedia:
1. ddeprinter:[base64_encode] -> tanpa tanda kurung
	base64_encode contains: "NamaFilePDF|NamaPrinter|LinkPDFFile|UkuranKertas|JumlahPrint"
2. ddeprinter:resumePrinter:NamaPrinter
3. ddeprinter:pausePrinter:NamaPrinter
4. ddeprinter:clearSpooling:NamaPrinter
5. ddeprinter:test

Cara menggunakan perintah:
Untuk menjalankan DDEPrinter dari Aplikasi web, anda dapat menggunaka tag html "a"
Contoh:
	<a href="ddeprinter:perintahnya_disini">
atau anda dapat memanggil dari javascript:
	window.location.href ="ddeprinter:perintahnya_disini";
atau anda dapat memanggilnya langsung dari addressbar browser pada komputer klien

Dokument yang didukung:
Hanya file PDF

Pembatasan:
Untuk keperluan ujicoba, server hanya dapat mencetak 50 kali. Setelah batasan tercapai, anda harus melakukan aktivasi untuk menggunakannya kembali.

Kontak kami:
Jika anda tertarik dengan aplikasi ini, anda dapat menghubungi kami secara langsung pada aplikasi Whatsapp atau Telegram pada +6285242703687