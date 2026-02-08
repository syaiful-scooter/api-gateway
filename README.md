# [Api-Gateway] with springboot

## 📌 Deskripsi Singkat [Backend]
"Service springboot untuk menjadi api gateway yang mengautomasi & meneruskan request ke servis yang di tuju."

## 🚀 Fitur Utama
- **[Fitur 1]:** Satu pintu masuk utama (single entry point) yang berdiri di depan sekelompok layanan (microservices).
- **[Fitur 2]:** menerima permintaan dari luar dan menentukan ke service mana permintaan tersebut harus dikirim berdasarkan URL-nya.
- **[Fitur 3]:** Gateway akan membagi request secara merata agar tidak ada satu pun server yang keberatan beban.
- **[Fitur 4]:** Monitoring

## 🛠️ Depedency Properties
Daftar teknologi yang digunakan dalam proyek ini:
- **[Monitoring]:** [spring-boot-starter-actuator]
- [spring-cloud-starter-gateway]
- [spring-boot-devtools]
- [lombok]
- [spring-boot-starter-test]


## Ringkasan Cara kerjanya

Jika kamu mengakses...,             Maka Gateway meneruskannya ke...

localhost:8888/v1/master/users, &rarr; localhost:9091/v1/master/users
localhost:8888/v1/transaction/buy,   localhost:9092/v1/transaction/buy
localhost:8888/v1/data/report,      localhost:9092/v1/data/report
localhost:8888/actuator/health,     (Internal Gateway) Mengecek status aplikasi


Dibuat dengan ❤️ oleh syaifulscooter