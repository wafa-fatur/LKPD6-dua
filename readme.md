# LKPD 6: Merge Conflict & Resolution

### Nama Anggota

1.Wafa
2.Abdul

### 1. Apa yang dimaksud dengan Merge Conflict dalam Git?
Merge Conflict adalah kondisi ketika Git mengalami kebingungan saat menggabungkan perubahan dari dua branch karena terdapat dua perubahan berbeda pada baris kode yang sama.

### 2. Pesan error/peringatan yang muncul saat terjadi conflict
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

### 3. `<<<<<<< HEAD`
Menunjukkan kode yang sedang digunakan pada branch saat ini atau **HEAD**.
### 4. `=======`
Menjadi pemisah antara dua versi kode yang mengalami conflict.
### 5. `>>>>>>> fitur-header-b`
Menunjukkan akhir dari perubahan yang berasal dari branch `fitur-header-b`.

### Kasus 1
**Perintah Git untuk membatalkan proses merge:**
```bash
git merge --abort
```
Perintah tersebut digunakan untuk membatalkan proses merge yang sedang mengalami masalah dan kembali ke kondisi sebelum merge.

### Kasus 2
**Apakah merge conflict selalu berarti ada anggota tim yang melakukan kesalahan?**
Tidak. Merge conflict tidak selalu berarti ada anggota tim yang melakukan kesalahan. Conflict dapat terjadi karena dua developer mengubah baris kode yang sama dengan isi yang berbeda pada branch yang berbeda.
Pada simulasi ini, Developer A membuat versi terang dan Developer B membuat versi gelap. Ketika kedua branch digabungkan, Git mengalami conflict karena terdapat perubahan berbeda pada bagian kode yang sama.
