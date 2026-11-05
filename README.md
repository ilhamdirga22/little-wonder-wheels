# Little Wonder Wheels — Wonder Island

Game 3D sederhana untuk anak, berbasis Three.js. **Versi: playable web release candidate 1.0**.

## Fitur
- Pulau 3D pastel dengan rumah, pepohonan, bunga, sungai, dan Bibi si kelinci.
- Ride: sepeda otomatis maju; tahan tombol kiri/kanan untuk belok.
- Build: tekan Place tiga kali untuk membuat jembatan.
- Paint: pilih warna, lalu sentuh bunga, pohon, atau balok jembatan.
- Wonder Book: tiga bintang pencapaian (jembatan, mewarnai, bertemu Bibi).
- Warna sepeda bisa diganti di Settings.
- Progres tersimpan secara lokal di browser, tanpa akun.
- PWA/service worker untuk caching setelah akses online pertama (bergantung dukungan browser).

## Cara menjalankan
1. Ekstrak ZIP. Jangan mengubah struktur folder.
2. Jalankan server lokal dari folder proyek, misalnya `python -m http.server 8000`.
3. Buka `http://localhost:8000` di browser desktop. Untuk Android, gunakan GitHub Pages (HTTPS).
4. Three.js dimuat dari CDN pada akses pertama, jadi perlu internet pada saat itu.

## GitHub Pages
1. Buat repository baru dan upload **semua file di folder ini** ke root branch `main`.
2. Repository → Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
3. Buka alamat yang diberikan GitHub Pages, misalnya `https://USERNAME.github.io/REPO/`.
4. Buka di Chrome Android, putar HP landscape, lalu pilih **Ayo Main!**.

## Kontrol
- Ride: kiri/kanan layar, atau keyboard panah kiri/kanan.
- Build: pilih Build, lalu Place tiga kali (keyboard: 2, lalu spasi).
- Paint: pilih Paint, warna, dan tap objek (keyboard: 3).
- Mode Ride via keyboard: 1.
- ⭐: album Wonder Book.
- ⚙️: pengaturan, ganti warna sepeda, reset progres.

## Catatan kualitas
Game ini adalah versi **fitur inti lengkap untuk pengujian keluarga**, bukan rilis komersial Play Store. Perlu pengujian nyata pada berbagai HP, evaluasi aksesibilitas dan UX anak, pengembangan aset original, serta review kebijakan privasi sebelum publikasi komersial.

## Privasi
Tidak ada analytics, login, chat, iklan, atau pengumpulan informasi pribadi dalam kode game. LocalStorage menyimpan progres hanya pada browser perangkat. Dependensi Three.js dimuat dari CDN eksternal. Lihat `PRIVACY.md`.
