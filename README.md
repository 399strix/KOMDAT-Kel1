<h1 align="center"><img src="https://i.pinimg.com/564x/e9/9e/d1/e99ed1d4a8bd897c2774a8756faced11.jpg"></h1>
<h2 align="center">Aplikasi Web "GHOST"</h2>

[Sekilas Tentang](#sekilas-tentang) | [Instalasi](#instalasi) | [Konfigurasi](#konfigurasi) | [Maintenance](#maintenance) | [Otomatisasi](#otomatisasi) | [Cara Pemakaian](#cara-pemakaian) | [Pembahasan](#pembahasan) | [Referensi](#referensi)

# Sekilas Tentang

Ghost merupakan salah satu platform Content Management System seperti Wordpress yang bersifat open source. Seperti Wordpress, Ghost digunakan untuk membuat, mempromosikan dan mengelola konten dengan interface yang lebih modern, sederhana dan intuitif.


# Instalasi

- Prasyarat, apa saja yang harus diinstal sebelumnya.
- Langkah instalasi dalam CLI
1.	Instal instance
2.	Root.
 ```
$ sudo service apache2 restart
 ```
3.	Membuat user dan loginn ssh 
```
$adduser komdat
```
4.	Mengubah user menjadi superuser serta login sebagai user
```
$usermod -aG sudo komdat , su -komdat
```
5.	Menginstal dan memastikan package yang terbaru sudah terinstal 
```
$sudo apt get update
$sudo apt get upgrade
```
6.	Instal king server “NGINX”, dan follow ‘NGINX’
```
$sudo apt-get install nginx
$sudo ufw allows ‘Nginx Full’
```
7.	Install MySql 
```
$sudo apt-get install mysql-server
```
8.	Install framework Node.js
```
$curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash
$sudo apt-get install -y node.js
```
9.	Install ghost client 
```
$sudo npm install ghost-cli@latest -g 
```
10.	Create directory 
```
$sudo mkdir -p /var/www/komdat-ghost
$sudo chown komdat:komdat /var/www/komdat-ghost
$cd /var/www/komdat-ghost
```
11.	Install process 
```
$ghost install
```
12.	Set blog URL dan set up system 
```
$http://34.101.93.101
```

#  Maintenance (opsional)

Setting tambahan untuk maintenance secara periodik, misalnya:
- membuat backup konten
Pada menu Labs yang bisa kita akses dengan menekan tombol roda gigi dibawah, terdapat menu Import, Export dan Delete Content. Menu Export digunakan untuk membackup konten secara manual. Meskipun backup dilakukan dengan manual, setidaknya konten yang dibuat bisa dikembalikan sewaktu-waktu terjadi hal yang tidak diinginkan.


# Cara Pemakaian

1.	Buka halaman Admin dari web
![image](https://user-images.githubusercontent.com/86305950/196965927-6f3627d3-220c-4855-8451-1c6b867b8d5f.png)
 
2.	Masuk ke Dashboard
Dasbor : merupakan laman dasbor setelah login admin, disini kita bisa melihat berbagai informasi yang tersedia pada website kita.
 ![image](https://user-images.githubusercontent.com/86305950/196965972-0cb685a7-cd2d-489d-b24e-053d6ede556d.png)
 ![image](https://user-images.githubusercontent.com/86305950/196967846-da868a80-e1d6-4fa7-b1f6-fb36eb642596.png)
  
3.	Menu View Site 
digunakan untuk melihat bagaimana website kita ditampilkan pada  pengguna.
 ![image](https://user-images.githubusercontent.com/86305950/196967875-ce01a134-0036-428b-9a44-07f431105288.png)

4.	Menu Post
digunakan untuk menampilkan konten apa saja yang sudah diterbitkan.
 ![image](https://user-images.githubusercontent.com/86305950/196967884-355a1094-0b9c-4067-85b3-831048682f31.png)

5.	Menu Draft
disini konten yang masih belum selesai/ belum siap ditampilkan disimpan.
 ![image](https://user-images.githubusercontent.com/86305950/196967896-d87d4342-4e34-462a-9c0f-783ecd317d55.png)

6.	Menu Scheduled
digunakan untuk menjadwalkan konten agar dapat tampil pada waktu tertentu secara otomatis
  ![image](https://user-images.githubusercontent.com/86305950/196967915-d3880c0b-accc-497c-8fae-0c62feb1df75.png)
  
7.	Post Settings 
berisi pengaturan mengenai konten yang akan dibuat.

  ![image](https://user-images.githubusercontent.com/86305950/196967938-cfd0fa4d-f663-47fe-8697-d04e49cc905e.png)

8.	Menu Publish
digunakan untuk melakukan penerbitan konten. Disini juga bisa diatur tentang kepada siapa konten akan diterbitkan serta penentuan jadwal kapan konten akan diterbitkan.
![image](https://user-images.githubusercontent.com/86305950/196967962-7fece3eb-5e79-4c8c-b094-d6991ef990f7.png)
![image](https://user-images.githubusercontent.com/86305950/196967989-ca6be152-c232-4400-86f1-e0330c6ff97b.png)
![image](https://user-images.githubusercontent.com/86305950/196967998-66966903-94b9-4680-9e8f-207d079374f0.png)

9.	 Menu Preview
mensimulasikan bagaimana konten akan diterbitkan nantinya. Terdapat pilihan preview untuk 4 pilihan ( komputer, mobile device, e-mail dan twitter).
 ![image](https://user-images.githubusercontent.com/86305950/196968019-aeb11088-f889-4585-a277-ecc0780ae3e9.png)

10.	Menu Pages
menampilkan halaman.
 ![image](https://user-images.githubusercontent.com/86305950/196968113-8aa52dcc-a633-4446-b09c-a659f88efe7a.png)

11.	Menu Tag 
untuk menambahkan tag agar postingan lebih mudah dikategorikan.
 ![image](https://user-images.githubusercontent.com/86305950/196968135-5c0f96f6-1867-43ee-814e-5c0f1fc0f82f.png)

12.	 Menu Members
menambahkan dan menampilkan daftar pengguna yang akan berlangganan atau sudah berlangganan untuk mengakses konten eksklusif.
![image](https://user-images.githubusercontent.com/86305950/196968161-6f80e221-3e3a-4513-a176-14af37676e69.png)
![image](https://user-images.githubusercontent.com/86305950/196968179-9abc56a9-a869-4931-9b26-eea660406cb9.png)


- Tampilan aplikasi web
<h1 align="center"><img src="https://user-images.githubusercontent.com/86305950/196953394-700c688b-5e91-4e7a-9aa5-c8ed6461af29.png"></h1>
<h2 align="center">Halaman utama website yang sudah dibuat</h2>

- Contoh konten yang sudah di-_publish_
![image](https://user-images.githubusercontent.com/86305950/196955987-d9314a36-c8e6-46df-b42f-68bafedc0e61.png)


# Pembahasan

Content Management System merupakan sebuah platform sistem yang digunakan untuk membantu penggunanya membuat, manajemen dan memodifikasi konten pada sebuah website tanpa membutuhkan keahlian teknis tertentu. Sederhananya, CMS merupakan alat untuk membuat website tanpa melakukan koding. 

Saat ini, sudah banyak CMS populer telah hadir seperti Wordpress, Magento, Joomla, Drupla, Wix dan Ghost. Ghost sendiri merupakan CMS open-source yang dibangun menggunakan Node.js berdasarkan bahasa pemrograman Javascript.

Berikut keunggulan Ghost :
1.	Interface Editor Minimalis dan Intuitif
2.	Bisa Self-Hosted
3.	Performa Dapat Diandalkan
4.	Fitur Search Engine Optimization Yang Lengkap
5.	Ringan dan Fleksibel

Kelemahan Ghost :
1.	Terlalu Minimalist
2.	Hosting Mandiri Ghost Cukup Sulit
3.	Backup Web Rumit

- Pendapat anda tentang aplikasi web ini
    - kelebihan
    - kekurangan
- Bandingkan dengan aplikasi web lain yang sejenis


# Referensi

https://kinsta.com/knowledgebase/content-management-system/

https://idcloudhost.com/ghost-cms-adalah/

https://ezy.co.id/ghost-cms-pengertian-fitur-keunggulan-dan-cara-install-ghost-di-hosting/
