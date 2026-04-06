# Contributing to AutoGoPay

Terima kasih atas minat Anda untuk berkontribusi ke AutoGoPay! 🎉

## Menambahkan Logo Toko Anda

Jika Anda menggunakan AutoGoPay untuk bisnis Anda dan ingin menampilkan logo toko di landing page kami, ikuti langkah-langkah berikut:

### Persyaratan Logo

1. **Format**: PNG atau SVG dengan background transparan
2. **Ukuran**: 100x100 pixels (akan di-resize otomatis jika lebih besar)
3. **Kualitas**: Logo harus jelas dan berkualitas tinggi
4. **Konten**: Logo harus merepresentasikan bisnis yang sah dan aktif menggunakan AutoGoPay

---

## 💻 Cara Manual (Untuk yang Familiar dengan GitHub)

### 1️⃣ Fork Repository

- Buka https://github.com/AutoFTbot/AutoGopay
- Klik tombol **"Fork"** di kanan atas
- Repository akan ter-copy ke akun GitHub Anda

### 2️⃣ Upload Logo

**Via GitHub Web (Tanpa Install Apapun):**

1. Buka repository Anda yang sudah di-fork
2. Masuk ke folder `logos/`
3. Klik **"Add file"** → **"Upload files"**
4. Upload logo Anda dengan nama: `nama-toko.png` atau `nama-toko.svg`
   - Contoh: `toko-elektronik.png`
   - Gunakan huruf kecil semua
   - Gunakan dash (-) untuk spasi

### 3️⃣ Edit stores.json

1. Masih di folder `logos/`, klik file **`stores.json`**
2. Klik icon **pensil** (Edit) di kanan atas
3. Tambahkan informasi toko Anda di akhir list (sebelum `]`):

```json
  ,
  {
    "name": "Nama Toko Anda",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/nama-toko.png",
    "website": "https://tokosaya.com",
    "description": "Deskripsi singkat toko Anda"
  }
```

**⚠️ Penting:**
- Jangan lupa koma (`,`) di awal
- Ganti `nama-toko.png` dengan nama file logo Anda
- Ganti URL website dan deskripsi sesuai toko Anda

**Contoh Lengkap:**
```json
[
  {
    "name": "Example Store",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/example-store.svg",
    "website": "https://github.com/AutoFTbot/AutoGopay",
    "description": "Contoh toko yang menggunakan AutoGoPay"
  },
  {
    "name": "Toko Elektronik Jaya",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/toko-elektronik.png",
    "website": "https://tokoelektronik.com",
    "description": "Toko elektronik terpercaya sejak 2020"
  }
]
```

4. Klik **"Commit changes"** di kanan atas
5. Tulis pesan commit: `Add [Nama Toko] logo`
6. Klik **"Commit changes"** lagi

### 4️⃣ Buat Pull Request

1. Kembali ke halaman utama repository Anda
2. Klik tombol **"Contribute"** → **"Open pull request"**
3. Tulis deskripsi:
   ```
   Menambahkan logo [Nama Toko]
   
   - Nama: [Nama Toko]
   - Website: [URL]
   - Menggunakan AutoGoPay untuk: [jelaskan singkat]
   ```
4. Klik **"Create pull request"**

### 5️⃣ Tunggu Review

- Kami akan review dalam 1-3 hari kerja
- Jika disetujui, logo akan otomatis muncul di website!

---

## 🖥️ Cara Advanced (Via Command Line)

Untuk developer yang familiar dengan Git:

```bash
# 1. Fork repository di GitHub, lalu clone
git clone https://github.com/USERNAME-ANDA/AutoGopay.git
cd AutoGopay

# 2. Tambahkan logo
cp /path/to/logo.png logos/toko-saya.png

# 3. Edit logos/stores.json (tambahkan entry baru)

# 4. Commit dan push
git add logos/toko-saya.png logos/stores.json
git commit -m "Add [Nama Toko] logo"
git push origin main

# 5. Buat Pull Request di GitHub
```

---

## ❓ FAQ

### Berapa lama proses review?
Biasanya 1-3 hari kerja. Kami akan review dan approve jika memenuhi persyaratan.

### Apakah gratis?
Ya, 100% gratis! Ini adalah cara kami mengapresiasi merchant yang menggunakan AutoGoPay.

### Logo saya ditolak, kenapa?
Kemungkinan:
- Kualitas logo kurang baik
- Ukuran tidak sesuai (harus 100x100px)
- Bisnis tidak aktif menggunakan AutoGoPay
- Konten tidak sesuai guidelines

### Bisa update logo nanti?
Bisa! Kirim Pull Request baru dengan logo yang sudah diupdate.

### Saya tidak punya GitHub, bagaimana?
Gunakan cara mudah: kirim logo via Telegram ke [@AutoGopayBot](https://t.me/AutoGopayBot)

---

## 📞 Butuh Bantuan?

Jika Anda kesulitan atau ada pertanyaan:
- 💬 Telegram: [@AutoFtBot69](https://t.me/AutoFtBot69)
- 🐛 GitHub Issues: [Create an issue](https://github.com/AutoFTbot/AutoGopay/issues)

---

## ⚖️ Aturan Umum

- Logo tidak boleh mengandung konten yang menyinggung, ilegal, atau tidak pantas
- Logo harus milik Anda atau Anda memiliki izin untuk menggunakannya
- Kami berhak menghapus logo kapan saja jika ditemukan pelanggaran
- Dengan mengirimkan logo, Anda setuju bahwa logo akan ditampilkan di website AutoGoPay

---

Terima kasih telah menggunakan AutoGoPay! 🚀
