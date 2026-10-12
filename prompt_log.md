# Log Prompt AI — Purwarupa Voucher Entri Transaksi Kas Keluar

**Nama:** Muhammad Ilman Assiediqie  
**NIM:** 12030123140343  
**Mata Kuliah:** Pengkodean dan Pemrograman  
**Kelas:** E  
**Proyek:** Purwarupa aplikasi web Voucher Entri Transaksi Kas Keluar

## 1. Informasi Penggunaan AI

- **AI Tool:** Gemini Canvas
- **Tujuan:** Membantu merancang dan mengembangkan purwarupa aplikasi Voucher Entri Transaksi Kas Keluar menggunakan HTML, Tailwind CSS, dan JavaScript, serta menyusun rancangan integrasi basis data untuk mendukung pencatatan transaksi akuntansi.

## 2. Prompt Utama

Prompt berikut digunakan sebagai acuan pengembangan purwarupa aplikasi:

> Buat purwarupa aplikasi web Voucher Entri Transaksi Kas Keluar menggunakan HTML, Tailwind CSS, dan JavaScript.
>
> Buat formulir yang terdiri atas tanggal transaksi, nomor voucher, deskripsi, dan tabel jurnal dinamis dengan kolom akun, debit, dan kredit. Sediakan fitur untuk menambah dan menghapus baris jurnal.
>
> Hitung total debit, total kredit, dan selisih secara otomatis setiap kali pengguna mengubah nominal. Tampilkan indikator Balanced jika total debit sama dengan total kredit dan selisihnya nol. Jika belum seimbang, tampilkan indikator Unbalanced.
>
> Tombol Submit hanya dapat digunakan jika jurnal memenuhi ketentuan validasi, yaitu memiliki minimal dua baris jurnal yang valid, setiap baris hanya memiliki salah satu nilai debit atau kredit yang positif, seluruh akun valid, serta total debit sama dengan total kredit.
>
> Rancang antarmuka yang responsif dan mudah digunakan. Tambahkan pesan validasi yang jelas untuk membantu pengguna mengetahui kesalahan input sebelum mengirimkan transaksi.
>
> Selain antarmuka, sertakan rancangan integrasi Supabase dengan PostgreSQL yang mencakup tabel chart_of_accounts, journal_headers, journal_lines, dan audit_logs. Dokumentasikan rancangan pencatatan identitas pengguna, waktu transaksi, aktivitas pengguna, dan hash_checksum untuk mendukung pemeriksaan integritas data.
>
> Rancang pula mekanisme agar jurnal berstatus POSTED tidak dapat diubah atau dihapus secara langsung. Koreksi transaksi dilakukan melalui reversing entry.
>
> Sertakan struktur file, skema SQL, penjelasan alur validasi, konfigurasi Supabase, serta skenario pengujian jurnal seimbang, jurnal tidak seimbang, nominal negatif, dan upaya mengubah jurnal yang telah diposting.
>
> Bedakan fitur yang telah diimplementasikan dari fitur yang masih berupa rancangan. Jangan menyatakan integrasi basis data, kontrol keamanan, atau skenario pengujian telah berhasil jika belum benar-benar dilakukan.

## 3. Tujuan dan Ruang Lingkup Prompt

Prompt tersebut digunakan untuk mengarahkan pengembangan purwarupa dengan memperhatikan beberapa aspek berikut:

1. **Antarmuka pengguna:** Menyediakan formulir transaksi kas keluar dan tabel jurnal yang dinamis.
2. **Validasi jurnal:** Menghitung total debit dan kredit serta memeriksa keseimbangan pencatatan.
3. **Validasi input:** Membantu mencegah input yang tidak sesuai dengan ketentuan jurnal.
4. **Rancangan basis data:** Menyiapkan struktur tabel untuk akun, header jurnal, baris jurnal, dan log audit.
5. **Audit trail:** Merancang pencatatan aktivitas pengguna dan informasi yang diperlukan untuk menelusuri perubahan transaksi.
6. **Integritas transaksi:** Merancang pembatasan perubahan terhadap jurnal yang telah diposting serta mekanisme koreksi melalui reversing entry.
7. **Pengujian:** Menentukan skenario pengujian yang dapat digunakan untuk memeriksa kesesuaian fungsi aplikasi.

## 4. Catatan Transparansi

Dokumen ini mencatat prompt utama yang menjadi acuan pengembangan purwarupa. Isi prompt merupakan spesifikasi yang diminta kepada AI dan tidak secara otomatis membuktikan bahwa seluruh spesifikasi telah diimplementasikan.

Status implementasi dan pengujian setiap fitur perlu diperiksa berdasarkan kode sumber serta hasil pengujian aktual. Integrasi Supabase, validasi pada sisi backend atau database, mekanisme audit trail, dan perlindungan jurnal berstatus POSTED tidak boleh dianggap berhasil sebelum diverifikasi.

Apabila terdapat prompt tambahan, perubahan instruksi, atau proses perbaikan kode selama pengerjaan, dokumentasi ini perlu dilengkapi berdasarkan riwayat penggunaan AI yang sebenarnya.

---

**Disusun oleh:** Muhammad Ilman Assiediqie  
**NIM:** 12030123140343  
**Kelas:** E
