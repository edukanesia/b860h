# Cara aktifkan wifi b860h v1/v2 armbian kernel 5.9.0 dan lainnya.
DTB untuk B860H agar WIFI internal berfungsi dengan baik.


Cara aktifkan wifi b860h v1/v2 armbian kernel 5.9.0 dan lainnya.
1. Login sebagai **root** user
2. Masuk ke folder **$ cd /boot/dtb/amlogic**
3. Copy file dtb amlogic dengan cara
4. '$ git clone' https://github.com/edukanesia/b860h.git
5. Edit file /boot/extlinux/extlinux.conf arahkan ke dtb yg dicopy
![276145324_2984455218523043_5375553760803676421_n](https://user-images.githubusercontent.com/102713707/160979667-a68f24cc-279d-4f69-8d91-a60173ecd592.jpg)
6. **Reboot**

Cara mengetahui wifi internal sudah aktif
Cek di terminal ' **dmesg |grep SDIO** '
kalo ada tulisan '**mmc2: new high speed SDIO card at address 0001**' berarti sukses
untuk driver wifi sudah ada di bawaan kernel 5.9.0 jadi otomatis terdetek

![277173901_2984455175189714_1567733966799583371_n](https://user-images.githubusercontent.com/102713707/160979662-d71e9975-e976-4c1b-8796-cec8e125519a.jpg)
![276137689_2984455195189712_5039484187729743701_n](https://user-images.githubusercontent.com/102713707/160979665-2dd9d2ff-6ad2-4d30-94e5-4eaf46235d56.jpg)

**Thanks for 
[Mas Sidik Hakim](https://www.facebook.com/groups/447949046027700/user/100008757824674/)**




