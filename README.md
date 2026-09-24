<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=230&section=header&text=AUTO-COMBAT&fontSize=68&fontAlignY=38&desc=Sang%20Pejuang%20Commit%20%E2%80%94%20Berpetualang%20Tanpa%20Henti&descAlignY=60&animation=fadeIn" alt="Auto Combat Banner" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=F7B731&center=true&vCenter=true&width=700&lines=Pedang+terhunus%2C+kotak+hijau+menanti+%E2%9A%94%EF%B8%8F;Setiap+fajar%2C+sang+pejuang+bertarung+sendiri+%F0%9F%8C%85;Tanpa+lelah.+Tanpa+libur.+Tanpa+ampun.+%F0%9F%94%A5" alt="Typing SVG" />

<br/>

[![Auto Combat](https://github.com/muchamad-fabian/auto-combat/actions/workflows/autocommit.yml/badge.svg)](https://github.com/muchamad-fabian/auto-combat/actions)
![Pertempuran per Hari](https://img.shields.io/badge/pertempuran-maks%204x%20sehari-e63946?style=for-the-badge&logo=github&logoColor=white)
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

> ⏳ **Catatan:** Pasukan kadang datang terlambat beberapa menit sampai puluhan menit. Itu bukan pengkhianatan, memang begitulah cara GitHub mengatur barisannya. Tidak semua pasukan hadir setiap hari, lihat bagian **Hari Istirahat** di bawah.

---

## 🛌 Hari Istirahat Sang Pejuang

Pejuang sejati juga butuh tidur. Supaya jejaknya tampak alami dan tidak seperti robot, sang pejuang **libur di hari-hari tertentu**:

| Jenis Libur | Kapan | Keterangan |
| :--- | :--- | :--- |
| 🙏 Hari Suci | Setiap hari **Minggu** | Pasti libur, tanpa pengecualian |
| 🩹 Hari Pemulihan | Sekitar **1 dari 6 hari** | Dipilih acak-tetap berdasarkan tanggal, jadi seluruh pasukan hari itu ikut libur |
| 🌲 Tersesat di Hutan | Sekitar **1 dari 5 serangan** | Satu pasukan tidak datang, sisanya tetap bertempur |
| 📣 Panggilan Manual | Kapan saja | Lewat tombol **Run workflow**, sang pejuang **selalu** bertempur |

Hasilnya, jumlah commit per hari **berbeda-beda**: ada hari ramai, ada hari sepi, dan ada hari kosong. Persis seperti petualang sungguhan. 🏕️

### 📝 Jurus dalam Setiap Commit

Setiap kali bertempur, sang pejuang memilih **satu kisah acak** sebagai pesan commit, misalnya:

> ⚔️ Menebas naga api di Gunung Merapi
> 🛡️ Menahan serangan pasukan kegelapan di gerbang timur
> 👑 Mengalahkan raja iblis di ujung petualangan

Kisah yang sama juga ditulis ke file `LAST_UPDATED` bersama waktunya. Mau menambah jurus baru? Cukup tambahkan satu baris di dalam daftar `PESAN=( ... )` pada file workflow.

### 🎚️ Mengatur Tingkat Kemalasan

Semua angka libur ada di langkah **Periksa kalender perang**:

- Ganti `HASH % 6` menjadi `HASH % 4` kalau ingin lebih sering libur, atau `% 10` kalau ingin lebih jarang
- Ganti `RANDOM % 5` dengan angka lebih besar supaya pasukan jarang tersesat
- Hapus blok `if [ "$HARI" = "7" ]` kalau tidak ingin libur hari Minggu

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
      - name: Periksa kalender perang
        id: kalender
        env:
          EVENT: ${{ github.event_name }}
        run: |
          ISTIRAHAT=false
          ALASAN="Maju bertempur!"

          if [ "$EVENT" = "workflow_dispatch" ]; then
            ALASAN="Dipanggil manual, pejuang wajib bertempur!"
          else
            HARI=$(date -u +%u)
            HASH=$(date -u +%Y%m%d | cksum | cut -d' ' -f1)

            if [ "$HARI" = "7" ]; then
              ISTIRAHAT=true
              ALASAN="Hari Minggu: hari suci, pejuang beristirahat."
            elif [ $((HASH % 6)) -eq 0 ]; then
              ISTIRAHAT=true
              ALASAN="Hari pemulihan: pejuang mengobati luka."
            elif [ $((RANDOM % 5)) -eq 0 ]; then
              ISTIRAHAT=true
              ALASAN="Pasukan ini tersesat di hutan belantara."
            fi
          fi

          echo "istirahat=$ISTIRAHAT" >> "$GITHUB_OUTPUT"
          echo "$ALASAN"

      - name: Bangunkan pasukan (Checkout)
        if: steps.kalender.outputs.istirahat == 'false'
        uses: actions/checkout@v4
        with:
          fetch-depth: 0
          ref: main

      - name: Catat kemenangan (Commit)
        if: steps.kalender.outputs.istirahat == 'false'
        run: |
          PESAN=(
            "⚔️ Menebas naga api di Gunung Merapi"
            "🛡️ Menahan serangan pasukan kegelapan di gerbang timur"
            "🏹 Memanah musuh dari menara tertinggi"
            "🔥 Membakar benteng para bandit hutan"
            "🐉 Menaklukkan naga es di puncak Jayawijaya"
            "🗡️ Mengasah pedang legendaris di tepi sungai"
            "🏰 Merebut kembali istana dari tangan penyihir jahat"
            "🌙 Berburu monster di bawah cahaya bulan purnama"
            "⚡ Menyambar pasukan musuh dengan jurus kilat"
            "🐺 Mengalahkan serigala raksasa penjaga lembah"
            "🌋 Melintasi lautan lava demi sebuah kemenangan"
            "👑 Mengalahkan raja iblis di ujung petualangan"
            "🧙 Memecahkan kutukan kuno di dalam gua rahasia"
            "🚩 Mengibarkan bendera kemenangan di medan perang"
          )
          PILIH="${PESAN[$RANDOM % ${#PESAN[@]}]}"

          {
            date -u '+%Y-%m-%dT%H:%M:%SZ'
            echo "$PILIH"
          } > LAST_UPDATED

          git config user.name "NAMA_GITHUB_ANDA"
          git config user.email "PASTE_EMAIL_NOREPLY_ANDA_DI_SINI"

          git add LAST_UPDATED

          if git diff --cached --quiet; then
            echo "Tidak ada jejak baru. Pasukan beristirahat."
            exit 0
          fi

          git commit -m "$PILIH"

      - name: Kirim laporan ke istana (Push)
        if: steps.kalender.outputs.istirahat == 'false'
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
- Mungkin sedang hari libur sang pejuang (Minggu, hari pemulihan, atau pasukan tersesat). Coba klik **Run workflow** untuk memastikan
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

**⚔️ Kotak hijau bukan akhir dari petualangan, tetapi hanya awal dari legenda. ⚔️**

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer" alt="Footer" />

</div>
