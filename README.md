<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=230&section=header&text=AUTO-COMBAT&fontSize=68&fontAlignY=38&desc=Sang%20Pejuang%20Commit%20%E2%80%94%20Berpetualang%20Tanpa%20Henti&descAlignY=60&animation=fadeIn" alt="Auto Combat Banner" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=F7B731&center=true&vCenter=true&width=700&lines=Pedang+terhunus%2C+kotak+hijau+menanti+%E2%9A%94%EF%B8%8F;Setiap+fajar%2C+sang+pejuang+bertarung+sendiri+%F0%9F%8C%85;Tanpa+lelah.+Tanpa+libur.+Tanpa+ampun.+%F0%9F%94%A5" alt="Typing SVG" />

<br/>

[![Auto Combat](https://github.com/muchamad-fabian/auto-combat/actions/workflows/autocommit.yml/badge.svg)](https://github.com/muchamad-fabian/auto-combat/actions)
![Pertempuran per Hari](https://img.shields.io/badge/pertempuran-4x%20sehari-e63946?style=for-the-badge&logo=github&logoColor=white)
![Ditenagai](https://img.shields.io/badge/ditenagai-GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Biaya](https://img.shields.io/badge/biaya-GRATIS-2ea44f?style=for-the-badge)

</div>

---

## 📜 Kisah Sang Pejuang

Di sebuah negeri bernama **GitHub**, hiduplah seorang pejuang yang tak pernah tidur.
Setiap fajar menyingsing, ia bangkit, mengayunkan pedangnya, dan meninggalkan **satu jejak pertempuran** di medan perang bernama `LAST_UPDATED`.

Ia bukan manusia. Ia adalah **GitHub Actions**, dan tugasnya satu: membuat halaman profilmu **hijau berkilau** ⚔️

> *"Jejak yang ditinggalkan hari ini adalah legenda yang dikenang esok hari."*

---

## 🗺️ Peta Petualangan

| Jam Serangan (WIB) | Jam Serangan (UTC) | Nama Pasukan |
| :---: | :---: | :--- |
| 🌅 08.00 | 01.00 | Pasukan Fajar |
| ☀️ 10.00 | 03.00 | Pasukan Pagi |
| 🌤️ 12.00 | 05.00 | Pasukan Siang |
| 🌇 14.00 | 07.00 | Pasukan Senja |

> ⏳ **Catatan:** Pasukan kadang datang terlambat beberapa menit sampai puluhan menit. Itu bukan pengkhianatan, memang begitulah cara GitHub mengatur barisannya.

---

## 🛡️ Perlengkapan yang Harus Dibawa

Sebelum berangkat, pastikan tas petualanganmu berisi:

- 🧙 **Akun GitHub** yang aktif
- 📧 **Email noreply GitHub** milikmu (rahasia, akan dijelaskan di bawah)
- 🐒 **Keberanian** untuk mengklik tombol

---

## ⚔️ Misi 1 — Tempa Markasmu (Buat Repo Baru)

> ⚠️ **Jangan fork!** Repo hasil *fork* tidak dihitung sebagai kontribusi. Bangun markas baru dari nol.

1. Klik tanda **➕** di pojok kanan atas GitHub, lalu **New repository**
2. Beri nama repo: `auto-combat`
3. Pilih **Public**
4. Centang **Add a README file**
5. Klik **Create repository**

✅ *Markas berdiri. Lanjut ke misi berikutnya.*

---

## 🗡️ Misi 2 — Asah Pedang (Buat File `LAST_UPDATED`)

Ini adalah medan perang tempat sang pejuang meninggalkan jejaknya.

1. Klik **Add file**, lalu **Create new file**
2. Di kolom nama, ketik: `LAST_UPDATED`
3. Di isi file, ketik angka `1`
4. Klik **Commit changes**, lalu **Commit changes** sekali lagi

---

## 🔮 Misi 3 — Temukan Mantra Rahasia (Email Noreply)

Tanpa mantra ini, jejak pertempuranmu **tidak diakui** oleh profil.

1. Buka 👉 https://github.com/settings/emails
2. Cari alamat berakhiran `@users.noreply.github.com`
3. **Salin** alamat itu, akan dipakai di Misi 4

> 💡 Bentuknya biasanya seperti `12345678+namamu@users.noreply.github.com`

---

## 📖 Misi 4 — Tulis Kitab Sihir (File Workflow)

1. Klik **Add file**, lalu **Create new file**
2. Di kolom nama, ketik persis: `.github/workflows/autocommit.yml`
   *(setiap mengetik `/`, folder terbentuk otomatis)*
3. Tempel kitab sihir di bawah ini
4. **Ganti** `PASTE_EMAIL_NOREPLY_ANDA_DI_SINI` dengan mantra dari Misi 3
5. Klik **Commit changes**, lalu **Commit changes** sekali lagi

```yaml
name: Auto Combat

on:
  schedule:
    - cron: "0 1 * * *"   # Pasukan Fajar  (08.00 WIB)
    - cron: "0 3 * * *"   # Pasukan Pagi   (10.00 WIB)
    - cron: "0 5 * * *"   # Pasukan Siang  (12.00 WIB)
    - cron: "0 7 * * *"   # Pasukan Senja  (14.00 WIB)

  workflow_dispatch:       # Tombol panggil pasukan manual

permissions:
  contents: write

jobs:
  auto_combat:
    runs-on: ubuntu-latest

    steps:
      - name: Bangunkan pasukan (Checkout)
        uses: actions/checkout@v4
        with:
          fetch-depth: 0
          ref: main

      - name: Tinggalkan jejak pertempuran
        run: |
          date -u '+%Y-%m-%dT%H:%M:%SZ' > LAST_UPDATED

      - name: Catat kemenangan (Commit)
        run: |
          git config user.name "NAMA_GITHUB_ANDA"
          git config user.email "PASTE_EMAIL_NOREPLY_ANDA_DI_SINI"

          git add LAST_UPDATED

          if git diff --cached --quiet; then
            echo "Tidak ada jejak baru. Pasukan beristirahat."
            exit 0
          fi

          git commit -m "chore(combat): sang pejuang telah bertempur"

      - name: Kirim laporan ke istana (Push)
        run: |
          git pull --rebase origin main
          git push origin main
```

> 🔔 Perhatikan: nama cabang di sini adalah **`main`**, bukan `master`. Kalau salah tulis, pasukan akan tersesat dan gagal.

---

## 🔥 Misi 5 — Bangkitkan Sang Pejuang

Jangan menunggu besok, uji sekarang juga!

1. Klik tab **Actions**
2. Klik **Auto Combat** di daftar sebelah kiri
3. Klik tombol **Run workflow**, lalu **Run workflow** hijau
4. Tunggu sekitar 15 detik, lalu refresh halaman
5. Muncul **✅ centang hijau**? Sang pejuang telah bangkit! 🎉

---

## 🪦 Misi 6 — Pensiunkan Pejuang Lama

Kalau kamu punya repo lama (misalnya hasil fork `auto-commit`), **matikan** supaya dua pejuang tidak saling bertabrakan.

**Cara halus: matikan workflow-nya saja**

1. Buka repo lama, lalu tab **Actions**
2. Klik **Auto Commit** di daftar sebelah kiri
3. Klik titik tiga **⋯** di pojok kanan atas
4. Klik **Disable workflow**
5. Muncul tulisan *"This workflow was disabled manually"*? Selesai ✅

**Cara tegas: hapus repo lamanya**

1. Buka repo lama, lalu tab **Settings**
2. Gulir sampai paling bawah ke bagian **Danger Zone**
3. Klik **Delete this repository**
4. Ketik nama repo persis seperti yang diminta, lalu konfirmasi

> ☠️ Menghapus repo bersifat **permanen**. Kalau ragu, pilih cara halus dulu.

---

## 👁️ Misi 7 — Saksikan Hasil Pertempuran

Buka profil GitHub-mu besok. Kotak hijau seharusnya bertambah.
Kadang butuh **beberapa jam** sebelum kemenangan tampil di layar. Bersabarlah, wahai pengembara.

---

## 🐉 Bestiari — Monster yang Mungkin Menghadang

<details>
<summary><b>👹 Workflow gagal (❌ merah)</b></summary>

<br/>

- Cek apakah nama cabang di file workflow sudah `main`
- Cek **Settings → Actions → General → Workflow permissions**, pilih **Read and write permissions**
- Klik run yang gagal untuk membaca pesan errornya

</details>

<details>
<summary><b>👻 Centang hijau ada, tapi kotak hijau di profil tidak bertambah</b></summary>

<br/>

- Email di file workflow harus **sama persis** dengan email noreply akunmu
- Pastikan repo **bukan fork**
- Pastikan commit masuk ke cabang default (`main`)
- Tunggu beberapa jam, lalu cek lagi

</details>

<details>
<summary><b>🧟 Pasukan tidak datang sesuai jadwal</b></summary>

<br/>

- Jadwal GitHub sering terlambat, itu normal
- Repo yang lama tidak ada aktivitas bisa dinonaktifkan otomatis oleh GitHub. Buka tab **Actions** dan aktifkan kembali kalau ada tombolnya

</details>

<details>
<summary><b>🐲 Muncul error saat push</b></summary>

<br/>

- Biasanya karena izin tulis belum aktif. Ulangi langkah **Read and write permissions** di atas

</details>

---

## ❓ Tanya Jawab Para Pengembara

**Apakah ini curang?**
Ini hanya alat otomatisasi untuk latihan dan bersenang-senang. Grafik kontribusi bukan penilaian kemampuan sejati, jadi tetaplah menulis kode sungguhan, wahai pejuang. 😉

**Apakah gratis?**
Ya, repo publik mendapat jatah GitHub Actions gratis.

**Bisakah mengganti jadwalnya?**
Bisa. Ubah baris `cron` di file workflow. Gunakan [crontab.guru](https://crontab.guru/) untuk membantu, ingat waktunya dalam **UTC**.

---

## 🏆 Penghargaan

- ⚙️ [GitHub Actions](https://github.com/features/actions) — pasukan yang tak pernah lelah
- 🌱 Proyek asli [mazipan/auto-commit](https://github.com/mazipan/auto-commit) — sumber inspirasi para pejuang

<div align="center">

<br/>

**⚔️ Kotak hijau bukan akhir dari petualangan, hanya awal dari legenda. ⚔️**

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer" alt="Footer" />

</div>
