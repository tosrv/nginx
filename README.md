# nginx

## 📦 Instalasi Nginx di Linux (Ubuntu/Debian)

Dokumentasi ini menjelaskan langkah-langkah untuk menginstal dan menjalankan Nginx di sistem operasi berbasis Debian seperti Ubuntu.

---

## 🔧 Langkah-langkah Instalasi

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl status nginx
```

Jika Nginx berhasil diinstal, kamu akan melihat status active (running).

## 🚀 Mengakses Nginx

Setelah Nginx aktif, buka browser dan akses:  
http://localhost  

Atau, jika server menggunakan IP publik:  
http://<IP-SERVER-KAMU>  

Kamu akan melihat halaman default Nginx seperti ini:  
    "Welcome to nginx!"  

## 🔄 Perintah Umum Nginx

Start Nginx
```bash
sudo systemctl start nginx
```
Stop Nginx
```bash
sudo systemctl stop nginx
```
Restart Nginx
```bash
sudo systemctl restart nginx
```
Reload konfigurasi tanpa restart penuh
```bash
sudo systemctl reload nginx
```
Cek status
```bash
sudo systemctl status nginx
```
## 📁 Lokasi Konfigurasi Utama

Konfigurasi utama: /etc/nginx/nginx.conf  
Site tersedia: /etc/nginx/sites-available/  
Site aktif: /etc/nginx/sites-enabled/  
Root default: /var/www/html  

## 🔍 Mengecek Sintaks Konfigurasi

Sebelum merestart/reload Nginx setelah mengedit konfigurasi:
```bash
sudo nginx -t
```
## 🧯 Uninstall Nginx

Jika ingin menghapus Nginx dari sistem:

sudo apt remove nginx -y  
sudo apt purge nginx -y  
sudo apt autoremove  

## 📝 Lisensi

Dokumentasi ini dilisensikan di bawah MIT License.
