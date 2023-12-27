
#   Aplikasi Task Manager

Ini adalah aplikasi Node.js sederhana yang berinteraksi dengan database MongoDB untuk melakukan berbagai operasi terkait manajemen tugas dan pengguna. Berikut adalah gambaran singkat tentang setiap file dalam proyek ini:

## `deleteDocument.js`

File ini terhubung ke database MongoDB dan menghapus satu dokumen tugas berdasarkan deskripsinya (dalam kasus ini, 'Membersihkan rumah'). Ini menggunakan metode `deleteOne` untuk menjalankan operasi ini. Jika berhasil, hasilnya dicatat dalam konsol.

## `insertDocument.js`

File ini terhubung ke database MongoDB dan memasukkan data ke dalam dua koleksi: 'pengguna' dan 'tugas'. Ini menjelaskan cara membuat ObjectId baru, memasukkan satu dokumen menggunakan `insertOne`, dan memasukkan beberapa dokumen menggunakan `insertMany`. Ini juga memperlihatkan berbagai operasi terkait ObjectId dan penanganan kesalahan.

## `readDocument.js`

Dalam file ini, aplikasi terhubung ke database MongoDB dan melakukan berbagai operasi baca pada koleksi 'pengguna'. Ini menjelaskan cara mencari dokumen berdasarkan nama, berdasarkan ObjectId, dan berdasarkan kriteria tertentu (dalam kasus ini, pengguna dengan usia 25). Hasilnya dicatat dalam konsol, beserta penanganan kesalahan.

## `updateDocument.js`

File ini terhubung ke database MongoDB dan memperbarui data dalam koleksi 'tugas'. Ini menggunakan metode `updateMany` untuk memperbarui beberapa dokumen dengan mengatur nilai 'StatusPenyelesaian' menjadi true untuk tugas-tugas dengan status false. File ini juga mencakup kode yang di-comment untuk menggunakan metode `updateOne` untuk memperbarui nama dan usia satu pengguna. Hasil dari jumlah dokumen yang diubah dicatat, dan penanganan kesalahan dilakukan.
