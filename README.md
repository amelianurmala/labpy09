# labpy09
# Latihan OOP
## Nama : Amelia Nurmala Dewi (312410199)
## Kelas : TI.24.A2





___

### Data -> Mahasiswa.py

![Screenshot (183)](https://github.com/user-attachments/assets/fb5e3558-433e-4bd7-a36f-0472326d0b2a)

### Penjelasan

- Kelas `Mahasiswa` digunakan untuk menyimpan data mahasiswa.
- Metode `__init__` adalah konstruktor yang dipanggil saat objek dibuat, untuk menginisialisasi atribut `nim`, `nama`, dan `jurusan`.
- Metode `__str__` mengembalikan representasi string dari objek dalam format: `NIM - Nama (Jurusan)`. Metode ini otomatis dipanggil saat objek dicetak menggunakan `print()` atau dikonversi ke string.

  


### View -> Input_form.py

![Screenshot (184)](https://github.com/user-attachments/assets/e6c1d408-5bcb-4e4c-8185-ff5963e1c5a3)

### Penjelasan

- `@staticmethod`: Menandai metode `input_data` sebagai metode statis, sehingga dapat dipanggil tanpa membuat objek dari kelas.
- `input_data()`: Mengambil data dari pengguna melalui input konsol untuk `nim`, `nama`, dan `jurusan`, lalu mengembalikan ketiga nilai tersebut dalam bentuk tuple.

  


### View -> Mahasiswa.py 

![Screenshot (185)](https://github.com/user-attachments/assets/18aff5a0-d716-4f01-b717-ccc09c2ca4a3)

![Screenshot (186)](https://github.com/user-attachments/assets/764518ea-e81d-4ae0-a1bd-471a569091d3)

### penjelasan

1. **`__init__`**: 
   - Inisialisasi atribut `data_mahasiswa` sebagai daftar kosong untuk menyimpan objek `Mahasiswa`.

2. **`tambah_data`**:
   - Mengambil input data menggunakan `InputForm.input_data`, membuat objek `Mahasiswa`, dan menambahkannya ke `data_mahasiswa`.

3. **`tampilkan_data`**:
   - Menampilkan daftar mahasiswa. Jika kosong, menampilkan pesan "Tidak ada data mahasiswa."

4. **`hapus_data`**:
   - Menampilkan data mahasiswa, meminta pengguna memilih nomor data untuk dihapus, lalu menghapusnya dari `data_mahasiswa`.

5. **`ubah_data`**:
   - Menampilkan data mahasiswa, meminta pengguna memilih nomor data untuk diubah, lalu memperbarui `nim` dan `nama` pada data tersebut menggunakan input baru.

     


### Main.py (input)

![Screenshot (180)](https://github.com/user-attachments/assets/68e6356b-e9dc-4fc2-a0e8-a3d0ae05c409)

![Screenshot (182)](https://github.com/user-attachments/assets/bd4c9422-c89c-4b6a-a030-f75bf87a641c)

### Penjelasan

1. **Kelas `Mahasiswa`:**
   - **Atribut:**
     - `self.data`: List untuk menyimpan data mahasiswa berupa dictionary dengan kunci `'nama'` dan `'nim'`.

   - **Metode:**
     - `tambah_data()`: 
       - Meminta input nama dan NIM, lalu menyimpan data ke dalam atribut `data`.
     - `tampilkan_data()`: 
       - Menampilkan semua data mahasiswa. Jika kosong, menampilkan pesan "Tidak ada data mahasiswa."
     - `ubah_data()`: 
       - Menampilkan data, meminta nomor data untuk diubah, lalu memperbarui nama dan NIM berdasarkan input baru.
     - `hapus_data()`: 
       - Menampilkan data, meminta nomor data untuk dihapus, lalu menghapus data dari list.

2. **Fungsi `main()`:**
   - Mengelola interaksi pengguna melalui menu:
     - Opsi **1**: Menambahkan data mahasiswa.
     - Opsi **2**: Menampilkan data mahasiswa.
     - Opsi **3**: Mengubah data mahasiswa.
     - Opsi **4**: Menghapus data mahasiswa.
     - Opsi **5**: Keluar dari program.
   - Menggunakan perulangan `while True` untuk menjalankan menu hingga pengguna memilih opsi keluar.

3. **Eksekusi Program:**
   - Program dijalankan dengan memanggil fungsi `main()` jika file dijalankan secara langsung (`if __name__ == "__main__":`).

### Alur Kerja:
- Pengguna memilih menu melalui input angka.
- Program menjalankan fungsi terkait berdasarkan pilihan menu.
- Data mahasiswa dikelola menggunakan list `self.data`, dengan setiap entri berupa dictionary.

### Contoh Penggunaan:
- Menambahkan data mahasiswa dengan nama dan NIM.
- Melihat daftar mahasiswa.
- Mengubah atau menghapus data berdasarkan nomor urut.





### Main.py (output)

![Screenshot (178)](https://github.com/user-attachments/assets/b53a6986-4926-426c-ac89-7311f215461e)

![Screenshot (179)](https://github.com/user-attachments/assets/956f871e-f77a-49e9-aacd-71294e221f32)




