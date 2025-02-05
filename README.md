# Magisk Module Template

## [Switch to English](README_EN.md)

## Cara Membuat Modul Magisk
1. Clone / download repositori ini
2. Buka `config.sh`, ikuti instruksi yang ada di awal file. Kamu setidaknya harus mengubah `config.sh` dan `module.prop`
3. Zip file-file kamu, file ZIP yang dihasilkan adalah file flashable untuk Magisk Manager dan custom recovery
4. Harap periksa **Catatan** untuk kewaspadaan

---

## Cara Meminta Repositori Baru
1. Fork [repositori ini](https://github.com/topjohnwu/magisk-module-template)
2. Buat Modul Magisk kamu sendiri seperti yang dijelaskan di atas
3. Push perubahan kamu ke Github
4. Ubah deskripsi repositori Github menjadi **ID modul kamu. Ini penting! Jangan ubah menjadi yang lain!**
5. Buka issue di [topjohnwu/Magisk_Repo_Central](https://github.com/topjohnwu/Magisk_Repo_Central/issues/new)  
   Harap sertakan link repositorimu agar saya bisa memeriksa dan meng-clone-nya
6. Repositori kamu akan di-clone ke [Magisk-Modules-Repo](https://github.com/Magisk-Modules-Repo), dan kamu akan menerima email untuk menjadi kolaborator repositori tersebut, sehingga kamu bisa mengeditnya di masa depan.

---

## Catatan
1. (Untuk pengguna Windows!!) Repositori git ini dikonfigurasi untuk memaksa endline Unix pada semua file yang diperlukan. Pastikan baris akhir pada file ini tetap dalam format Unix. Gunakan editor teks tingkat lanjut seperti Sublime, Atom, Notepad++ dll. untuk mengedit file teks.
2. Di dalam `module.prop`, `version` bisa berupa string apapun yang kamu inginkan, jadi nama versi yang fancy (misalnya ultra-beta-v0.0.0.1) diperbolehkan. Namun, `versionCode` **HARUS** berupa angka bulat. Nilai ini digunakan untuk perbandingan versi.
3. Pastikan ID modul kamu **tidak mengandung spasi**.
4. (Untuk pengembang repositori) Magisk Manager memantau semua cabang `master` dari repositori. Jadi, setiap perubahan pada cabang `master` akan langsung diterapkan ke semua pengguna. Jika kamu sedang mengerjakan pembaruan modul, harap bekerja di cabang lain, pastikan itu berfungsi, dan kemudian gabungkan perubahan ke cabang `master`.

---

## Praktik Terbaik untuk Memperbarui Repositori
1. Buka cabang baru, dan mulai perbarui file kamu di cabang baru tersebut
2. Uji apakah semuanya berfungsi dengan baik
3. Tingkatkan `versionCode` di `module.prop`, atau Magisk Manager tidak akan tahu bahwa modul kamu diperbarui!
4. Gabungkan perubahan kembali ke cabang master, dan semua pengguna sekarang akan menerima pembaruan di Magisk Manager.


