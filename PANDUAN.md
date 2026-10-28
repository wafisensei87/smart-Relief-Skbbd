# SmartRelief — Panduan Ringkas

Sistem pengurusan jadual guru ganti (relief). Satu fail sahaja: `index.html`.

## Cara guna
1. Buka `index.html` dengan Chrome / Edge (klik dua kali).
2. Log masuk kali pertama: ID `admin`, kata laluan `admin123`.
   **Tukar segera** di tab ⚙️ Tetapan.
3. Tab **📅 Jadual Induk** → **Pilih Fail .roz**: pilih fail jadual aSc Timetables (cth. `JADUAL 2026 V5.roz`).
   Semua guru, kelas, subjek, hari (Ahad–Khamis) dan waktu dibaca terus daripada fail.
   Guru contoh akan digantikan; no. telefon guru yang namanya sama dikekalkan.
   Kelas 2 atau 3 masa (cth. 10:45–11:45) diisi pada setiap masa yang terlibat.
4. Tab **⚙️ Tetapan** → **Waktu Rasmi**: masa loceng (W1 7:45 – W11 1:15) dibaca daripada fail; semak dan
   tandakan waktu rehat jika perlu. Isi juga no. WhatsApp pentadbir.
5. Tab **💬 WhatsApp Guru** → **Upload Maklumat Guru Secara Pukal**:
   - Tekan **Muat Turun Templat** untuk dapat senarai semua guru (CSV, boleh dibuka dengan Excel).
   - Isi lajur **Telefon** (dan Subjek jika perlu), simpan, kemudian **Pilih Fail Excel / CSV**.
   - Atau salin 2–3 lajur dari Excel (Nama, Telefon, Subjek) dan tampal dalam kotak, tekan **Proses**.
   - Nama dipadankan tanpa mengira huruf besar/kecil. Nama yang tiada dalam sistem ditambah sebagai guru baharu
     (nyahtanda kotak jika tidak mahu).
6. Setiap pagi di **Dashboard**:
   - Tekan butang HADIR → CUTI pada guru tidak hadir, pilih sebab cuti.
   - Tekan **🪄 Jana Automatik**. Guru ganti boleh ditukar secara manual melalui senarai pilihan.
   - Tekan **WhatsApp** (atau "Hantar Semua Serentak") untuk hantar mesej berserta pautan pengesahan.
   - Tekan **⬇ Download Imej Jadual (.PNG)** dan post ke grup WhatsApp, atau 🖨️ untuk cetak.

## Kriteria pilihan guru ganti (automatik)
1. Guru kosong pada waktu itu (tiada kelas & belum jadi guru ganti).
2. Diutamakan guru yang tiada kelas sebelum & selepas slot itu.
3. Diutamakan beban sehari lebih rendah: ≤3 waktu (Pilihan 1), 4 waktu (Pilihan 2), ≥5 waktu (Pilihan 3).

## Pentadbir tidak dijadikan guru ganti
Guru bertanda **Pentadbir** (tab WhatsApp Guru) tidak akan dipilih sebagai guru ganti.
Nama dengan (GB), (PKP), (PK HEM), (PK KO) ditanda secara automatik; tanda/nyahtanda sendiri jika perlu.
Dalam upload pukal, lajur **Pentadbir** boleh diisi Ya / Tidak.

## Kelas pairing (Tasmik, Tilawah, PI(Q) dan lain-lain)
- Pelajaran dengan lebih daripada seorang guru dalam aSc dikenal pasti sebagai kelas pairing.
  Untuk jadual yang diisi sendiri, pilih rakan di lajur **Guru Pairing** dalam Jadual Induk.
- Jika seorang guru pairing cuti dan rakannya hadir, slot itu ditanggung rakan pairing (status hijau "Pairing").
  Tiada guru lain dipilih.
- Jika semua guru pairing kelas itu cuti, hanya **seorang** guru ganti dipilih untuk kelas itu.
- Guru yang sedang mengajar pada waktu itu (termasuk kelas pairingnya sendiri) tidak akan dipilih
  sebagai guru ganti untuk kelas lain.

## Pengesahan guru
Guru buka pautan dalam WhatsApp → tekan **Sahkan** → WhatsApp terbuka untuk membalas "SAH" kepada
pentadbir. Pentadbir kemudian tekan butang **Belum Sah** supaya bertukar **Sah** (hijau).
(Status tidak boleh bertukar sendiri dari telefon guru kerana sistem ini tiada pelayan/server.)

## Penting
- Data disimpan dalam pelayar komputer itu sahaja. Gunakan **Eksport Data** di Tetapan untuk sandaran
  atau untuk pindah ke komputer lain (**Import Data**).
- Pautan pengesahan hanya boleh dibuka oleh guru jika `index.html` dihoskan di internet
  (cth. GitHub Pages / Netlify). Jika dibuka terus dari komputer, pautan itu tidak berfungsi di telefon guru.
- Muat turun PNG dan fon memerlukan sambungan internet.
