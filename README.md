# FinalProjectWebsiteSBD
Di root project-mu (`C:\Users\Hikari Reiziq\Website\my-retail-app`) belum ada file **package.json**, jadi `npm install` memang gagal. Ikuti langkah ini:

1. **Inisialisasi package.json**
   Di folder `my-retail-app` jalankan:

   ```powershell
   npm init -y
   ```

   Ini akan membuat file `package.json` dengan konfigurasi default.

2. **Install dependencies**
   Setelah itu install library yang kita butuhkan:

   ```powershell
   npm install express mongoose cors
   ```

   Jika kamu mau, bisa tambahkan juga `npm install dotenv` untuk menyimpan connection string di `.env`.

3. **Jalankan server**
   Sekarang file `package.json` sudah ada, dependencies ter-install, kamu tinggal:

   ```powershell
   node server.js
   ```

   Lalu buka di browser ke `http://localhost:3000/login.html`.

---

> **Tip tambahan:**
>
> * Kalau nanti ingin pakai script npm, bisa edit `package.json` → bagian `"scripts"`:
>
>   ```json
>   "scripts": {
>     "start": "node server.js"
>   }
>   ```
>
>   Lalu cukup `npm start` untuk menjalankan server.
> * Pastikan struktur folder tetap:
>
>   ```
>   my-retail-app/
>   ├ server.js
>   ├ package.json
>   └ public/
>       ├ login.html
>       ├ dashboard.html
>       └ app.js
>   ```

Silakan dicoba—seharusnya setelah ini server bisa jalan tanpa error! 😊

npm install       # sekali saja untuk install dependencies
node server.js

