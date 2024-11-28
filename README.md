# Praktikum-7
Praktikum 7
Tugas Praktikum 7 Mata Kuliah Program Komputer dan Praktek

Penjelasan Pemrograman
1. Inisialisasi Dictionary
Program dimulai dengan membuat dictionary kosong yang akan menyimpan data. Misalnya:
python
data_mahasiswa = {}

2. Menampilkan Menu
Program akan menampilkan menu pilihan kepada pengguna:
python
print("Menu:")
print("1. Tambah Data")
print("2. Ubah Data")
print("3. Hapus Data")
print("4. Tampilkan Data")
print("5. Cari Data")
print("6. Keluar")

3. Input Pilihan
Pengguna diminta untuk memilih opsi dari menu:
python
pilihan = input("Masukkan pilihan (1-6): ")

4. Tambah Data
Jika pengguna memilih untuk menambah data:
Program meminta input untuk nama dan detail lainnya (NIM, nilai, dll).
Menyimpan data dalam dictionary.
python
if pilihan == '1':
    nama = input("Nama: ")
    nim = input("NIM: ")
    # Simpan data dalam dictionary
    data_mahasiswa[nama] = {'NIM': nim}

5. Ubah Data
Jika pengguna memilih untuk mengubah data:
Program meminta nama yang ingin diubah.
Jika nama ada dalam dictionary, minta detail baru dan perbarui.
python
elif pilihan == '2':
    nama = input("Nama yang ingin diubah: ")
    if nama in data_mahasiswa:
        nim_baru = input("NIM baru: ")
        data_mahasiswa[nama]['NIM'] = nim_baru

6. Hapus Data
Jika pengguna memilih untuk menghapus data:
Program meminta nama yang ingin dihapus.
Menghapus entri dari dictionary jika ada.
python
elif pilihan == '3':
    nama = input("Nama yang ingin dihapus: ")
    if nama in data_mahasiswa:
        del data_mahasiswa[nama]

7. Tampilkan Data
Jika pengguna memilih untuk menampilkan semua data:
Program mencetak semua entri dalam dictionary.
python
elif pilihan == '4':
    for nama, details in data_mahasiswa.items():
        print(f"Nama: {nama}, NIM: {details['NIM']}")

8. Cari Data
Jika pengguna memilih untuk mencari data:
Program meminta nama yang dicari dan menampilkan informasi jika ditemukan.
python
elif pilihan == '5':
    nama = input("Nama yang dicari: ")
    if nama in data_mahasiswa:
        print(f"Data ditemukan: {data_mahasiswa[nama]}")

9. Keluar
Jika pengguna memilih untuk keluar, program akan berhenti.
Dengan mengikuti struktur di atas, Anda dapat membuat program sederhana menggunakan dictionary yang memungkinkan pengguna untuk mengelola data dengan mudah melalui menu interaktif.



KODE PROGRAM

![Screenshot 2024-11-28 230312](https://github.com/user-attachments/assets/7a2adfa1-4732-412e-a7f3-73ab6fc377cf)







FLOWCHART
text
[Start]
   |
   v
[Display Menu]
   |
   v
[Input Choice]
   |
   +------------------+
   |                  |
   v                  v
[Tambah Data]    [Ubah Data]
   |                  |
   v                  v
[Input Data]     [Input Name to Change]
   |                  |
   v                  v
[Save Data]     [Update Data]
   |                  |
   v                  v
[Back to Menu]    [Back to Menu]
   |
   +------------------+
   |
   v
[Hapus Data]
   |
   v
[Input Name to Delete]
   |
   v
[Delete Data]
   |
   v
[Back to Menu]
   |
   +------------------+
   |
   v
[Tampilkan Data]
   |
   v
[Display All Data]
   |
   v
[Back to Menu]
   |
   +------------------+
   |
   v
[Cari Data]
   |
   v
[Input Name to Search]
   |
   v
[Display Found Data]
   |
   v
[Back to Menu]
   |
   +------------------+
   |
   v
[End]






HASIL PROGRAM

![Screenshot 2024-11-28 230347](https://github.com/user-attachments/assets/bbcb1b0c-c161-4fb5-a91b-3fd6c248f4d3)


