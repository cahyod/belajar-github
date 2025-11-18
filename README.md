# Belajar Github
### Belajar menggunakan Git

Posisi kursor ada di folder yang akan dilakukan sinkronisasi ke Github.

0. `git init` berhasil dan sekarang folder `belajar-github` sudah menjadi repository Git. Selanjutnya, kamu bisa melakukan langkah-langkah berikut sesuai kebutuhan.

### 📌 Langkah Umum Setelah `git init`

1. **Cek status repo**

   ```bash
   git status
   ```

2. **Tambahkan file ke staging**

   ```bash
   git add .
   ```

   atau pilih file tertentu:

   ```bash
   git add nama_file
   ```

3. **Commit perubahan**

   ```bash
   git commit -m "Initial commit"
   ```

4. **(Opsional) Tambahkan remote origin GitHub / GitLab**
   Contoh GitHub:

   ```bash
   git remote add origin https://github.com/cahyod/kobedork-app.git
   ```
   Pindah URL
   
   ```bash
   git remote set-url origin https://github.com/OWASP/www-chapter-surabaya.git
   ```

5. **Push ke remote**
   Jika branch default kamu adalah `master` atau `main`, sesuaikan:

   ```bash
   git push -u origin main
   ```

   atau

   ```bash
   git push -u origin master
   ```

### 💡 Tips

* Untuk memastikan branch default kamu:

  ```bash
  git branch -M main
  ```

* Buat file `.gitignore` agar file tidak penting tidak ikut ke repo, misal Node.js:

  ```bash
  npx gitignore node
  ```

  atau manual:

  ```bash
  nano .gitignore
  ```