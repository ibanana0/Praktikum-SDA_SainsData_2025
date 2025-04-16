# Binary Search Tree
- [Binary Search Tree](#binary-search-tree)
  - [Pengertian](#pengertian)
  - [Kelebihan](#kelebihan)
  - [Kekurangan](#kekurangan)
  - [Solusi dari Kekurangan](#solusi-dari-kekurangan)
  - [Contoh](#contoh)
  - [Implementasi](#implementasi)

![Binary Search Tree](Binary-Search-Tree.png)
## Pengertian
Binary Search Tree merupakan konsep Binary Tree yang memiliki aturan bahwa left child memiliki value yang lebih kecil daripada parent node-nya sedangkan right child memiliki value yang lebih besar daripada parent node-nya. Hal ini menyebabkan tree memiliki struktur data yang berurutan.

![Struktur dari Binary Search Tree](Structure-of-Binary_Search_Tree.png)
## Kelebihan
- Mampu melakukan *sorting*
- Karena memiliki kemampuan *sorting*, proses operasi *insertion, deletion*, dan *searching* bisa dilakukan dengan lebih cepat
- Menjadi landasan untuk konsep algoritma **AVL Tree** dan **Red Black Tree**
## Kekurangan
![Imbalance Tree dan Balanced Tree](Imbalanced-Balanced_Tree.png)
- Tidak memiliki aturan yang mengikat terkait keseimbangan *tree* sehingga ada kemungkinan terbentuk *imbalanced tree* (*tree* yang tidak seimbang antara subtree kiri dan kanannya)
- *Imbalanced tree* cenderung lebih lambat daripada *balanced tree* untuk proses operasi *insertion*, *deletion*, dan *searching* karena ada kemungkinan langkah/jarak yang ditempuh lebih banyak daripada *balanced tree*
- *Imbalanced tree* memiliki kompleksitas waktu O(n)
## Solusi dari Kekurangan
- Dibuatlah konsep *self balancing tree* seperti **AVL Tree** dan **Red Black Tree** sehingga proses operasi memiliki kompleksitas waktu O(log n)
## Contoh
- Algoritma sorting
- Decision tree
- Program pencarian kata di dalam kamus
## Implementasi
```java
kodingan
```
