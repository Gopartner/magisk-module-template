# Magisk Module Template

## !! Please update this README.md file for online Repo submission !!
You can edit your `README.md` within Github's online editor, it also has a preview button!  
Check the [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for markdown syntaxes, it's super easy!

---

## Cara Membuat Modul Magisk
1. Clone / download repositori ini
2. Buka `config.sh`, ikuti instruksi yang ada di awal file. Kamu setidaknya harus mengubah `config.sh` dan `module.prop`
3. Zip file-file kamu, file ZIP yang dihasilkan adalah file flashable untuk Magisk Manager dan custom recovery
4. Harap periksa **Catatan** untuk kewaspadaan

---

## How to Create a Magisk Module
1. Clone / download this repo
2. Open `config.sh`, follow the instructions written at the beginning of the file. You should at least change `config.sh` and `module.prop`
3. Zip your files, the zipped file is a flashable zip for both Magisk Manager and custom recoveries
4. Please check **Notes** for precautions

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

## How to Request a New Repo
1. Fork [this repo](https://github.com/topjohnwu/magisk-module-template)
2. Create your own Magisk Module as stated above
3. Push your changes to Github
4. Change the description of the Github repo to **the id of your module. This is important! Never change it to anything else!**
5. Open an issue in [topjohnwu/Magisk_Repo_Central](https://github.com/topjohnwu/Magisk_Repo_Central/issues/new)  
   Please include your repo link so I can check and clone it
6. Your repo should be cloned into [Magisk-Modules-Repo](https://github.com/Magisk-Modules-Repo), and you should receive an email to become the collaborator of that repo so you can edit it in the future.

---

## Catatan
1. (Untuk pengguna Windows!!) Repositori git ini dikonfigurasi untuk memaksa endline Unix pada semua file yang diperlukan. Pastikan baris akhir pada file ini tetap dalam format Unix. Gunakan editor teks tingkat lanjut seperti Sublime, Atom, Notepad++ dll. untuk mengedit file teks.
2. Di dalam `module.prop`, `version` bisa berupa string apapun yang kamu inginkan, jadi nama versi yang fancy (misalnya ultra-beta-v0.0.0.1) diperbolehkan. Namun, `versionCode` **HARUS** berupa angka bulat. Nilai ini digunakan untuk perbandingan versi.
3. Pastikan ID modul kamu **tidak mengandung spasi**.
4. (Untuk pengembang repositori) Magisk Manager memantau semua cabang `master` dari repositori. Jadi, setiap perubahan pada cabang `master` akan langsung diterapkan ke semua pengguna. Jika kamu sedang mengerjakan pembaruan modul, harap bekerja di cabang lain, pastikan itu berfungsi, dan kemudian gabungkan perubahan ke cabang `master`.

---

## Notes
1. (Windows aware!!) This git repo is configured to force Unix endlines on all necessary files. The line endings on these files should remain the Unix format. Please use advanced text editors like Sublime, Atom, Notepad++ etc. to edit the text files.
2. In `module.prop`, `version` is any string you like, so any fancy version name (e.g. ultra-beta-v0.0.0.1) is allowed. However, `versionCode` **MUST** be an integer. The value is used for version comparison.
3. Make sure your module ID **doesn't contain any spaces**.
4. (For repo developers) Magisk Manager monitors all repo's `master` branch. So any changes to the branch `master` will be reflected to all users immediately. If you are working on an update for a module, please work on another branch, make sure it works, and then merge the changes back to `master`.

---

## Praktik Terbaik untuk Memperbarui Repositori
1. Buka cabang baru, dan mulai perbarui file kamu di cabang baru tersebut
2. Uji apakah semuanya berfungsi dengan baik
3. Tingkatkan `versionCode` di `module.prop`, atau Magisk Manager tidak akan tahu bahwa modul kamu diperbarui!
4. Gabungkan perubahan kembali ke cabang master, dan semua pengguna sekarang akan menerima pembaruan di Magisk Manager.

---

## Best Practice for Updating a Repo
1. Open a new branch, and start update your files on the new branch
2. Test if everything works fine
3. Bump up the `versionCode` in `module.prop`, or Magisk Manager won't know that your module is updated!
4. Merge the changes back to master, all users shall now receive the update in Magisk Manager.

