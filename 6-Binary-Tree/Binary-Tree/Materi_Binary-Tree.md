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
Tree yang memiliki children node dengan jumlah maksimal dua buah di mana node-node di dalam tree tidak memiliki urutan antara satu dengan yang lain. Children node dibedakan menjadi left child dan right child. Jika node tidak memiliki anak atau child maka node itu disebut daun (leaf)

![Structue of Binary Tree](Structure-of-binary_tree.png)

## Kenapa Menggunakan Binary Tree
- Memiliki sintaks *insertion*, *deletion*, dan *searching* yang lebih simple daripada *tree*.
- Menjadi landasan untuk algoritma **Binary Search Tree**, **AVL Tree** dan, **RB Tree**

## Kekurangan
- Tidak memperdulikan urutan
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
class Node {
    int value;
    Node left, right;

    Node(int value) {
        this.value = value;
        left = right = null;
    }
}

class BinaryTree {
    Node root;

    // Tambahkan node secara level-order
    void add(int value) {
        Node newNode = new Node(value);

        if (root == null) {
            root = newNode;
            return;
        }

        java.util.Queue<Node> queue = new java.util.LinkedList<>();
        queue.add(root);

        while (!queue.isEmpty()) {
            Node current = queue.poll();

            if (current.left == null) {
                current.left = newNode;
                return;
            } else {
                queue.add(current.left);
            }

            if (current.right == null) {
                current.right = newNode;
                return;
            } else {
                queue.add(current.right);
            }
        }
    }

    // Traversal InOrder
    void inOrder(Node root) {
        if (root != null) {
            inOrder(root.left);
            System.out.print(root.value + " ");
            inOrder(root.right);
        }
    }

    // Traversal PreOrder
    void preOrder(Node root) {
        if (root != null) {
            System.out.print(root.value + " ");
            preOrder(root.left);
            preOrder(root.right);
        }
    }

    // Traversal PostOrder
    void postOrder(Node root) {
        if (root != null) {
            postOrder(root.left);
            postOrder(root.right);
            System.out.print(root.value + " ");
        }
    }

    // Search value dalam tree (BFS)
    boolean search(int target) {
        if (root == null) return false;

        java.util.Queue<Node> queue = new java.util.LinkedList<>();
        queue.add(root);

        while (!queue.isEmpty()) {
            Node current = queue.poll();

            if (current.value == target) return true;

            if (current.left != null) queue.add(current.left);
            if (current.right != null) queue.add(current.right);
        }
        
        return false;
    }

    // Delete node dengan value tertentu
    void delete(int value) {
        if (root == null) return;

        if (root.left == null && root.right == null) {
            if (root.value == value) root = null;
            return;
        }

        java.util.Queue<Node> queue = new java.util.LinkedList<>();
        queue.add(root);

        Node targetNode = null;
        Node current = null;

        while (!queue.isEmpty()) {
            current = queue.poll();

            if (current.value == value) targetNode = current;

            if (current.left != null) queue.add(current.left);
            if (current.right != null) queue.add(current.right);
        }

        if (targetNode != null) {
            int deepestValue = current.value;
            deleteDeepest(current);
            targetNode.value = deepestValue;
        }
    }

    // Menghapus node terdalam
    void deleteDeepest(Node delNode) {
        java.util.Queue<Node> queue = new java.util.LinkedList<>();
        queue.add(root);

        while (!queue.isEmpty()) {
            Node current = queue.poll();

            if (current.left != null) {
                if (current.left == delNode) {
                    current.left = null;
                    return;
                } else {
                    queue.add(current.left);
                }
            }

            if (current.right != null) {
                if (current.right == delNode) {
                    current.right = null;
                    return;
                } else {
                    queue.add(current.right);
                }
            }
        }
    }

    void printInOrder() {
        System.out.print("InOrder Traversal: ");
        inOrder(root);
        System.out.println();
    }

    void printPreOrder() {
        System.out.print("PreOrder Traversal: ");
        preOrder(root);
        System.out.println();
    }

    void printPostOrder() {
        System.out.print("PostOrder Traversal: ");
        postOrder(root);
        System.out.println();
    }

    boolean contains(int value) {
        return search(value);
    }
}

// Main Program
public class BabBinaryTree {
    public static void main(String[] args) {
        BinaryTree tree = new BinaryTree();

        // Tambah node
        tree.add(7);  // root
        tree.add(4);  // left of root
        tree.add(9);  // right of root
        tree.add(1);  // left of 4
        tree.add(5);  // right of 4

        // Tampilkan traversal
        tree.printInOrder();
        tree.printPreOrder();
        tree.printPostOrder();

        // Cari data
        System.out.println("Cari 5? " + tree.contains(5));
        System.out.println("Cari 10? " + tree.contains(10));

        // Hapus node
        System.out.println("Hapus 4...");
        tree.delete(4);
        tree.printInOrder();
    }
}
```

