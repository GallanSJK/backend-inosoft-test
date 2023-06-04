# [Laravel 8 MongoDB](https://github.com/GallanSJK/backend-inosoft-test)

Laravel 8 + PHP 8 With MongoDB 4.2 (Test PT. INOSOFT TRANS SISTEM).

- [Installation](#installation)
  - [Developments](#developments)
  - [Requirements](#requirements)
  - [Copyright](#copyright)

## Installation

1. Clone repository
	```bash
	# Clone dengan SSH
	git clone git@github.com:GallanSJK/backend-inosoft-test.git
	# Clone dengan HTTPS
	git clone https://github.com/GallanSJK/backend-inosoft-test.git
  # Atau dengan mendownload folder zip
  https://github.com/GallanSJK/backend-inosoft-test/archive/refs/heads/master.zip
	```

2. Update composer :

```bash
composer update
```

3. Install vendors composer :

```bash
composer install
```

4. Copy File .env.example to .env :
Buat file `.env` di root project dan copy isi file `.env.example` ke `.env`  
Ubah konfigurasi sesuai keperluan.

```bash
cp .env.example .env
```

5. Generate key :

```bash
php artisan key:generate
```

6. Migrasi database
Pastikan konfigurasi database di `.env` sudah benar

```bash
php artisan migrate
```

7. Generate Secret Key JWT
Command Untuk Generate Key :

```bash
php artisan jwt:secret
```

Command diatas untuk mengupdate file `.env` seperti `JWT_SECRET=foobar`

8. Jalankan Project Laravel

```bash
php artisan serve
```

## Developments
1. Run Test   
Jalankan command dibawah ini untuk melakukan test (Menggunakan PHP Unit Test):
```bash
php artisan test
```

2. [Routes Viewer](http://127.0.0.1:8000/routes)   
Lihat list routes `/routes` langsung dari browser. List route akan tampil apabila  `APP_DEBUG` env bernilai true.

## Requirements
- PHP >= 8.0
- MySQL >= 8.0
- [Composer Requirements](https://getcomposer.org/download/)
- [MongoDB Requirements](https://www.mongodb.com/try/download/community) >= 4.2
- [Laravel Requirements](https://laravel.com/docs/8.x/installation) >= 8.x

## Copyright
2023 [Gallan Stefan Jayakelana](https://www.github.com/GallanSJK/)