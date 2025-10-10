# Kali Linux – Command

Berikut ini beberapa perintah dasar yang umum digunakan di Kali Linux.

## List of Kali Linux Command

### Linux Filesystem

### Basic Command

- `pwd`: Menampilkan direktori saat ini.

!!! example "Penggunaan perintah `pwd`"

    ```bash
    pwd
    ```

- `whoami`: Menampilkan pengguna yang sedang aktif (baik user biasa atau root).

!!! example "Penggunaan perintah `whoami`"

    ```bash
    whoami
    ```

- `cd`: Berpindah direktori.

!!! example "Penggunaan perintah `cd`"

    ```bash
    cd newfolder
    ```

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

!!! example "Contoh penggunaan `ls -l - a` atau `ls -la`"
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
- `find`: Mencari lokasi file secara lebih powerfull.

!!! info "`find` Basic Syntax"

`find` `directory options` `expressions`

- `grep`: Mencari dan memanipulasi teks dalam sebuah file dan direktori di Kali Linux dengan menggunakan keyword spesifik.

### Modifying Files and Directories

#### Creating Files

- `cat`: Membuat file di Linux.
- `touch`

!!! example "Penggunaan perintah `cat`"

    ```bash
    cat > coba.txt
    ```

!!! info "Perintah `cat` di Kali Linux"

!!! example "Membuat file baru"

    Basic _syntax_:

    ```
    cat > nama_file.extension file
    ```

    ```bash
    cat > coba.txt
    ```

- Tekan `CTRL + D` untuk keluar dan kembali ke _prompt_ jika telah memasukkan isi file.

!!! example "Menampilkan isi file"

    ```bash
    cat coba.txt
    ```

- Perintah `cat` tanpa tanda `>` digunakan untuk melihat isi file.

!!! example "Menambahkan konten baru ke dalam file"

    ```bash
    cat >> coba.txt
    ```

- Perintah `cat` dengan tanda `>>` digunakan untuk menambahkan konten baru ke dalam file.

!!! example "_Overwrite_ file"

    ```bash
    cat > coba.txt
    ```

- Perintah `cat` dengan tanda `>` digunakan untuk meng-_overwrite_ file.

!!! info "Pembuatan file di Kali Linux"

- Secara teknis, pengguna bisa membuat file di Kali Linux baik dengan menambahkan _file extension_ atau tanpa _file extension_ sama sekali.

#### Creating Directory

- `mkdir`: Membuat folder di Linux.

!!! example "Penggunaan perintah `mkdir`"

    ```bash
    mkdir newfolder
    ```

!!! info "Navigasi ke Folder yang telah dibuat"
    Gunakan perintah `cd` untuk berpindah ke folder atau direktori yang telah dibuat.

    ```bash
    cd newfolder
    ```

#### Copying Files

`cp`: Meng-copy file.

Syntax dasar:

cp [source_file] [destination]

!!! example "Penggunaan perintah `cp`"

    ```bash
    cp newfile /home/momoi/newfolder
    ```

!!! info "Perintah `cp`"
    Jika ingin menyalin dan mengganti nama file nya, bisa dengan cara berikut.

    ```bash
    cp newfile /home/momoi/newfolder/newfile-copy
    ```

#### Renaming File

`mv`: Memindahkan file dari satu direktori ke direktori yang lain atau mengganti nama file

!!! example "Penggunaan perintah `mv`"

    ```bash
    mv file-copy filecopy
    ```

#### Removing File

`rm`: Menghapus file

!!! example "Penggunaan perintah `rm`"

    ```bash
    rm filecopy
    ```

#### Removing Directory / Folder

`rmdir`: Menghapus direktori / folder

!!! example "Penggunaan perintah `rmdir`"

    ```bash
    rmdir newfolder
    ```

!!! info "Catatan untuk penggunaan perintah `rmdir`"

Pastikan direktori atau folder yang ingin dihapus telah kosong (tidak ada isian konten), karena kalau masih ada file / isian konten akan mengeluarkan _output_ error berikut

    rmdir: failed to remove 'newfolder': Directory not empty

Atau bisa dengan menambahkan `-r` agar direktori serta file yang berada didalamnya akan terhapus semuanya.

!!! example "Menghapus direktori beserta isinya"

    ```bash
    rmdir newfolder -r
    ```
