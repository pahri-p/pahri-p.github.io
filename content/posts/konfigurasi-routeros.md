+++
date = '2025-05-20T14:26:56Z'
draft = false
title = 'Tutorial Konfigurasi RouterOS'
+++

Postingan ini berisi tutorial mengkonfigurasi Mikrotik RouterOS untuk memungkinkan
komunikasi antarhos, menghubungkan LAN dengan internet, memblokir situs-web, dan
membatasi bandwidth maksimal. RouterOS sendiri adalah sistem operasi yang
dikembangkan oleh Mikrotik, perusahaan Latvia, untuk perangkat keras jaringannya,
RouterBoard. 

Router Mikrotik yang digunakan untuk membangun LAN ini adalah hAP Lite, dengan
RouterOS v6. Router ini memiliki empat port Ethernet dan mendukung koneksi
nirkabel (Wi-Fi). Karena itu, *empat* komputer desktop yang dihubungkan secara 
kabel dengan router dijadikan hos; router, kemudian, untuk mendapatkan koneksi 
Internet, dihubungkan secara nirkabel dengan perangkat seluler yang memiliki akses
Internet dari ISP seluler.

Cara yang paling sederhana untuk mengkonfigurasi RouterOS adalah dengan menggunakan
CLI (command-line interface) melalui SSH (secure-shell), WinBox, atau WebFig. Pada
tutorial ini, menggunakan WinBox. Sebelum itu, unduh dulu utility tersebut di
[situs web Mikrotik](https://mikrotik.com/download/). Kemudian, hubungkan desktop
dengan router melalui port Ethernet kecuali ether1. Setelah itu, jalankan WinBox,
pilih router melalui alamat MAC-nya, dan klik **Connect**. Terakhir, reset 
konfigurasi RouterOS dengan, pada WinBox, pergi pada **Terminal** dan jalankan
perintah ini:

```
/system reset-configuration no-defaults=yes skip-backup=yes
```

Kemudian klik **Enter**, ketik "y", dan klik **Enter**. Terakhir, pada Windows
Start Menu, cari

*next ...*

Hidupkan hotspot pada smartphone (pastikan itu memiliki akses Internet), dan
jalankan lagi WinBox. Setelah berhasil terkoneksi, klik menu **Terminal**, kemudian
langkah selanjutnya adalah:

Langkah 1
: Untuk ..., jalankan
