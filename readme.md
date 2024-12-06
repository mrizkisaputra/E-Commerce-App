# Ecommerce App

Ini adalah aplikasi e-commerce yang dirancang untuk mempermudah pengguna dalam belanja online dan mendukung admin dalam
pengelolaan produk serta inventaris. Tujuan dari proyek ini adalah untuk memahami cara membangun aplikasi yang
mengandalkan logika dengan model data yang kompleks.

## Features

Berikut adalah fitur-fitur yang ada saat ini, dan akan terus dikembangkan:

1. **Panel Admin:**
    - kemampuan bagi admin untuk login
    - kemampuan bagi admin merubah password
    - kemampuan bagi admin untuk mengelola produk (insert, update, dan delete)
    - kemampuan bagi admin untuk mengelola inventaris
    - Kemampuan bagi admin untuk mengelola pesanan pengguna (melihat, mengubah status pesanan)

2. **Integrasi dengan Payment Gateway (Stripe)**
    - Menggunakan Stripe untuk pembayaran

3. **Pengguna:**
    - menyediakan API untuk registrasi dan login pengguna
    - menyediakan API untuk melihat dan mencari produk
    - menyediakan API untuk menambahkan produk ke keranjang
    - menyediakan API untuk menghapus produk dari keranjang
    - menyediakan API untuk memeriksa dan membayar produk

## Endpoint API

Berikut adalah endpoint API Pengguna:

- ``POST api/v1/auth/register``: Endpoint untuk registrasi
- ``POST api/v1/auth/login``: Endpoint untuk login
- ``GET api/v1/products``: Endpoint untuk mendapatkan semua produk
- ``GET api/v1/products?name=shoes``: Endpoint untuk mencari produk
- ``POST api/v1/cart``: Endpoint untuk menambah produk ke keranjang
- ``DELETE api/v1/cart?product_id=001``: Endpoint untuk menghapus produk dari keranjang

## Tech Stack

Daftar teknologi dan library apa saja yang digunakan:

- [Golang v1.23.3]() (programming language)
- [PostgreSQL v8]() (relational database)
- [MongoDB v]() (document oriented database)
- [Redis v]() (key value database)
- [Docker v]() (containerize)
- [Gofiber v2](https://docs.gofiber.io/) (http framework)
- [Logrus v1.9.3](https://github.com/sirupsen/logrus) (logging)
- [Go Playground v10.23.0](https://github.com/go-playground/validator) (validation)
- [Go JWT](https://github.com/golang-jwt/jwt) (JSON web token)
- [HTML v2.x.x](https://docs.gofiber.io/template/html/) (golang template engine)

## Design Schema Relational Database

Tidak perlu membuat dalam bentuk ERD yang kompleks, karena mungkin saja pada saat implementasi ada beberapa attribute
yang tidak ada. Cukup tentukan saja
entity apa saja yang terlibat dan juga kardinalitasnya:

## Application Architecture Drawing

Ini adalah gambaran dari aplikasi yang akan dibuat

## Run to Run this Application   

### Local Development Usage
    make run
