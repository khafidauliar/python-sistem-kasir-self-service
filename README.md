# Project Python Sistem Kasir Self Service
## A. Latar Belakang Problem
Andi adalah seorang pemilik supermarket besar di salah satu kota di Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Andi akan membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain.
## B. Requirements / Objectives
1. Membuat Sistem Kasir Self Service yang memudahkan pelanggan dalam berbanja, dengan fitur sebagai berikut:
   - Pelanggan membuat ID transaksi atas transaksi yang telah dibuat.
   - Pelanggan dapat memasukkan nama barang, jumlah barang dan harga barang yang ingin dibeli.
   - Pelanggan dapat melakukan pembaruan barang, jumlah barang dan harga barang yang telah dipilih.
   - Pelanggan dapat menghapus barang yang telah dipilih.
   - Pelanggan dapat menghapus semua transaksi yang tidak jadi dibeli.
   - Pelanggan dapat melakukan pengecekan daftar belanjaan yang telah dipilih.
   - Pelanggan dapat melakukan pengecekan total harga belanjaan yang telah dipilih beserta diskon dengan ketentuan sebagai berikut:
     - Jika total belanja di atas Rp200.000 maka akan mendapat diskon 5%.
     - Jika total belanja di atas Rp300.000 maka akan mendapat diskon 8%.
     - Jika total belanja di atas Rp500.000 maka akan mendapat diskon 10%
2. Membuat Sistem Kasir Self Service menggunakan Python.
3. Menggunakan Modular Code dalam membuat program di Python.
4. Menggunakan konsep OOP dalam membuat program di Python.
5. Menerapkan prinsip Clean Code (PEP8) dalam membuat program di Python.
6. Membuat dokumentasi Docstring di Class atau Function di program yang telah dibuat.
7. Mengimplementasikan Data Structure, Branching dan Try Error dalam membuat program di Python.
8. Menggunakan library sesuai dengan kebutuhan.
## C. Alur Code / Flowchart

![flowchart](https://user-images.githubusercontent.com/123468166/216752864-2062b52f-a72a-46de-80d3-116e38e65351.png)

## D. Function / Attribute
Pada script `main.py` berfungsi untuk memanggil modul `transaction.py` yang memiliki function/attribute sebagai berikut:
1. `__init__` : fungsi yang di dalamnya menyimpan attribute `data_trx` yang memiliki tipe data dictionary untuk menyimpan data transaksi.
2. `add_item` : fungsi untuk menambahkan data transaksi berupa `nama_item`, `jumlah_item` dan `harga_per_item`.
3. `update_item_name` : fungsi untuk memperbarui `nama_item`.
4. `update_item_qty` : fungsi untuk memperbarui `jumlah_item`.
5. `update_item_price` : fungsi untuk memperbarui `harga_per_item`.
6. `delete_item` : fungsi untuk menghapus salah satu `nama_item`.
7. `reset_transaction` : fungsi untuk menghapus seluruh item yang telah dipesan.
8. `check_order` : fungsi untuk menampilkan list item yang telah dipesan.
9. `total_price` : fungsi untuk menghitungan total harga yang telah dipesan dan diskon sesuai dengan ketentuan di atas.
## E. Test Case
#### Test Case 1 :
Pelanggan ingin menambahkan dua item baru menggunakan method `add_item`. Item yang ditambahkan adalah sebagai berikut:
- Nama Item: Ayam Goreng, Qty: 2, Harga: 20000
- Nama Item: Pasta Gigi, Qty: 3, Harga: 15000

Output:

![testcase1](https://user-images.githubusercontent.com/123468166/216752806-f85413e8-1daf-43cb-9afd-495fc42d5693.PNG)

#### Test Case 2 :
Pelanggan salah membeli salah satu item dari belanjaan yang sudah ditambahkan, maka pelanggan menggunakan method `delete_item` untuk menghapus item. Item yang ingin dihapuskan adalah 'Pasta Gigi'.

Output:

![testcase2](https://user-images.githubusercontent.com/123468166/216752891-0062847d-ccf8-4816-ba36-0f81f5921f2e.PNG)

#### Test Case 3 :
Pelanggan ingin menggunakan method `reset_transaction` untuk menghapus semua item yang sudah ditambahkan, dibandingkan menghapus satu-satu per item.

Output:

![testcase3](https://user-images.githubusercontent.com/123468166/216752901-0a177eca-1427-4c9a-a21c-92de1e360247.PNG)

#### Test Case 4 :
Setelah pelanggan selesai berbelanja, program akan menghitung total belanjaan yang harus dibayarkan menggunakan method `total_price`. Sebelum mengeluarkan output total belanja akan menampilkan item-item yang dibeli.

Output:

![testcase4](https://user-images.githubusercontent.com/123468166/216752905-1544a56a-dd86-4ace-959d-48c11b9f8965.PNG)

#### Test Case 5 :
Pelanggan ternyata ingin melakukan perubahan pada item-item yang telah masuk ke dalam list, perubahannya sebagai berikut:
- Melakukan update nama item 'Ayam Goreng' menjadi 'Ayam Geprek' menggunkan method `update_item_name`.
- Melakukan update jumlah item 'Pasta Gigi' yang menjadi '10' menggunkan method `update_item_qty`.
- Melakukan update harga item 'Mainan Mobil' yang menjadi '300000' menggunkan method `update_item_price`.

Output:

![testcase5](https://user-images.githubusercontent.com/123468166/216752917-fffced7d-313f-4ebc-b3e1-9ceec494a05e.PNG)

## F. Kesimpulan
Sistem kasir self service secara keseluruhan telah sesuai dengan kebutuhan Andi, akan tetapi ada beberapa catatan untuk peningkatan sistem kasir self service agar lebih baik ke depannya, antara lain:
1. Agar ke depannya data transaksi yang telah dibuat pelanggan dapat disimpan di database.
2. Setelah data disimpan dalam database, data tersebut dapat dilakukan analisa maupun visualisasi sesuai dengan kebutuhan Andi.


**Author** Copyright (c) 2023 Khafid Aulia Rahman
