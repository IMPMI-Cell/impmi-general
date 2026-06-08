# IM PMI — Template Kerja Tim

Repository ini digunakan oleh tim **Information Management (IM) PMI** untuk mengelola tasking, progres kerja, output, dan dokumentasi keputusan selama latihan maupun operasi.

Repo ini bekerja bersama **Microsoft Teams** (komunikasi dan koordinasi), **SharePoint** (penyimpanan dokumen kerja), dan **GitHub Project Kanban** (tasking dan pelacakan progres).

---

## 📈 Progress Project Kanban

<!-- PROJECT_PROGRESS:START -->
![Progress](https://geps.dev/progress/0)

**Progress Kanban:** 0/0 item selesai (0%).
<!-- PROJECT_PROGRESS:END -->

> Progress dihitung otomatis dari [GitHub Project Kanban](https://github.com/orgs/IMPMI-Cell/projects/12) berdasarkan jumlah item berstatus `Done` dibandingkan total item yang memiliki field `Status`.

---

## 📞 Saluran Komunikasi Tim

| Kanal | Fungsi | Tautan |
|---|---|---|
| MS Teams | Diskusi formal dan koordinasi | [Buka Teams](https://teams.microsoft.com/l/channel/19%3A9c086bccf28d499f94ad6a4daeb26bf7%40thread.skype/TEAM%20IM?groupId=bbf3c731-4917-4fee-aab6-2c078eca3108&tenantId=1e4e05eb-0506-49fc-b693-1adf0e95d162) |
| SharePoint | Penyimpanan dokumen kerja | [Buka SharePoint](https://pmipusat.sharepoint.com/:f:/r/sites/IM-PMI/Shared%20Documents/TEAM%20IM?csf=1&web=1&e=K6qfoS) |
| GitHub Kanban | Tasking dan tracking progres | [Buka Project](https://github.com/orgs/IMPMI-Cell/projects/12) |
| WhatsApp | Koordinasi cepat | [Buka WA](#) |

---

## 📁 Struktur Folder Kerja

```text
├── 00_Admin/
├── D_Data/
│   ├── 1_Sekunder/
│   ├── 2_Prime/
│   ├── 3_Analisis/
│   ├── 4_Kobo/
│   └── Image/
├── P_Produk/
│   ├── P1_Laporan/
│   ├── P2_Peta/
│   └── P3_Dashboard/
└── Z_Arsip/
```

---

## 🧩 Format Tasking 8-Field

Setiap issue dibuat menggunakan format 8-field berikut:

| Field | Isi |
|---|---|
| **Apa** | Tugas yang harus dikerjakan |
| **Tujuan** | Alasan tugas diperlukan |
| **Hasil** | Output akhir yang diharapkan |
| **Format** | Bentuk output (Excel, PDF, Markdown, Peta, Dashboard, Slide) |
| **Prioritas** | Tinggi / Sedang / Rendah |
| **Deadline** | Tanggal dan jam batas pengerjaan |
| **Sumber Data** | Dataset, dokumen, atau tautan referensi |
| **Requester** | Pihak yang meminta tugas |

---

## 🤝 Cara Berkontribusi

1. Buka [kanban](https://github.com/orgs/IMPMI-Cell/projects/12) dan pilih issue berlabel sesuai kapasitas (mis. `gis`, `data`, `mdc`, `infographic`, `qa-qc`).
2. Jika ada kebutuhan baru, buat issue baru menggunakan format 8-field di atas.
3. Untuk diskusi, gunakan **thread di Teams** agar satu topik = satu thread.
4. Tandai issue sebagai `Done` di Project Kanban setelah selesai agar progress otomatis terupdate.

---

## 🗃️ Aturan Dasar Data

- Setiap data atau produk wajib mencantumkan minimal: **sumber**, **timestamp (as-of)**, dan **tingkat kepercayaan (confidence)**.
- Tidak membagikan PII atau data sensitif (nama, nomor HP individu) pada output publik.
- Data kontak untuk verifikasi disimpan terbatas sesuai persetujuan (consent).
- Jika ada perbedaan angka antar sumber, jangan pilih salah satu tanpa catatan — tampilkan semua versi dengan keterangan sumbernya dan tandai sebagai *unverified* sampai direkonsiliasi.
- Setiap perubahan signifikan pada dataset (koreksi, penambahan, penghapusan) wajib dicatat di changelog atau komentar issue terkait, lengkap dengan alasan perubahan.

---

## 🤲 Kode Etik Kolaborasi

- Fokus pada kebutuhan operasional dan hindari duplikasi kerja.
- Gunakan bahasa yang jelas dan singkat.
- Cantumkan asumsi dan metodologi saat membuat peta atau analisis.
- Saling menghargai kapasitas dan waktu anggota tim.
- Jika mengambil alih atau melanjutkan pekerjaan orang lain, konfirmasi dulu kepada pemilik issue sebelum melakukan perubahan besar.
- Eskalasi hambatan lebih awal — jika ada kendala yang berpotensi menggeser deadline, informasikan ke koordinator **sebelum** deadline terlewat, bukan sesudahnya.

---

## ⚙️ Integrasi Progress Otomatis

Progress bar di atas diperbarui otomatis oleh GitHub Actions setiap kali ada perubahan di Project Kanban. Workflow membaca status item dan menghitung:

```
Progress (%) = jumlah item "Done" ÷ total item dengan field Status × 100
```

Status yang dihitung sebagai selesai: `Done`, `Selesai`, `Completed`, `Complete`.

Lihat [`CARA_PAKAI_PROGRESS.md`](./CARA_PAKAI_PROGRESS.md) untuk panduan setup lengkap termasuk cara membuat PAT dan menyimpannya sebagai secret.

---

## 📎 Dokumen Pendukung

| File | Keterangan |
|---|---|
| [`CARA_PAKAI_PROGRESS.md`](./CARA_PAKAI_PROGRESS.md) | Panduan setup workflow progress otomatis + PAT |
| [`STRUKTUR_FOLDER.md`](./STRUKTUR_FOLDER.md) | Panduan penggunaan folder kerja |
| [`LABEL_ISSUE.md`](./LABEL_ISSUE.md) | Rekomendasi label GitHub Issue |
| [`tasking-8-field.md`](./tasking-8-field.md) | Template issue GitHub format 8-field |
