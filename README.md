# b860h
DTB untuk B860H agar WIFI internal berfungsi dengan baik.


Cara aktifkan wifi b860h v1/v2 armbian kernel 5.9.0 dan lainnya.
1. Login sebagai root user
2. Masuk ke folder /boot/dtb/amlogic
3. Copy file dtb amlogic 
    $ git clone 
4. Edit file /boot/extlinux/extlinux.conf arahkan ke dtb yg dicopy
5. Reboot

Cara mengetahui wifi internal sudah aktif
Cek di terminal ' dmesg |grep SDIO '
kalo ada tulisan 'mmc2: new high speed SDIO card at address 0001' berarti sukses
untuk driver wifi sudah ada di bawaan kernel 5.9.0 jadi otomatis terdetek
