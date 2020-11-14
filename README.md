<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->





<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Kelompok][kelompok-shield]][kelompok-url]


<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05">
    <img src="images/logo.gif" alt="Logo" width="280" height="280">
  </a>

  <h3 align="center">Nama dan NRP kelompok</h3>

  <p align="center">
    M. Mikail Dwi K.    (05311840000028)
    <br />
    Dimas P. H.         (05311840000037)
    <br />
    <a href="https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05#daftar-isi"><strong>Lihat Daftar Isi »</strong></a>
    <br />
    <br />
    <a href="https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/tree/main/images">Gambar</a>
    ·
    <a href="https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/pulse">Grafik</a>
    ·
    <a href="https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/issues">Lihat issue</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Daftar Isi

* [Soal](#Soal)
* [Persiapan](#Persiapan)
  * [Setting Topologi](#Setting-Topologi)
  * [Setting DNS](#Setting-DNS)
* [Jawaban](#Jawaban)
  * [No 1](#No-1)
  * [No 2](#No-2)
  * [No 3](#No-3)
  * [No 4](#No-4)
  * [No 5](#No-5)
  * [No 6](#No-6)
  * [No 7](#No-7)
  * [No 8](#No-8)
  * [No 9](#No-9)
  * [No 10](#No-10)
  * [No 11](#No-11)
  * [No 12](#No-12)
  * [No 13](#No-13)
  * [No 14](#No-14)
  * [No 15](#No-15)
  * [No 16](#No-16)
  * [No 17](#No-17)



<!-- ABOUT THE PROJECT -->
## Soal
<br />

![screenshot][screenshot1]

<br />
Semeru adalah salah satu gunung yang terkenal di Jawa Timur. Bibah adalah salah satu juru kunci Semeru. Bibah ingin menyebarkan keindahan Semeru pada dunia sehingga dia membeli 3 buah server yang berada di MALANG, MOJOKERTO dan PROBOLINGGO. Server MALANG akan digunakan sebagai DNS Server Master, MOJOKERTO akan digunakan sebagai DNS Server Slave dan PROBOLINGGO akan digunakan sebagai Web Server. Selain 3 server terdapat 2 klien yang digunakan untuk testing oleh Bibah yaitu GRESIK dan SIDOARJO. Untuk menyambungkan semua jaringan tersebut Bibah memberi router di SURABAYA. 
Kalian diminta untuk membuat sebuah website utama dengan (1) alamat http://semeruyyy.pw yang memiliki (2) alias http://www.semeruyyy.pw, dan (3) subdomain http://penanjakan.semeruyyy.pw yang diatur DNS-nya pada MALANG dan mengarah ke IP Server PROBOLINGGO serta dibuatkan (4) reverse domain untuk domain utama. Untuk mengantisipasi server dicuri/rusak, Bibah minta dibuatkan (5) DNS Server Slave pada MOJOKERTO agar Bibah tidak terganggu menikmati keindahan Semeru pada Website. Selain website utama Bibah juga meminta dibuatkan (6) subdomain dengan alamat http://gunung.semeruyyy.pw yang didelegasikan pada server MOJOKERTO dan mengarah ke IP Server PROBOLINGGO. Bibah juga ingin memberi petunjuk mendaki gunung semeru kepada anggota komunitas sehingga dia meminta dibuatkan (7) subdomain dengan nama 
http://naik.gunung.semeruyyy.pw, domain ini diarahkan ke IP Server PROBOLINGGO. 
Setelah selesai membuat keseluruhan domain, kamu diminta untuk segera mengatur web server. (8) Domain http://semeruyyy.pw memiliki DocumentRoot pada /var/www/semeruyyy.pw. Awalnya web dapat diakses menggunakan alamat http://semeruyyy.pw/index.php/home. Karena dirasa alamat urlnya kurang bagus, maka (9) diaktifkan mod rewrite agar urlnya menjadi http://semeruyyy.pw/home. (10) Web http://penanjakan.semeruyyy.pw akan digunakan untuk menyimpan assets file yang
memiliki DocumentRoot pada /var/www/penanjakan.semeruyyy.pw dan memiliki struktur folder sebagai berikut: 
* /var/www/penanjakan.semeruyyy.pw 
* /public/javascripts 
* /public/css 
* /public/images 
* /errors 

(11) Pada folder /public dibolehkan directory listing namun untuk folder yang berada di dalamnya tidak dibolehkan. (12) Untuk mengatasi HTTP Error code 404, disediakan file 404.html pada folder /errors untuk mengganti error default 404 dari Apache. (13) Untuk mengakses file assets javascript awalnya harus menggunakan url http://penanjakan.semeruyyy.pw/public/javascripts. Karena terlalu panjang maka dibuatkan konfigurasi virtual host agar ketika mengakses file assets menjadi http://penanjakan.semeruyyy.pw/js. 
Untuk web http://gunung.semeruyyy.pw belum dapat dikonfigurasi pada web server karena menunggu pengerjaan website selesai. (14) sedangkan web http://naik.gunung.semeruyyy.pw sudah bisa diakses hanya dengan menggunakan port 8888. DocumentRoot web berada pada /var/www/naik.gunung.semeruyyy.pw. Dikarenakan web http://naik.gunung.semeruyyy.pw bersifat private (15) Bibah meminta kamu membuat web http://naik.gunung.semeruyyy.pw agar diberi autentikasi password dengan username “semeru” dan password “kuynaikgunung” supaya aman dan tidak sembarang orang bisa mengaksesnya. 
Saat Bibah mengunjungi IP PROBOLINGGO, yang muncul bukan web utama http://semeruyyy.pw melainkan laman default Apache yang bertuliskan “It works!”. (16) Karena dirasa kurang profesional, maka setiap Bibah mengunjungi IP PROBOLINGGO akan dialihkan secara otomatis ke http://semeruyyy.pw. (17) Karena pengunjung pada 
/var/www/penanjakan.semeruyyy.pw/public/images sangat banyak maka semua request gambar yang memiliki substring “semeru” akan diarahkan menuju semeru.jpg.

## Persiapan
### Setting Topologi
Sebelum mejawab pertanyaan no 1, kita harus membuat topologi yang benar, buka xming dan putty, lalu buka openvpn connect, pertama konekkan vpn menggunakan .ovpn yang diberi asisten, lalu gunakan putty logi menggunakan IP pada modul sesuai kelompok, lalu buat topologi.sh menggunakan 
```bash
nano topologi.sh
```
lalu tuliskan
```sh
# Switch
uml_switch -unix switch1 > /dev/null < /dev/null &
uml_switch -unix switch2 > /dev/null < /dev/null &

# Router
xterm -T SURABAYA -e linux ubd0=SURABAYA,jarkom umid=SURABAYA eth0=tuntap,,,'ip_tuntap_tiap_kelompok' eth1=daemon,,,switch2 eth2=daemon,,,switch1 mem=96M &

# Server
xterm -T MALANG -e linux ubd0=MALANG,jarkom umid=MALANG eth0=daemon,,,switch2 mem=126M &
xterm -T MOJOKERTO -e linux ubd0=MOJOKERTO,jarkom umid=MOJOKERTO eth0=daemon,,,switch2 mem=126M &
xterm -T PROBOLINGGO -e linux ubd0=PROBOLINGGO,jarkom umid=PROBOLINGGO eth0=daemon,,,switch2 mem=126M &

# Klien
xterm -T SIDOARJO -e linux ubd0=SIDOARJO,jarkom umid=SIDOARJO eth0=daemon,,,switch1 mem=96M &
xterm -T GRESIK -e linux ubd0=GRESIK,jarkom umid=GRESIK eth0=daemon,,,switch1 mem=96M &
```
lalu seting interfaces sesuai modul, sedangkan probolinggo mirip dengan malang namun menggunakan ip probolinggo. lalu melakukan ``iptables –t nat –A POSTROUTING –o eth0 –j MASQUERADE –s 192.168.0.0/16`` pada router suarabaya lalu melakukan export.
### Setting DNS
lakukan ``apt-get update`` pada UML malang, lalu install bind9 menggunakan command ``apt-get install bind9 -y``, pada uml yang sama, gunakan konfigurasi pada ``/etc/bind/named.conf.local`` untuk menambahkan
```
zone "semerut05.pw" {
	type master;
	file "/etc/bind/jarkom/semerut05.pw";
};
```
Buat folder jarkom di dalam /etc/bind

```
mkdir /etc/bind/jarkom
```

Copykan file db.local pada path /etc/bind ke dalam folder jarkom yang baru saja dibuat dan ubah namanya menjadi semerut05.pw

```
cp /etc/bind/db.local /etc/bind/jarkom/semeruyyy.pw
```

Kemudian buka file semeruyyy.pw dan edit seperti gambar berikut dengan IP MALANG masing-masing kelompok:
```
nano /etc/bind/jarkom/semeruyyy.pw
```
<br />

![screenshot][screenshot2]

<br />

Restart bind9 dengan perintah

```
service bind9 restart

ATAU

named -g //Bisa digunakan untuk restart sekaligus debugging
```

Lalu membuat DNS Reverse(sesuai modul)

Lalu agar kita dapat mengakses website menggunakan semeruyyy.pw dan tidak perlu mengetikkan IP maka kita menggunakan cname
tambahkan, seperti gambar
<br />

![screenshot][screenshot2]

<br />
Kemudian restart bind9 dengan perintah

service bind9 restart
Lalu cek dengan melakukan ``host -t CNAME www.semeruyyy.pw`` atau ``ping www.semeruyyy.pw``. Hasilnya harus mengarah ke host dengan IP MALANG.

untuk membuat dns slave, kita gunakan server malang ``nano /etc/bind/named.conf.local`` lalu tambahkan
```
zone "semeruyyy.pw" {
    type master;
    notify yes;
    also-notify { "IP MOJOKERTO"; }; // Masukan IP MOJOKERTO tanpa tanda petik
    allow-transfer { "IP MOJOKERTO"; }; // Masukan IP MOJOKERTO tanpa tanda petik
    file "/etc/bind/jarkom/semeruyyy.pw";
};
```
Lakukan restart bind9

``service bind9 restart``

lalu pada mojokerto, update package lists dengan menjalankan command:

``apt-get update`` lalu ``apt-get install bind9 -y`` kemudian ``nano /etc/bind/named.conf.local`` tambahkan
```
zone "semeruyyy.pw" {
    type slave;
    masters { "IP MALANG"; }; // Masukan IP MALANG tanpa tanda petik
    file "/var/lib/bind/semeruyyy.pw";
};
```
<br />

![screenshot][screenshot3]

<br />

Lakukan restart bind9

``service bind9 restart``

membuat sub domain ``nano /etc/bind/jarkom/semerut05.pw`` tambahkan seperti gambar
<br />

![screenshot][screenshot4]

<br />

lalu ``service bind9 restart``
lalu coba ping apakah berhasil

<br />

![screenshot][screenshot5]

<br />

setelah itu membuat delegasi sub-domain ``nano /etc/bind/jarkom/semerut05.pw`` pada malang

<br />

![screenshot][screenshot2]

<br />

lalu ``service bind9 restart``

## Setting Web Service


## Jawaban
<!-- GETTING STARTED -->
### No 1

pada soal pertama, kita disuruh membuat website dengan alamat http://semeruyyy.pw.

<br />

![screenshot][screenshot6]

<br />

### No 2

pada soal pertama, kita disuruh membuat alias website dengan alamat http://www.semeruyyy.pw.

<br />

![screenshot][screenshot7]

<br />

### No 3

pada soal pertama, kita disuruh membuat subdomain website dengan alamat http://penanjakan.semeruyyy.pw.

<br />

![screenshot][screenshot8]

<br />

### No 4

Reverse Domain

<br />

![screenshot][screenshot9]

<br />

### No 5

Slave DNS

<br />

![screenshot][screenshot10]

<br />

### No 6

Subdomain delegasi

<br />

![screenshot][screenshot11]

<br />

### No 7

Subdomain delegasi

<br />

![screenshot][screenshot12]

<br />

### No 8

Subdomain delegasi

<br />

![screenshot][screenshot12]

<br />



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/peacefulhack/Jarkom_Modul2_Lapres_T05?style=flat-square
[contributors-url]: https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/graphs/contributors
[stars-shield]: https://img.shields.io/packagist/stars/peacefulhack/Jarkom_Modul2_Lapres_T05?style=flat-square
[stars-url]: https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/stargazers
[kelompok-shield]: https://img.shields.io/badge/Kelompok-T05-blue
[kelompok-url]: https://github.com/peacefulhack/Jarkom_Modul2_Lapres_T05/
[screenshot1]: images/screenshot1.png
[screenshot2]: images/ss2.png
[screenshot3]: images/ss3.png
[screenshot4]: images/ss4.png
[screenshot5]: images/ss5.png
[screenshot6]: images/ss6.png
[screenshot7]: images/ss7.png
[screenshot8]: images/ss8.png
[screenshot9]: images/ss9.png
[screenshot10]: images/ss10.png
[screenshot11]: images/ss11.png
[screenshot12]: images/ss12.png
[screenshot13]: images/ss13.png
[screenshot14]: images/ss14.png
[screenshot15]: images/ss15.png
[screenshot16]: images/ss16.png
