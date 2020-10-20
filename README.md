# shadowsocks-all

<h1 align="center">Run The ShadowsocksR Auto-Installer</h1>

<h3 align="center">Supported Linux Distribution</h3>
<p align="center">
  <a><img src="https://img.shields.io/badge/Support-CentOS 6+-red.svg"></a>
  <a><img src="https://img.shields.io/badge/Support-Debian%207+-red.svg"></a>
  <a><img src="https://img.shields.io/badge/Support-Ubuntu%2012+-red.svg"></a>
</p>
<h3 align="center">Services</h3>
<p align="center">
  <a><img src="https://img.shields.io/badge/Service-Shadowsocks Python-green.svg"></a>
  <a><img src="https://img.shields.io/badge/Service-Shadowsocks R-green.svg"></a>
  <a><img src="https://img.shields.io/badge/Service-Shadowsocks Go-green.svg"></a>
  <a><img src="https://img.shields.io/badge/Service-Shadowsocks Libev-green.svg"></a>
 </p>
 
$ wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/gugun09/shadowsocks_install/main/shadowsocks-all.sh
$ chmod +x shadowsocks-all.sh
$ ./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log

Notes: Ini berisi installer untuk paket Shadowsocks lainnya juga.

# Penginstal akan membuat dan menampilkan konfigurasi akhir. Ini menampilkan IP Pribadi (bukan IP publik). Jadi pastikan Anda menggunakan IP Publik dalam aplikasi klien. Seperti yang saya sebutkan sebelumnya, Anda dapat menemukan IP publik Anda dalam halaman instans AWS EC2 yang sesuai atau menjalankan perintah di bawah ini untuk menampilkan IP publik

$ wget -qO- -t1 -T2 ipinfo.io/ip


# Commands to start | stop | restart | status

Shadowsocks-Python：

$ /etc/init.d/shadowsocks-python start | stop | restart | status

ShadowsocksR：

$ /etc/init.d/shadowsocks-r start | stop | restart | status


Shadowsocks-Go：

$ /etc/init.d/shadowsocks-go start | stop | restart | status


Shadowsocks-libev：

$ /etc/init.d/shadowsocks-libev start | stop | restart | status
