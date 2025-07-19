## Kali Linux – Command

Berikut ini beberapa perintah dasar yang umum digunakan di Kali Linux.

### Basic Command 

- `pwd`: Menampilkan direktori saat ini.
- `whoami`: Menampilkan pengguna yang sedang aktif (baik user biasa atau root).
- `cd`: Berpindah direktori.

!!! info "Command `cd`"
    ```
    ..         → naik satu level folder
    ../..      → naik dua level folder
    ../../..   → naik tiga level folder, dan seterusnya
    ```

- `ls`: Melihat isi konten dari direktori saat ini (file dan subdirektori).

!!! info "Command `ls`"
    Untuk mendapatkan informasi lebih lengkap mengenai file atau direktori, 
    gunakan opsi tambahan seperti `-l` atau `-a`.

!!! example "Contoh penggunaan `ls`"
    ```bash
    ls -l -a
    # atau
    ls -la
    ```

!!! info "Mendapatkan Bantuan"
    Gunakan perintah `--help`, `-h`, atau `-?` untuk melihat petunjuk penggunaan perintah di Kali Linux.

!!! info "Referensi Manual (Manual Pages)"
    Gunakan perintah `man` diikuti nama command untuk melihat dokumentasi lengkap, misalnya:
    ```bash
    man ls
    ```

---

### Finding Files

- `locate`: Mencari lokasi file berdasarkan database file sistem. Gunakan perintah `updatedb` untuk mengupdate database file sistem.
- `whereis`: Mencari lokasi file binary.
- `which`: Mencari lokasi file binary dalam PATH Variable.
- `find`: Mencari lokasi file secara lebih powerfull 

!!! info "`find` Basic Syntax"

`find` `directory options` `expressions`

- `grep`: Mencari dan memanipulasi teks dalam sebuah file dan direktori di Kali Linux dengan menggunakan keyword spesifik. 

### Modifying Files and Directories