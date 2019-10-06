# Tugas-5-Pemrograman-Jaringan  
### Javiar Fasyah - 1301164477  
### Fahrur Rozi Syarbini - 1301164213  
### Hilmi Triandi N - 1301164286  
  
**Jawaban soal No. 1:**  
![1.png](/screenshot/1.png)  
Struct Person diinisialisasi pada variabel bytes dengan atribut nama depan (Firstname) “John” dan nama belakang (Lastname) “Dow”. Kemudian, bytes diserialisasikan kedalam bentuk JSON dan dicetak menghasilkan keluaran struct Person dalam bentuk JSON ({“firstname”:”John”,”lastname”:”Dow”}).  
  
**Jawaban soal No. 2:**  
![2.png](/screenshot/2.png)  
Struct Person dalam bentuk JSON di-assign ke variabel in, yang kemudian variabel in menjadi nilai untuk variabel bytes dalam tipe data []byte. Kemudian, variabel bytes di decode dari bentuk JSON menjadi bentuk struct Person dan ditampung pada variabel p. Sehinga, keluaran yang dihasilkan dari mencetak variabel p adalah {Firstname:John Lastname:Dow}.  
  
**Jawaban soal No. 3:**  
sisi client:  
![3_client.png](/screenshot/3/client.png)  
sisi server:  
![3_server.png](/screenshot/3/server.png)  
  
Perbedaan antara protocol buffer dengan flatbuffer adalah pada representasi in-memory dan wire format-nya. Protocol buffer memisahkan representasi in-memory dengan wire protocolnya (butuh parsing dan serialsiasi), sementara flatbuffer tidak memisahkan keduanya (serialisasi terjadi disaat pembuatan objek flatbuffer pada representasi in-memory). Hal yang sama terjadi saat objek protocol buffer ingin dikembalikan ke asalnya, terjadi parsing dan deserialisasi lagi. Namun pada flatbuffer, yang dtiampilkan adalah pointer kepada objek flatbuffer yang ada.
