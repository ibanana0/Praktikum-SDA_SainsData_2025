# Rotation
Algoritma rotasi digunakan pada AVL Tree dan Red Black Tree. Pada kedua *tree*, algoritma rotasi adalah sama. Namun terdapat perbedaan antara kapan harus terjadi rotasi.

## Perbedaan Kapan Waktu Rotasi
### AVL Tree
- Ketika terdapat selisih ketinggian yang **bernilai {-2, 2}**
- Dilakukan pada *node* yang **memiliki tanda *balance factor* yang sama** (negatif-negatif, positi-positif) 
### Red Black Tree
- Ketika pada proses pemeriksaan *uncle node* ditemukan *uncle node* bernilai **null** atau **berwarna hitam**
- Dilakukan pada **grandparent node dan parent node**

## Algoritma
### Basic
#### Left Rotation
![Left Rotation](Left_Rotation.png)
#### Left-Right Rotation
![LR Rotation](LR.png)
#### Right Rotation
![Right Rotation](Right_Rotation.png)
#### Right-Left Rotation
![RL Rotation](RL.png)

### Special Case
#### Left-Left Rotation
![LL Special Rotation](LL_Special.png)
#### Right-Right Rotation
![RR Special Rotation](RR_Special.png)
#### Right-Left Special Rotation
![LR Special Rotation](RL_Special.png)

## Referensi
[Youtube](https://www.youtube.com/watch?v=jDM6_TnYIqE&t=1892s)
