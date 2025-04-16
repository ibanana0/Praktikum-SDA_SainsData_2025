# AVL Tree
## Pengertian
AVL Tree adalah Binary Tree yang dapat melakukan *self balancing* dengan meninjau selisih *height* subtree yaitu **harus tidak lebih dari 1**. Proses *self balancing* dilakukan dengan melakukan *rotating*.

## Aturan
```
balance factor = height of left subtree - height of right subtree
bf = hl - hr = {-1, 0, 1}
```

## Algoritma
>**Note:** perhitungan *height* dan *balance factor (bf)* pada *node* dilakukan dari *node* paling bawah

>**Note:** *rotation* dilakukan di antara *node* yang memiliki tanda *bf* yang sama dan *node* yang mengarah pada *subtree* tempat *node* baru diletakkan

### Insertion
1. **Mencari lokasi *node* baru** dengan membandingkan *node* baru dengan *root node*, lalu ke *children node* hingga mencapai pada lokasi yang sesuai
2. **Menganalisis balance factor**:
   - Jika ditemukan *balance factor* yang bernilai {2, -2}, maka dilakukan **rotasi**
3. **Mengulangi langkah 2**

### Deletion
1. **Mencari lokasi *node* yang akan dihapus** dengan membandingkan *node* yang dicari dengan *node-node* di dalam tree
2. **Mencari *node successor* (*node* pewaris)** yaitu *node* dengan nilai terkecil pada *subtree* sebelah kanan *node* yang akan dihapus
3. **Menghapus node** yang akan dihapus dan **mengganti *node* yang dihapus dengan *node successor***
4. **Melakukan *re-balancing***:
   - Menganalisis *balance factor*
   - Jika ditemukan *balance factor* yang bernilai {2,-2} maka dilakukan **rotasi**
   - Mengulangi proses menganalisis *balance factor* hingga semua *balance factor* pada *tree* memenuhi aturan

## Kelebihan
- Mampu melakukan *self-balancing*
- Kompleksitas waktu untuk *insertion, searching,* dan *deletion* yaitu **O(log n)**
- Kecepatan *searching* lebih cepat daripada Red Black Tree
## Kekurangan
- Melakukan *self-balancing* setiap kali melakukan proses operasi *insertion* dan *deletion*
- Sehingga proses *insertion* dan *deletion* lebih lambat daripada Red Black Tree
## Contoh

## Implementasi
```java
kodingan
```
