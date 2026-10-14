# 🏛️ Capital Hub - Berkas Rilis & Distribusi Resmi

Selamat datang di repositori distribusi resmi **Capital Hub**, aplikasi manajemen keuangan pribadi dan bisnis yang beroperasi 100% offline, aman, dan privat di komputer Anda.

---

## 📥 Unduh Versi Terbaru

Silakan unduh paket rilis terbaru pada tab **[Releases](https://github.com/230055Fawwaz/capital-hub-releases/releases/latest)**.

| Berkas | Deskripsi |
|---|---|
| `capital-hub-windows-x64.zip` | Versi portabel mandiri untuk Windows 64-bit (Ekstrak & Langsung Pakai) |

---

## 🚀 Panduan Instalasi & Pembaruan

### Pemasangan Baru:
1. Unduh berkas `capital-hub-windows-x64.zip` dari rilis terbaru.
2. Ekstrak ke folder yang Anda inginkan (misal: `D:\CapitalHub` atau `C:\CapitalHub`).
3. Buka folder hasil ekstrak dan jalankan `CapitalHub.exe`.
4. Anda akan otomatis dipandu melalui **Setup Wizard** untuk inisialisasi akun perdana Anda.

### Pembaruan dari Versi Sebelumnya:
1. Cadangkan basis data Anda terlebih dahulu melalui menu **Pengaturan ➔ Sistem & Basis Data ➔ Cadangkan & Unduh**.
2. Tutup aplikasi Capital Hub yang sedang berjalan.
3. Ekstrak berkas rilis baru dan timpa (*overwrite*) seluruh berkas lama, **KECUALI** folder `instance/` (tempat basis data keuangan Anda).
4. Jalankan `CapitalHub.exe` kembali.

---

## 🛠️ Catatan Khusus Pengembang (Build Nuitka ke ZIP Rilis):

Folder hasil kompilasi Nuitka di direktori `dist/`:
* `dist/desktop.build/`: Folder cache/temporary C compiler. **Jangan pernah dibagikan**.
* `dist/desktop.dist/`: **Folder aplikasi utama**. Berisi file `CapitalHub.exe` beserta seluruh dependencies.

### Langkah Menyiapkan `capital-hub-windows-x64.zip`:
1. Buka folder `dist/desktop.dist/instance/`.
2. **PENTING:** Hapus berkas `capital_hub.db` dan `secret_key.token` jika ada di folder `instance/` tersebut (agar data uji coba Anda tidak bocor dan pengguna baru otomatis mendapatkan Setup Wizard bersih).
3. Ubah nama folder `desktop.dist` menjadi `CapitalHub`.
4. Klik kanan folder `CapitalHub` ➔ **Compress to ZIP file** ➔ beri nama `capital-hub-windows-x64.zip`.
5. Berkas `.zip` ini siap Anda seret dan unggah (*drag & drop*) ke GitHub Releases!

---

## 💖 Dukung Pengembang (Donationware)

Capital Hub dikembangkan dengan komitmen 100% gratis tanpa iklan dan tanpa pelacak privasi. Jika aplikasi ini bermanfaat untuk Anda, Anda dapat memberikan apresiasi sukarela melalui:

* **Saweria (QRIS & E-Wallet Lokal):** [saweria.co/capitalhub](https://saweria.co/capitalhub)
* **Ko-fi (Kartu / Internasional):** [ko-fi.com/capitalhub](https://ko-fi.com/capitalhub)

---

## 📄 Lisensi
Perangkat lunak ini didistribusikan di bawah lisensi **Capital Hub Donationware License**. Lihat berkas [LICENSE](LICENSE) untuk rincian lengkap.
