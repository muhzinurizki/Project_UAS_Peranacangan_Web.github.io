- Penting ⚠️. Install dependencies yang diperlukan dengan cara menjalankan perintah berikut di terminal:

```shell
composer install
```

- Buat database `db_book_library` di phpMyAdmin / mysql
- Penting ⚠️. Jalankan migrasi database untuk membuat struktur tabel yang diperlukan. Ketikkan perintah berikut di terminal:

```shell
php spark migrate --all
```

- Penting ⚠️. Karena belum memiliki akun admin, untuk mengakses halaman admin, anda memerlukan user/akun dengan level `superadmin`. Jalankan perintah berikut untuk membuat akun `superadmin`:

```shell
php spark db:seed SuperAdminSeeder
```

- (Opsional) Isi database dengan data dummy / seeder.

```shell
php spark db:seed Seeder # semua seeder
php spark db:seed BookSeeder # buku
php spark db:seed MemberSeeder # anggota
php spark db:seed LoanSeeder # peminjaman, pengembalian & denda
```

- Jalankan website

```shell
php spark serve
```

- Buka http://localhost:8080

- Login dengan kredensial `superadmin` berikut:

```
username : superadmin
email    : superadmin@admin.com
password : superadmin
```
