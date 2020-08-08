# Phase 2 - Live Code 1

## BabiesFactory
Pada kali ini kalian akan membuat sebuah website yang dapat menampilkan list of babies, menambahkan babies (name, img), serta menghapus babies yang tidak kalian suka

### Summary
- Menggunakan sequelize n postgres dan jquery html css
- Memberikan environtment variables jika menggunakan node env
- Dilarang menggunakan alert()
- SPA & **Reactive**

## Release 0 - Authentication

### Server - Register

- buatlah register sesuai api-doc
- password di hash
- email dan password di validasi

### Server - Login

- buatlah login sesuai api-doc

### Client - Login & Logout

- jika sudah login, kalau direfresh tidak harus login lagi
- logout berhasil dan menghapus localstorage
- jika berhasil login, tombol logout muncul, form login ke hide
- Sehabis login, data babies langsung muncul (fetch babies ada di release 2)

NOTES: REGISTER CLIENT TIDAK PERLU ADA

Contoh halaman login (gambar ini hanya layout, jika kalian membuat lebih baik dan rapi sangat diperbolehkan):
![login](https://imgur.com/vbZeWl7.jpg)

## Release 1 - POST Babies

### Server

- buatlah Post Babies sesuai api-doc (sesuaikan dengan request dan response nya)
- authentication needed

### Client

- integrasikan form yang ada 

Contoh halaman post babies (gambar ini hanya layout, jika kalian membuat lebih baik dan rapi sangat diperbolehkan):
![login](https://imgur.com/l4ihAPq.jpg)

## Release 2 - Fetch Babies List

### Server

- buatlah fetch babies sesuai api-doc (sesuaikan dengan request dan response nya)
- authentication needed

### Client

- Tampilkan daftar babies sesuai user yang sedang login

Contoh halaman fetch babies (gambar ini hanya layout, jika kalian membuat lebih baik dan rapi sangat diperbolehkan):
![login](https://imgur.com/k3MBvmM.jpg)

## Release 3 - Delete babies

### Server

- buatlah delete babies sesuai api-doc
- gunakan authentication && authorization

### Client

- Integrasikan tombol delete yang ada pada detail babies dengan fungsi delete
