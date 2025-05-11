# Program Jumlah Hari Berdasarkan Bulan dan Tahun

Program ini dibuat menggunakan bahasa pemrograman Java dan bertujuan untuk menentukan jumlah hari dalam sebuah bulan berdasarkan input bulan dan tahun dari pengguna.

## 📌 Fitur
- Input tahun (misalnya: 2024)
- Input bulan (1–12)
- Menentukan jumlah hari dalam bulan tersebut, dengan memperhitungkan tahun kabisat

## 💡 Logika Utama
- Menggunakan `switch` untuk menentukan jumlah hari berdasarkan bulan.
- Untuk bulan Februari (2), dilakukan pemeriksaan apakah tahun merupakan tahun kabisat:
  ```java
  if (((tahun % 4 == 0) && !(tahun % 100 == 0)) || (tahun % 400 == 0))
  ```
- Menampilkan jumlah hari berdasarkan bulan dan tahun yang dimasukkan.

## 🧪 Contoh Output
```
Masukkan Tahun : 
2024
Masukkan Bulan : 
2
Jumalah hari pada 2024 bulan 2 adalah 29 hari
```

## 🛠 Dibuat Dengan
- Java SE
- Scanner untuk input dari pengguna
- Struktur kontrol `switch` dan `if-else`
