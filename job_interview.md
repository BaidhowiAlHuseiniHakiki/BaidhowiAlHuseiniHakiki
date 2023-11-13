## 1.1 Latar Belakang

 Saya diprojek ini membuat website Toko Mamah Online. Toko Mamah Online adalah sebuah website yang menjual brand pakaian lokal yang original tidak kw. Pakaian adalah sebuah kebutuhan primer manusia selain makanan dan minuman. Jadi saya membuat website ini untuk memudahkan masyarakat dalam membeli pakaian agar tidak keluar rumah.

## 1.2. Deksripsi Teknologi Informasi

Website ini bertujuan untuk memudahkan masyarakat untuk membeli pakaian agar tidak keluar rumah. Maka dengan website ini orang bisa membeli pakaian kapan ajah tanpa harus datang langsung ke Toko Offline.

## 1.3. Branding
 - merk: Toko Mamah Online
 - Tagline: "kamu mau membeli pakaian? pesan di sini ajh."
 - Campaign: Silahkan untuk melakukan pembelian pakaian
 - Target User:
    -Usia: 10 tahun ke atas
    -Orang yang ingin membeli pakaian tanpa harus datang ke toko offline.
 - User Experience Theme:
    -Sederhana
    -Mudah
    
## 2. User Story

Sebagai | Saya ingin bisa | Sehingga | Prioritas
---|---|---|---
Penguna | Memesan baju | Bisa memakainya tanpa harus datang ke toko offline | ⭐⭐⭐⭐⭐
Pengguna | Memesan jaket | Bisa memakainya tanpa harus datang ke toko offline | ⭐⭐⭐⭐⭐
Pengguna | Memesan hoodie | Bisa memakainya tanpa harus datang ke toko offline | ⭐⭐⭐⭐⭐

## 3. Struktur Data
```mermaid
erDiagram
    pelanggan ||--o{ pelanggan : membeli
    pelanggan {
        char ID_pelanggan
        varchar namadepan
        varchar namabelakang
        varchar email
        varchar password
        varchar telp
    }
    produk ||--|{ produk : masuk
    produk {
        bigint ID_produk
        varchar nama_produk
        varchar deskripsi
        varchar harga
        varchar foto
        varchar category
        varchar stok
    }
    pesanan ||--|{ pesanan : menanggapi
    petugas {
        bigint id_petugas
        varchar nama_petugas
        varchar username
        varchar password
        varchar telp
        enum level
    }
    tanggapan {
        bigint id_tanggapan
        bigint id_pengaduan
        datetime tgl_tanggapan
        text tanggapan
        bigint id_petugas
}
```


## 4. Arsitektur Sistem



## 5. Teknologi, Library, dan Framework

Untuk teknologi saya menggunakan Visual Studio Code

## 6. Desain User Experience dan User Interface

![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/855de87b-de5e-4a78-bbe1-f42040abbf19)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/93746ded-124c-40d6-b7e3-e39af1ce5dc4)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/184dcd30-18a8-4be5-bc3a-e5e072fd40ae)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/6e23896c-1521-4254-ab65-4c6c0c5c123e)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/60316733-2040-4238-94d5-48d4da949c19)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/801a3f00-3754-41f3-9b77-aa9a130610c5)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/43859cd3-18dc-495c-8cc9-9918b2ccf021)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/24322ba1-78fe-4d13-aefe-1c7576d6add3)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/345d4761-973d-405a-8dbd-176e66353884)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/ea2e60e6-88d8-4686-815c-12cff3466578)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/8e88e3c4-ac85-4713-8490-1b679fb71739)
![image](https://github.com/BaidhowiAlHuseiniHakiki/BaidhowiAlHuseiniHakiki/assets/144520859/4dd1c31b-9779-4d2b-a0ce-32b19c856d0d)




## 7. Demonstrasi Video


## 8. Bagaimana mesin komputasi dan sistem operasi berperan dalam produk teknologi informasimu ?


## 9. Bagaimana algoritma, struktur data, dan bahasa pemrograman berperan dalam produk teknologi informasimu ?


## 10. Bagaimana metode pengembangan perangkat lunak / Software Development Life Cycle berperan dalam produk teknologi informasimu ?



## 11. Bagaimana database / sistem basis data berperan dalam produk teknologi informasimu ?


