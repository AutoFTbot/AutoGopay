# Contributing to AutoGoPay

Terima kasih atas minat Anda untuk berkontribusi ke AutoGoPay! 🎉

## Menambahkan Logo Toko Anda

Jika Anda menggunakan AutoGoPay untuk bisnis Anda dan ingin menampilkan logo toko di landing page kami, ikuti langkah-langkah berikut:

### Persyaratan Logo

1. **Format**: PNG atau SVG dengan background transparan
2. **Ukuran**: 100x100 pixels (akan di-resize otomatis jika lebih besar)
3. **Kualitas**: Logo harus jelas dan berkualitas tinggi
4. **Konten**: Logo harus merepresentasikan bisnis yang sah dan aktif menggunakan AutoGoPay

### Cara Menambahkan Logo

1. **Fork repository ini**
   ```bash
   git clone https://github.com/AutoFTbot/AutoGopay.git
   cd AutoGopay
   ```

2. **Tambahkan logo Anda**
   - Buat folder baru di `autogopay/public/stores/` dengan nama toko Anda (lowercase, gunakan dash untuk spasi)
   - Upload logo dengan nama `logo.png` atau `logo.svg`
   - Contoh: `autogopay/public/stores/toko-saya/logo.png`

3. **Update file stores.json**
   - Edit file `autogopay/public/stores/stores.json`
   - Tambahkan informasi toko Anda:
   ```json
   {
     "name": "Nama Toko Anda",
     "logo": "/stores/toko-saya/logo.png",
     "website": "https://tokosaya.com",
     "description": "Deskripsi singkat toko Anda"
   }
   ```

4. **Buat Pull Request**
   - Commit perubahan Anda
   ```bash
   git add .
   git commit -m "Add [Nama Toko] logo"
   git push origin main
   ```
   - Buat Pull Request ke repository utama
   - Jelaskan bisnis Anda dan bagaimana Anda menggunakan AutoGoPay

### Review Process

- Setiap Pull Request akan di-review oleh maintainer
- Logo akan di-approve jika memenuhi persyaratan dan bisnis terbukti aktif menggunakan AutoGoPay
- Proses review biasanya memakan waktu 1-3 hari kerja
- Kami berhak menolak logo yang tidak sesuai dengan guidelines

### Contoh Struktur Folder

```
autogopay/public/stores/
├── stores.json
├── example-store/
│   └── logo.png
├── toko-elektronik/
│   └── logo.png
├── warung-kopi/
│   └── logo.svg
└── toko-buku/
    └── logo.png
```

### Contoh stores.json

```json
[
  {
    "name": "Example Store",
    "logo": "/stores/example-store/logo.png",
    "website": "https://example.com",
    "description": "Contoh toko yang menggunakan AutoGoPay untuk payment gateway"
  },
  {
    "name": "Toko Elektronik",
    "logo": "/stores/toko-elektronik/logo.png",
    "website": "https://tokoelektronik.com",
    "description": "Toko elektronik terpercaya sejak 2020"
  },
  {
    "name": "Warung Kopi",
    "logo": "/stores/warung-kopi/logo.svg",
    "website": "https://warungkopi.id",
    "description": "Kopi berkualitas dengan harga terjangkau"
  }
]
```

## Aturan Umum

- Logo tidak boleh mengandung konten yang menyinggung, ilegal, atau tidak pantas
- Logo harus milik Anda atau Anda memiliki izin untuk menggunakannya
- Kami berhak menghapus logo kapan saja jika ditemukan pelanggaran
- Dengan mengirimkan logo, Anda setuju bahwa logo akan ditampilkan di website AutoGoPay

## Pertanyaan?

Jika Anda memiliki pertanyaan, silakan hubungi kami melalui:
- Telegram: [@AutoGopayBot](https://t.me/AutoGopayBot)
- GitHub Issues: [Create an issue](https://github.com/AutoFTbot/AutoGopay/issues)

---

Terima kasih telah menggunakan AutoGoPay! 🚀
