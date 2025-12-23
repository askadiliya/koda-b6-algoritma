# Algoritma

## Analisis Proses Checkout Tokopedia

## Deskriptif

1. Mulai
2. masuk halaman tokopedia "https://www.tokopedia.com/"
3. Pilih barang yang diinginkan
4. Pilih jenis dan ukuran
5. Atur Jumlah dan catatan
6. silakan pilih masukan Keranjang atau Beli Langsung
7. Jika klik keranjang atau Beli Langsung maka sistem akan meminta user melakukan login
8. Masukan email dan password
9. Jika Username dan Password Benar maka user diminta untuk memasukan kode verivikasi yang dikirim melalui email
10. Masukan Kode verifikasi
11. Pilih barang yang sudahdipilih
12. Pilih Jasa Pengiriman
13. Pilih Metode Pembayaran 
14. klik bayar sekarang
15. Selesai

## Flowchart


```mermaid
flowchart TD
    A@{ shape: circle, label: "Mulai" }
    B@{ shape: rect, label: "Masuk halaman Tokopedia" }
    C@{ shape: rect, label: "Pilih barang" }
    D@{ shape: rect, label: "Pilih jenis & ukuran" }
    E@{ shape: rect, label: "Atur jumlah & catatan" }
    F@{ shape: diamond, label: "Keranjang / Beli Langsung?" }
    G@{ shape: lean-r, label: "Input Email & Password" }
    H@{ shape: diamond, label: "Login Valid?" }
    I@{ shape: lean-r, label: "Input Kode Verifikasi" }
    J@{ shape: rect, label: "Pilih barang yang dipilih" }
    K@{ shape: rect, label: "Pilih jasa pengiriman" }
    L@{ shape: rect, label: "Pilih metode pembayaran" }
    M@{ shape: rect, label: "Klik Bayar Sekarang" }
    N@{ shape: dbl-circ, label: "Selesai" }

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H -- False --> G
    H -- True --> I
    I --> J
    J --> K
    K --> L
    L --> M
    M --> N

    


```