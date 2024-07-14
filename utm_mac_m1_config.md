# Install Debian i3 dan Konfigurasi UTM Pada MBA M1 (Apple Silicon Chip - 2024)

## Install UTM via Homebrew [^1]

1. Buka terminal, lalu ketikan : \
   `brew install --cask utm`

2. Tunggu sampai proses download dan instalasi selesai pada terminal

## Install Prebuilt Debian i3

1. Buka aplikasi UTM dan pilih menu `Create a New Virtual Machine`, lalu pada window Start pilih `Download prebuilt from UTM Gallery`

2. Kemudian browser Safari akan mengarahkan ke galery OS prebuilt dari UTM [^2], tetapi dari sekian banyak yang OS yang ditampilkan kita pilih prebuilt OS `Debian 10.4 (Custom i3) - arm64` dan selanjutnya diarahkan halaman detail OS yang dipilih

3. Pada halaman ini akan menampilkan beberapa opsi, tapi untuk saat ini kita pilih `Open in UTM` dan akan muncul notifkasi bahwa _UTM akan membuka halaman ini_, selanjutnya pilih saja `Allow` dan tunggu sampai proses download OS selesai.

4. OS Debian i3 telah didownload telah otomatis terinstal pada UTM \
   Harap dicatat konfigurasi root serta default username dan password untuk dilanjutkan ke tahap berikutnya
   | User | Username | Password |
   | :---: | :---: | :---: |
   | Root | `root` | `password` |
   | Default | `debian` | `debian` |

> [!NOTE]  
> Pada tahap ini Debian i3 sudah bisa digunakan tapi akan dikustomasi sesuai kebutuhan

## Konfigurasi Debian i3

### Update Debian

1. Jalankan OS Debian [^3] yang telah didownload pada langkah sebelumnya, masukan username `debian` dan password `debian` untuk **default user** pada tampilan login

2. Ketik `command + return` untuk membuka jendela terminal

### Konfigurasi i3

## Penutup

[^1]: Jika tidak terbiasa menggunakan terminal, bisa mendownload melalui link <https://mac.getutm.app> dan instalasi file .dmg seperti biasa
[^2]: Akan diarahkan ke halaman gallery prebuilt OS dari UTM di <https://mac.getutm.app/gallery/>, beberapa OS memiliki penjelasan bahkan sampai tutorial instalasi terpisah
[^3]: Perlu diingat, bahwa OS prebuilt dari galeri UTM adalah `Debian 10.4` untuk arsitektur arm64 (Apple Silicon), sementara untuk versi terbaru dari website Debian saat ini (per 14 Juli 2024) adalah `Debian 12.6` untuk arsitektur arm64 (Apple Silicon) yang direlease bulan Juni 2024 kemarin, sehingga kita akan melalukan update dan upgrade dari Debian 10 ke 11, setelah itu baru 11 ke 12.
