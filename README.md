# Angular Task Manager

Proyek latihan CRUD sederhana menggunakan Angular (frontend) dan PHP Slim + PostgreSQL (backend). Dibuat untuk belajar framework baru.

> ⚠️ **Status: Work in Progress** — proyek ini masih dalam pengembangan, beberapa fitur mungkin belum lengkap atau masih disempurnakan.

## Tentang Proyek

Task Manager sederhana yang memungkinkan pengguna untuk:
- Menambahkan task baru
- Menandai task sebagai selesai/belum selesai
- Menghapus task
- Melihat daftar task yang tersimpan di database

## Tech Stack

**Frontend:**
- Angular 21 (standalone components)
- TypeScript
- RxJS

**Backend:**
- PHP Slim Framework
- PostgreSQL

## Struktur Proyek

```
src/app/
  app.ts, app.html, app.config.ts   -> root component & konfigurasi
  task.ts                            -> model & service (CRUD API calls)
  task-list/                         -> komponen tampilan daftar task
```

## Menjalankan Proyek Secara Lokal

### Frontend (Angular)

Pastikan Node.js dan Angular CLI sudah terinstall, lalu jalankan:

```bash
npm install
ng serve
```

Buka `http://localhost:4200/` di browser. Aplikasi akan otomatis reload setiap ada perubahan pada source file.

### Backend (PHP Slim)

Backend berjalan terpisah di folder lain (`task-manager-api`). Pastikan PHP, Composer, dan PostgreSQL sudah terinstall, lalu jalankan:

```bash
php -S localhost:8080 -t public
```

Pastikan database PostgreSQL dan konfigurasi `.env` sudah disesuaikan sebelum menjalankan backend.

## Code Scaffolding

Angular CLI menyediakan tools scaffolding untuk generate komponen baru:

```bash
ng generate component component-name
```

Untuk daftar lengkap schematic yang tersedia (components, directives, pipes):

```bash
ng generate --help
```

## Build

```bash
ng build
```

Hasil build akan tersimpan di folder `dist/`. Secara default, production build sudah dioptimasi untuk performa.

## Unit Testing

Menjalankan unit test dengan [Vitest](https://vitest.dev/):

```bash
ng test
```

## End-to-End Testing

Angular CLI tidak menyertakan framework e2e testing secara default. Kamu bisa memilih framework yang sesuai kebutuhan.

```bash
ng e2e
```

## To-Do

- [ ] Styling tampilan (masih default browser)
- [ ] Validasi input
- [ ] Error handling untuk request yang gagal
- [ ] Deployment ke server

## Referensi

Proyek ini dibuat menggunakan [Angular CLI](https://github.com/angular/angular-cli) versi 21.2.23. Untuk dokumentasi lebih lanjut, kunjungi [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli).
