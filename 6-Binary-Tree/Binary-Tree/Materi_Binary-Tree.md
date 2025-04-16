# Binary Tree

- [Binary Tree](#binary-tree)
  - [Overview](#overview)
    - [Konsep Tree](#konsep-tree)
    - [Perbedaan Tree dan Binary Tree](#perbedaan-tree-dan-binary-tree)
  - [Pengertian](#pengertian)
  - [Kenapa Menggunakan Binary Tree](#kenapa-menggunakan-binary-tree)
  - [Kekurangan](#kekurangan)
  - [Solusi dari Kekurangan](#solusi-dari-kekurangan)
  - [Contoh](#contoh)
  - [Implementasi](#implementasi)


## Overview
### Konsep Tree
![Konsep Tree](Tree_BST_AVL_RB.png)
<hr>

### Perbedaan Tree dan Binary Tree
![Tree vs Binary Tree](Tree-vs-Binary.png)
## Pengertian
Tree yang memiliki children node dengan jumlah maksimal dua buah di mana node-node di dalam tree tidak memiliki urutan antara satu dengan yang lain. Children node dibedakan menjadi left child dan right child.

![Structue of Binary Tree](Structure-of-binary_tree.png)

## Kenapa Menggunakan Binary Tree
- Memiliki sintaks *insertion*, *deletion*, dan *searching* yang lebih simple daripada *tree*.
- Menjadi landasan untuk algoritma **Binary Search Tree**, **AVL Tree** dan, **RB Tree**

## Kekurangan
- Belum bisa melakukan *sorting*
- Kecepatan operasi *insert*, *delete*, dan pencarian atau pengaksesan elemen adalah O(n), karena untuk menemukan posisi elemen yang dicari diperlukan iterasi dengan menelusuri semua *node* elemen di dalam *tree*

## Solusi dari Kekurangan
- Dibuatlah konsep Binary Search Tree

## Contoh
- Digunakan pada teori bahasa automata (bahasa komputer) untuk membentuk *parse tree* (grammar) dan *expression tree* (aritmatika)
- Digunakan untuk pembuatan program yang memerlukan penyimpanan data secara hierarki tapi tidak terikat dengan kemampuan pengurutan
- Digunakan pada konsep algoritma **Binary Search Tree**, **AVL Tree** dan, **RB Tree**

## Implementasi
```java
coding
```

