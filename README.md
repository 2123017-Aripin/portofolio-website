# Aripin — Portfolio Website

Website portofolio pribadi untuk menampilkan latar belakang, keahlian, dan proyek di bidang **mobile development** dan **jaringan komputer**.

🔗https://2123017-aripin.github.io/portofolio-website/

## Preview

Single-page portfolio dengan tema dark navy, aksen amber, dan elemen visual bertema jaringan (notasi subnet pada label section, animasi trace-route pada hero).

## Tech Stack

Dibangun sebagai satu file statis, tanpa build step atau dependency eksternal selain Google Fonts:

- **HTML5 + CSS3** (murni, tanpa framework)
- **Vanilla JavaScript** (animasi ringan via CSS)
- **Google Fonts** — Space Grotesk, Inter, JetBrains Mono
- Gambar profil di-embed langsung sebagai base64 (tidak perlu file gambar terpisah)

## Struktur Konten

| Section | Isi |
|---|---|
| Hero | Nama, tagline, foto profil, stack overview |
| About | Latar belakang pendidikan (Teknik Informatika, UIM Yogyakarta) |
| Skills | Mobile Development, Backend & Cloud, Jaringan & Infrastruktur |
| Projects | Proyek **Panda Ramen** (Flutter + Firebase + Node.js + Midtrans) dan studi kasus jaringan (VLSM, OSPF, ACL, VLAN, QoS) |
| Contact | Link GitHub dan email |

## Menjalankan Secara Lokal

Karena ini murni HTML/CSS/JS statis, tidak perlu instalasi apa pun:

```bash
git clone https://github.com/2123017-Aripin/portfolio-website.git
cd portfolio-website
```

Lalu buka `index.html` langsung di browser, atau jalankan local server sederhana:

```bash
python3 -m http.server 8000
```

Akses di `http://localhost:8000`.

## Deploy ke GitHub Pages

1. Push repository ini ke GitHub (lihat langkah upload di bawah).
2. Buka repo di GitHub → **Settings** → **Pages**.
3. Pada **Source**, pilih branch `main` dan folder `/root`.
4. Klik **Save**. Tunggu 1–2 menit, link live akan muncul di bagian atas halaman Pages.

## Kustomisasi

- **Email kontak:** cari `email-anda@contoh.com` di `index.html` dan ganti dengan email asli.
- **Tambah proyek baru:** duplikasi salah satu `.case-card` di section `#projects`.
- **Ganti foto:** ganti string base64 pada tag `<img src="data:image/jpeg;base64,...">`, atau ubah jadi `<img src="foto.jpg">` dan taruh file gambar terpisah di folder yang sama.

## Kontak

- GitHub: [@2123017-Aripin](https://github.com/2123017-Aripin)

---

_Dibangun dengan perhatian pada detail — Aripin, 2026._
