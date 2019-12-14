# LabPratikum5.02
- ![](https://github.com/aditya-sultan/LabPratikum5.02/blob/master/latuhan5.PNG)

print("==================================================================")
print("|                    PROGRAM INPUT NILAI MAHASISWA               |")
print("==================================================================")

nilai = []
perulangan = True

while perulangan:
   nama = input("Masukkan Nama: ")
   nim = input("Masukkan NIM: ")
   nilaiTugas = int(input("Masukkan Nilai Tugas: "))
   nilaiUts = int(input("Masukkan Nilai UTS: "))
   nilaiUas = int(input("Masukkan Nilai UAS    : "))
   nilaiAkhir = (nilaiTugas * 30/100) + (nilaiUts * 35/100) + (nilaiUas * 35/100)

    nilai.append([nama, nim, nilaiTugas, nilaiUts, nilaiUas, int(nilaiAkhir)])
    if (input("Tambah data (y/t)? ") == 't'):
        perulangan = False

print("\n                    DAFTAR NILAI MAHASISWA                      ")
print("==================================================================")
print("| No | Nama | NIM | Tugas | UTS | UAS | Akhir |")
print("==================================================================")

i = 0
for item in nilai:
   i += 1
   print("| {no:2d} | {nama:12s} | {nim:9s} | {nilaiTugas:5d} | {nilaiUts:5d} | {nilaiUas:5d} | {nilaiAkhir:6.2f} |"
         .format(no=i, nama=item[0], nim=item[1], nilaiTugas=item[2], nilaiUts=item[3], nilaiUas=item[4], nilaiAkhir=item[5]))
print("==================================================================")

# hasil run

![](https://github.com/aditya-sultan/LabPratikum5.02/blob/master/Capture.PNG)

==================================================================
|                    PROGRAM INPUT NILAI MAHASISWA               |
==================================================================
- Masukkan Nama: Zahra
- Masukkan NIM: 311242
- Masukkan Nilai Tugas: 32
- Masukkan Nilai UTS: 34
- Masukkan Nilai UAS    : 33
- Tambah data (y/t)? y
- Masukkan Nama: Robi
- Masukkan NIM: 212532
- Masukkan Nilai Tugas: 32
- Masukkan Nilai UTS: 23
- Masukkan Nilai UAS    : 34
- Tambah data (y/t)? y
- Masukkan Nama: Ferdi
- Masukkan NIM: 32135
- Masukkan Nilai Tugas: 33
- Masukkan Nilai UTS: 32
- Masukkan Nilai UAS    : 34
- Tambah data (y/t)? t

-                    DAFTAR NILAI MAHASISWA                      
- ==================================================================
- | No | Nama | NIM | Tugas | UTS | UAS | Akhir |
- ==================================================================
- |  1 | Zahra        | 311242    |    32 |    34 |    33 |  33.00 |
- |  2 | Robi         | 212532    |    32 |    23 |    34 |  29.00 |
- |  3 | Ferdi        | 32135     |    33 |    32 |    34 |  33.00 |
- ==================================================================

- Process finished with exit code 0
