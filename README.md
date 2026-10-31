# Pertemuan 11 — Dictionary/Map

## Identitas Mahasiswa

* **Nama:** Maila Andira Putri
* **NIM:** 2225250126
* **Kelas:** 3A

## Deskripsi

Repository ini berisi hasil praktikum Algoritma dan Pemrograman Pertemuan 11 tentang penggunaan Dictionary/Map dalam Python.

Praktikum ini membahas cara menyimpan dan mengelola data pendidikan menggunakan struktur dictionary dengan pasangan `key-value`. Data yang digunakan berupa informasi mahasiswa, seperti NIM, nama, kelas, dan nilai. Program juga menerapkan dictionary bersarang untuk memudahkan pencarian, penambahan, perubahan, dan penampilan data mahasiswa.

## 1. Tujuan Praktikum

1. Memahami penggunaan dictionary dalam Python.
2. Memahami konsep pasangan `key-value`.
3. Menerapkan NIM sebagai key utama dalam penyimpanan data mahasiswa.
4. Mengelola data mahasiswa menggunakan dictionary bersarang.
5. Melakukan pencarian data berdasarkan NIM.
6. Menambahkan dan mengubah data mahasiswa.
7. Menampilkan seluruh data menggunakan method `items()`.
8. Menghindari kesalahan `KeyError` ketika mengakses key yang tidak tersedia.

## 2. Struktur Data

Program ini menggunakan dictionary untuk menyimpan data mahasiswa. NIM digunakan sebagai key utama, sedangkan nama, kelas, dan nilai digunakan sebagai value.

Setiap data mahasiswa disimpan dalam dictionary bersarang (*nested dictionary*), sehingga informasi mahasiswa dapat dicari dan dikelola berdasarkan NIM.

Contoh struktur dictionary:

```python
data_mahasiswa = {
    "A001": {
        "nama": "Andi",
        "kelas": "3A",
        "nilai": 85
    },
    "A002": {
        "nama": "Budi",
        "kelas": "3A",
        "nilai": 80
    }
}
```

Pada struktur tersebut, setiap NIM menjadi key utama yang terhubung dengan informasi mahasiswa.

## 3. Pengelolaan Data Mahasiswa

Program melakukan beberapa operasi dictionary, yaitu:

1. **Pencarian data:** mencari mahasiswa berdasarkan NIM.
2. **Penambahan data:** memasukkan data mahasiswa baru ke dalam dictionary.
3. **Perubahan data:** mengubah nilai mahasiswa berdasarkan NIM.
4. **Penampilan data:** menampilkan seluruh informasi mahasiswa menggunakan `items()`.
5. **Perhitungan rata-rata:** menghitung rata-rata nilai seluruh mahasiswa.

## 4. Cara Menjalankan Program

Pastikan Python telah terpasang dan folder tugas sudah dibuka melalui Visual Studio Code (VS Code).

Langkah-langkah menjalankan program:

1. Buka folder tugas melalui Visual Studio Code.
2. Buka folder `praktik`.
3. Pilih file `data_mahasiswa.py`.
4. Jalankan program menggunakan tombol **Run Python File** atau terminal.

Perintah yang digunakan:

```bash
python praktik/data_mahasiswa.py
```

Jika perintah `python` tidak dikenali pada Windows, gunakan:

```bash
py praktik/data_mahasiswa.py
```

## 5. Test Case

Pengujian dilakukan untuk memastikan setiap operasi dictionary dapat berjalan sesuai dengan hasil yang diharapkan.

| No. | Pengujian                                      | Hasil                |
| --: | ---------------------------------------------- | -------------------- |
|   1 | Mencari NIM A003                               | Data Citra ditemukan |
|   2 | Mencari NIM A999                               | Data tidak ditemukan |
|   3 | Mengubah nilai A002 menjadi 82                 | Berhasil             |
|   4 | Menambahkan mahasiswa A006                     | Berhasil             |
|   5 | Menampilkan seluruh data menggunakan `items()` | Berhasil             |

### Hasil Perhitungan

Hasil perhitungan rata-rata nilai seluruh mahasiswa adalah:

```text
Rata-rata nilai mahasiswa: 83.50
```

## 6. Refleksi

Selama mengerjakan praktikum ini, saya memahami bahwa dictionary dapat digunakan untuk menyimpan data dalam bentuk pasangan `key-value`. Penggunaan NIM sebagai key memudahkan proses pencarian informasi mahasiswa tanpa harus mencari berdasarkan posisi indeks seperti pada list.

Salah satu kesalahan yang perlu diperhatikan adalah `KeyError`, yaitu ketika program mengakses key yang tidak tersedia dalam dictionary. Kesalahan tersebut dapat dihindari dengan menggunakan method `get()` atau memeriksa keberadaan key menggunakan operator `in`.

Melalui latihan ini, saya juga memahami cara menambahkan, mengubah, mencari, dan menampilkan data mahasiswa menggunakan dictionary dalam Python.

## 7. Kesimpulan

Berdasarkan praktikum Pertemuan 11, dapat disimpulkan bahwa dictionary merupakan struktur data Python yang dapat digunakan untuk menyimpan informasi dalam bentuk pasangan `key-value`. Dengan menggunakan dictionary bersarang, data mahasiswa dapat dikelola berdasarkan NIM sehingga proses pencarian dan perubahan informasi menjadi lebih mudah. Selain itu, penggunaan method seperti `get()` dan `items()` membantu dalam mengakses serta menampilkan data secara lebih terstruktur.

