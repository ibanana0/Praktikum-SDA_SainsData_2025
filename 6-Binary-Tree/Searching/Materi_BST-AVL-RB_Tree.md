# Searching
Metode *searching* adalah metode yang digunakan untuk mencari suatu elemen di dalam kumpulan elemen. 

Metode *searching* yang paling cepat berada pada Array di mana kompleksitas waktunya O(1).

Pada konsep *tree*, metode *searching* secara umum memiliki kompleksitas waktu O(n), karena *tree* menerapkan konsep List dan Queue.

Maka dari itu, dibuatlah konsep *binary search tree* di mana proses *searching* dapat dilakukan dengan *average case* O(log n). Namun, *binary tree* masih memiliki *worst case* O(n) karena masih ada kemungkinan bahwa *binary tree* tersebut tidak seimbang.

Maka dari itu, dibuatlah konsep *tree* yang mampu melakukan *self-balancing* seperti AVL Tree dan Red Black Tree. Hal ini memastikan proses *searching* memiliki kompleksitas waktu O(log n).

## Algoritma
```java
Node search(Node root, int key) {
        if (root == null || root.key == key)    // Memeriksa apakah root bernilai null atau sudah ditemukan node yang dicari
            return root;    // Mengembalikan nilai node

        if (key < root.key) // Jika elemen yang dicari lebih kecil, maka akan melakukan searching ke subtree kiri
            return search(root.left, key);
        else    // Jika elemen yang dicari lebih besar, maka akan melakukan searching ke subtree kanan
            return search(root.right, key);
    }

```
