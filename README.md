# praktikum4
Modul 2

Latihan 1: Membuat program menentukan nilai akhir

 nama = input("Masukkan nama:")
 uts = input("Masukkan nilai UTS:")
 uas = input("Masukkan nilai UAS:")
 tugas = input("Masukkan nilai Tugas:")

 akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
 keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
 if akhir > 80:
    huruf = "A"
  elif akhir > 70:
    huruf = "B"
  elif akhir > 50:
    huruf = "C"
  elif akhir > 40:
    huruf = "D"
  else:
    huruf = "E"

print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan)
![lab2 py latihan1](https://user-images.githubusercontent.com/116045324/200495247-9e9bbea5-e16e-4fb3-ab87-1fb7b33b797b.PNG)
hasil run
![hasilrunlab2 py latihan1](https://user-images.githubusercontent.com/116045324/200495319-8cc37a40-ceb9-4540-87f6-eeb465d04555.PNG)


Latihan 2: Membuat program menampilkan status gaji karyawan.

gaji = int(input("Masukkan gaji:"))
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]
if gaji > 3000000:
    print ("Gaji sudah diatas UMR")
    if berkeluarga:
      print ("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
      print ("Tidak perlu ikutan asuransi")
    if punya_rumah:
      print ("wajib bayar pajak rumah")
    else:
      print ("tidak wajib bayar pajak rumah")
else:
  print ("Gaji belum UMR")
![lab2 py latihan2](https://user-images.githubusercontent.com/116045324/200495382-b1d8df24-eb04-44e1-98f8-3b96f9d05478.PNG)
hasil run
![hasilrunlab2 py latihan2](https://user-images.githubusercontent.com/116045324/200495432-3726fe78-6719-43b8-8be0-f7aa288b831a.PNG)


Latihan 3: penggunaan kondisi OR program membandingkan 3 input bilangan, apabila penjumlahan 2 bilangan hasilnya sama dengan bilangan lainnya, maka cetak pernyataan “BENAR”

a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
if a+b == c or b+c == a or c+a == b:
  print("BENAR")
else:
  print("SALAH")
![lab2 py latihan3](https://user-images.githubusercontent.com/116045324/200495499-2bc79ad3-8265-49bd-a011-8a8aecf0dde6.PNG)
hasil run
![hasilrunlab2 py latihan3](https://user-images.githubusercontent.com/116045324/200495539-7f602bc5-8629-4f6e-94ce-b10dd9a0a3f7.PNG)


Praktikum 2 Buat program sederhana dengan input tiga buah bilangan, dari ketiga bilangan tersebut tampilkan bilangan terbesarnya. Gunakan statement if.

data =[]
for i in range (3):
    x=int(input("masukkan bilangan :"))
    data.append(x)
print ("data sebelum diurutkan :", data)
list.sort(data)
print ("data setelah diurutkan :", data)
![praktikum2 py](https://user-images.githubusercontent.com/116045324/200495635-c823955a-24b9-4535-8035-1b3a86a74664.PNG)
hasil run
![hasilrunpraktikum2 py](https://user-images.githubusercontent.com/116045324/200495711-1a0882e1-93c4-4699-8a99-75b500a98694.PNG)


flowchart

Modul3 Latihan 1: latihan1.py

Tampilkan n bilangan acak yang lebih kecil dari 0.5.

nilai n diisi pada saat runtime

anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya

gunakan fungsi random() yang dapat diimport terlebih dahulu

print ("masukan nilai N: 5 ") import random jumlah=5 a=0

for x in range (jumlah): i = random.uniform (.0,.5) a+=1 print('data ke :',a, '==>', i)

print("selesai")

![labpy3latihan1 py](https://user-images.githubusercontent.com/116045324/200495795-915b8e03-cf9c-4898-b699-7ee878d18aa5.PNG)
hasil run
![hasilrunlabpy3latihan1 py](https://user-images.githubusercontent.com/116045324/200495852-abf18161-eedb-465f-9a79-9a0fd199cafe.PNG)


Latihan 2: latihan2.py Buat program untuk menampilkan bilangan terbesar dari n buah data yang diinputkan. Masukkan angka 0 untuk berhenti.

print("menampilkan bilangan terbesar dari n buah data")
max=0
while True:
    a=int(input("masukkan bilangan :"))
    if max < a :
       max = a
    if a==0 :
        break
print("bilangan terbesar adalah= ", max)
![labpy3latihan2](https://user-images.githubusercontent.com/116045324/200495947-88d10b58-88fa-4490-8cd3-24e341765327.PNG)
hasil run
![hasilrunlabpy3latihan2](https://user-images.githubusercontent.com/116045324/200496018-856f72f0-8f28-4b6f-84d8-69ad48f27c42.PNG)


Praktikum 3

Buat program sederhana dengan perulangan: program1.py Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan modal awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada bulan ketiga baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5, pendapatan meningkat 5%, selanjutnya pada bulan ke 8 mengalami penurunan keuntungan sebesar 2%, sehingga laba menjadi 3%. Hitung total keuntungan selama 8 bulan berjalan usahanya.

a=1000000000
for x in range (1,9):
    if(x>=1 and x<=2):
        b=a*0
        print("laba bulan ke-",x, ":", b)
    if(x>=3 and x<=4):
        c=a*0.1
        print("laba bulan ke-",x, ":", c)
    if(x>=5 and x<=7):
        d=a*0.5
        print("laba bulan ke-",x, ":", d)
    if(x==8):
        e=a*0.2
        print("laba bulan ke-",x, ":", e)
total=b+b+c+c+d+d+d+e
print("\ntotal :", total)
![praktikum3 py](https://user-images.githubusercontent.com/116045324/200496175-cf190b1c-88f9-4649-b659-112e589b3c5b.PNG)
hasil run
![hasilrunpraktikum3 py](https://user-images.githubusercontent.com/116045324/200496231-b5a2b90b-a921-4f39-838e-5c6bc8299932.PNG)
