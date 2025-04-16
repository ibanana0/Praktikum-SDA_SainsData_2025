# Red Black Tree
- [Red Black Tree](#red-black-tree)
  - [Pengertian](#pengertian)
  - [Aturan](#aturan)
  - [Algoritma](#algoritma)
    - [Insertion](#insertion)
    - [Deletion](#deletion)
  - [Kelebihan](#kelebihan)
  - [Kekurangan](#kekurangan)
  - [Contoh](#contoh)
  - [Implementasi](#implementasi)

## Pengertian
Red Black Tree adalah Binary Tree yang dapat melakukan *self balancing* dengan meninjau jumlah *black node* untuk setiap *subtree* yaitu harus sama. Hal ini menyebabkan Red Black Tree memiliki panjang *subtree* maksimal yaitu dua kali panjang *subtree* terpendek
## Aturan
- Setiap *node* berwarna **merah** atau **hitam**
- ***Root*** dan ***null leaf*** selalu berwarna **hitam**
- *Node* merah tidak boleh punya *child node* merah (**tidak ada dua merah berurutan**)
- Setiap *path* dari *root* ke *leaf* mengandung **jumlah *node* hitam yang sama** (*black height*)

## Algoritma
### Insertion
1. Memasukkan *node* baru dan memberi warna merah
2. Mencari posisi *node* baru:
   - Jika ditemukan warna ***parent* hitam**, ***insertion* berhasil**
   - Jika ditemukan warna ***parent* merah**, terjadi pelanggaran aturan (**aturan 3**), maka perlu melakukan **pemeriksaan *uncle node***:
     - **Jika *uncle* merah, maka melakukan ***passing blackness***** → mengubah warna *parent* dan *uncle* menjadi hitam untuk diteruskan ke atas (hingga warna *root* menjadi merah), lalu:
       - **Melakukan pemeriksaan *parent* dan *child node***. Jika ditemukan warna merah-merah, perlu melakukan pemeriksaan *uncle* lagi dari awal
       - **Mengubah kembali warna *root* menjadi hitam**
     - **Jika *uncle null* atau hitam, maka melakukan rotasi**, lalu menyesuaikan warna *parent* dengan *uncle* (berwarna hitam)

### Deletion
1. **Mencari posisi *node*** yang akan dihapus
2. **Mencari *node* pengganti** dengan mencari *child* *node* terbesar yang berada di *subtree* sebelah kiri
   - **Jika *node* pengganti berwarna merah, proses deletion dapat dilakukan tanpa masalah**
   - **Jika *node* pengganti berwarna hitam, dilakukan pemeriksaan *sibling node***:
     - Jika *sibling node* berwarna merah, dilakukan rotasi dan ubah warna lalu hapus *node* yang akan dihapus 
     - Jika *sibling node* berwarna hitam dan anak-anaknya berwarna hitam, ubah warna *sibling node* menjadi warna merah lalu hapus *node* yang akan dihapus
     - Jika *sibling node* berwarna hitam dan ada salah satu anak nya yang berwarna merah, lakukan rotasi dan ubah warna lalu hapus *node* yang akan dihapus
## Kelebihan
- Mampu melakukan *self-balancing*
- Kompleksitas waktu untuk *insertion, searching,* dan *deletion* yaitu **O(log n)**
- Kecepatan *insertion* dan *deletion* lebih cepat daripada AVL Tree
- Cocok untuk menyimpan data yang berubah secara dinamis
## Kekurangan
- Struktur *tree* tidak terlalu seimbang dengan maksimal toleransi perbedaan ketinggian antara *subtree*-nya yaitu dua kali dari ketinggian *subtree* terpendek
- Sehingga proses *searching* akan menjadi lebih lambat daripada AVL Tree
## Contoh
## Implementasi
```java
kodingan
```
