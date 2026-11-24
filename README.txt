FAQIHAL STORE — WEBSITE MULTI-HALAMAN (VERSI MODERN)

File utama: index.html
Halaman: hosting.html, vps.html, web-hosting.html, Build Server.html,
developer.html, ddos-protection.html, testimoni.html, bantuan.html,
kontak.html, tos.html.

Semua tombol dan tautan pemesanan menggunakan WhatsApp Only.
Tidak ada lagi pilihan order melalui Discord. Nomor WhatsApp pemesanan:
+62 831-3897-7096.

Web Hosting dan jasa pembuatan website ditambahkan sebagai layanan baru.
Semua file HTML dan gambar harus berada dalam folder yang sama saat
diunggah ke hosting. Untuk Netlify, ekstrak ZIP lalu unggah folder ini.

Tema gelap modern, aksen emas, efek transparansi, dan penyesuaian responsif
diterapkan tanpa mengubah identitas warna utama Faqihal Store.

Catatan: detail kapasitas, harga, domain, SSL, backup, dan spesifikasi paket
Web Hosting perlu dikonfirmasi kepada pelanggan melalui WhatsApp sebelum
dipublikasikan sebagai penawaran tetap.


CLEAN URL:
File .htaccess sudah ditambahkan agar halaman dapat dibuka tanpa ekstensi .html, misalnya /web-hosting/. Upload seluruh isi ZIP ke folder public_html pada hosting Apache yang mengaktifkan mod_rewrite dan mengizinkan .htaccess (AllowOverride). Jika server menggunakan Nginx, aturan .htaccess tidak berlaku dan perlu konfigurasi Nginx.


PERBAIKAN VERCEL 404 NOT_FOUND:
File vercel.json disertakan untuk mengarahkan URL bersih seperti /hosting/ dan /web-hosting/ ke file HTML yang benar. Untuk Vercel, deploy seluruh ISI ZIP ini sebagai Root Directory (project root), sehingga index.html dan vercel.json berada langsung di root. Jangan hanya upload .htaccess; Vercel tidak memakai aturan Apache .htaccess. Setelah upload, lakukan redeploy.


PENGATURAN VERCEL YANG DIPERBAIKI:
vercel.json memakai cleanUrls dan trailingSlash bawaan Vercel. Tidak memakai
rewrite manual maupun .htaccess. Ini membuat file hosting.html bisa diakses
sebagai /hosting/, vps.html sebagai /vps/, web-hosting.html sebagai
/web-hosting/, dan seterusnya.

CARA DEPLOY:
1. Ekstrak ZIP.
2. Di Vercel, buka project yang benar lalu pilih Deployments atau gunakan
   Import Project untuk upload repository.
3. Pastikan index.html, vercel.json, dan semua file gambar berada di Root
   Directory yang sama.
4. Untuk situs HTML statis, Framework Preset pilih Other; Build Command
   dikosongkan; Output Directory gunakan . (root) atau kosong sesuai UI.
5. Deploy ulang dan buka domain deployment terbaru.
6. Jika domain utama masih menunjukkan deployment lama, periksa Project
   Settings > Domains dan pastikan domain terpasang ke project yang benar.
