---
layout: post
title: "Konfigurasi RouterOS"
author: "Pahri Permana"
---

Postingan ini memberikan tutorial mengkonfigurasi RouterOS dari
router Mikrotik untuk membangun LAN. Router ini adalah Mikrotik
hAP Lite menggunakan OS RouterOS v6 dengan 4 port Ethernet,
dan memiliki WAP, firewall, dan switch. LAN terdiri dari
4 komputer Windows, 1 router, dan 1 ponsel pintar. Komputer
dihubungkan dengan router, dan router dihubungkan dengan ponsel
pintar. Ponsel tersebut memiliki koneksi Internet melalui ISP 
seluler, dan meng-tether koneksi tersebut kepada router supaya LAN
memiliki akses Internet.

## Persiapan

Langkah pertama adalah merencanakan LAN yang ingin dibangun,
kemudian menyiapkan hal-hal yang dibutuhkan, misalnya komponen
jaringan, sesuai dengan rancangan itu. Kemudian menghubungkan
komponen dengan pasangannya sesuai dengan rancangan LAN. Setelah
itu mengkonfigurasi komponen-komponen tersebut sehingga berjalan
sesuai rencana atau keinginan.

Pada postingan ini, komputer dihubungkan pada router dengan
memasangkan kabel Ethernet pada port komputer dan router.
Kemudian mengkonfigurasi router untuk memberikan informasi
konfigurasi pada komputer yang terhubung, sehingga komputer
dapat mengirim dan dan menerima data.

Untuk mengkonfigurasi router yang ber-OS RouterOS, maka RouterOS
harus diakses terlebih dahulu. Untuk mengakses RouterOS, dapat
menggunakan CLI (atau console) melalui WinBox, SSH, atau telnet,
atau menggunakan GUI melalui WinBox atau WebFig. CLI lebih
sederhana, tetapi GUI lebih familiar bagi kebanyakan orang. Maka
pada postingan ini, menggunakan CLI.

## Tutorial Konfigurasi RouterOS

Unduh WinBox di [situs-web resmi](https://mikrotik.com/download),
kemudian jalankan. Pada WinBox, isikan alamat MAC atau alamat
IP router, dan username dan password, kemudian klik **Connect**.

