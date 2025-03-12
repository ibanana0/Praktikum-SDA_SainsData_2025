# 1 - Introduction

- [1 - Introduction](#1---introduction)
  - [1.1 - Tujuan Pembelajaran](#11---tujuan-pembelajaran)
  - [1.2 - Kontrak](#12---kontrak)
    - [1.2.1 - Materi](#121---materi)
    - [1.2.2 - Penugasan](#122---penugasan)
  - [1.3 - Instalasi](#13---instalasi)
    - [1.3.1 - IDE](#131---ide)
    - [1.3.2 - Java](#132---java)
      - [1.3.2.1 - VS Code (Package)](#1321---vs-code-package)
      - [1.3.2.2 - Manual](#1322---manual)
    - [1.3.3 - Extension (Opsional)](#133---extension-opsional)
  - [1.4 - Referensi](#14---referensi)




## 1.1 - Tujuan Pembelajaran
Setelah menyelesaikan tutorial ini, mahasiswa diharapkan untuk dapat:

- Mengetahui materi apa saja yang akan dipelajari selama praktikum Struktur dan Algoritma Data
- Mengetahui cara instalasi IDE dan extension untuk keperluan praktikum

## 1.2 - Kontrak
### 1.2.1 - Materi
Materi yang akan diajarkan selama praktikum meliputi:

| Pertemuan | Materi |
| --------- | ------- |
| Pertemuan 1 | [Introduction](0-Introduction.md) |
| Pertemuan 2 | [1-Perkenalan](1-Perkenalan) |
| Pertemuan 3 | [lorem](link) |
| Pertemuan 4 | [lorem](link) |
| Pertemuan 5 | [lorem](link) |
| Pertemuan 6 | [lorem](link) |
| Pertemuan 7 | [lorem](link) |
| Pertemuan 8 | [lorem](link) |
| Pertemuan 9 | [lorem](link) |
| Pertemuan 10 | [lorem](link) |
| Pertemuan 11 | [lorem](link) |
| Pertemuan 12 | [lorem](link) |
| Pertemuan 13 | [lorem](link) |
| Pertemuan 14 | [lorem](link) |

### 1.2.2 - Penilaian
- Pre-test 
Dilakukan di awal kelas
- Post-test (**Bobot: 10%**)
Dilakukan di akhir kelas
- Tugas (**Bobot: 50%**)
Pengurangan nilai 3/hari
- Responsi (**Bobot 40%**)
Dilakukan di waktu UTS dan UAS

## 1.3 - Instalasi
### 1.3.1 - IDE
*Integrated Development Environment* (IDE) adalah *software* yang membantu *programmer* dalam mengembangkan kode dari perangkat lunak yang sedang dikembangkan secara mudah dan efisien. IDE membantu *programmer* dalam mengedit, membangun, menguji, dan mengelola kode dari perangkat lunak yang sedang dikembangkan.

Adapun langkah-langkah untuk meng-*install* IDE yaitu:

**Langkah 1: Memilih IDE**

Ada beberapa IDE yang dapat digunakan selama praktikum SDA. Adapun *list* IDE tersebut yaitu:
- [**Visual Studio Code**](https://code.visualstudio.com/) (*digunakan Asdos*)
-  [**IntelliJ IDEA**](https://www.jetbrains.com/idea/) (*digunakan Asdos*)
-   [Sublime Text](https://www.sublimetext.com/)

**Note:**
- IntelliJ IDEA merupakan IDE dengan fitur yang lengkap dan berfokus pada pengembangan program menggunakan Java
- Anda tidak memerlukan proses instalasi tambahan untuk melakukan *set up Java development environment* ketika menggunakan IntelliJ
- IntelliJ IDEA memiliki fitur berbayar, Anda dapat menggunakan akun UNS untuk melakukan aktivasi Educational License
- IntelliJ IDEA membutuhkan ruang penyimpanan yang besar dalam proses peng-*install*-annya, Anda dapat menggunakan VS Code apabila Anda menginginkan alternatif IDE dengan kebutuhan penyimpanan yang lebih kecil

**Langkah 2: Meng-*Install* IDE**
1. Mengunjungi situs resmi IDE
2. Mengikuti petunjuk untuk meng-*install* *installer*
3. Menjalankan *installer* dan mengikuti instruksi yang ditampilkan pada *installer*

**Langkah 3: Menggunakan IDE**
1. Membuka IDE yang sudah ter-*install*
2. Memulai eksplorasi *interface* IDE untuk mengenali IDE yang digunakan

**Note:**
- Pastikan kamu memilih IDE yang sesuai dengan jenis proyek yang akan dikerjakan
- Eksplorasi fitur-fitur IDE seperti *extensions* dan *plugins*
- Kunjungi dokumentasi terkait IDE apabila menemukan masalah terkait IDE
### 1.3.2 - Java
#### 1.3.2.1 - VS Code (Package)
1. Meng-*install* Coding Pack for Java pada [link](https://code.visualstudio.com/docs/java/java-tutorial), pilih sesuai Operating System yang digunakan
2. Membuka *file* yang sudah di-*download*
3. Mengikuti instruksi yang ditampilkan
4. Memeriksa apakah Java sudah ter-*install* di cmd atau terminal menggunakan perintah:
   ```
   java --version
   ```
   Jika Java sudah ter-*install*, terminal akan menampilkan versi JDK
5. Memulai membuat program Java!

**Note:**
- Coding Pack for Java adalah program yang digunakan untuk membantu *programmer* melakukan *set up* secara otomatis di dalam *Java development environment* dalam bentuk *package*
- Adapun program yang akan di-*install* melalui Coding Pack for Java yaitu VS Code, Java Development Kit (JDK), dan beberapa *extensions* yang dapat membantu *programmer*
#### 1.3.2.2 - Manual
Apabila Anda ingin meng-*install* Java secara manual, berikut langkah-langkahnya:
1. Meng-*install* Java Development Kit (JDK) sesuai Operating System dan CPU Architecture laptop Anda pada tautan berikut:
   - [JDK 23 Windows (x64 Installer)](https://download.oracle.com/java/23/latest/jdk-23_windows-x64_bin.exe)
   - [JDK 23 macOS (ARM64 DMG Installer)](https://download.oracle.com/java/23/latest/jdk-23_macos-aarch64_bin.dmg)
   - [JDK 23 macOS (x64 DMG Installer)](https://download.oracle.com/java/23/latest/jdk-23_macos-x64_bin.dmg)
2.  Membuka *installer* yang sudah di-*download*
3.  Mengikuti instruksi dari *installer*
5.  Memeriksa apakah Java sudah ter-*install* atau belum melalui cmd atau terminal Anda dengan perintah:
   ```
   java --version
   ```
**Note:**
- Untuk proses instalasi dengan versi JDK dan Operating System yang lain, Anda dapat mencari informasi lebih lanjut pada tautan berikut:
  
  [JDK Download Link](https://www.oracle.com/id/java/technologies/downloads/)
### 1.3.3 - Extension (Opsional)
*Extentsion* yang diperlukan untuk membantu keperluan praktikum:
1. [Code Runner by Jun Han](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner) (Extension ID: formulahendry.code-runner)
2. [Language Support for Java by Red Hat](https://marketplace.visualstudio.com/items?itemName=redhat.java) (Extension ID: redhat.java)
3. [Debugger for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-debug) (Extension ID: vscjava.vscode-java-debug)
4. [Maven for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-maven) (Extension ID: vscjava.vscode-maven)
5. [Project Manager for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-dependency) (Extension ID: vscjava.vscode-java-dependency)
6. [Test Runner for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-test) (Extension ID: vscjava.vscode-java-test)
7. [IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode) (Extension ID: VisualStudioExptTeam.vscodeintellicode)
## 1.4 - Referensi
1. <https://www.oracle.com/id/java/>
2. <https://code.visualstudio.com/docs/java/java-tutorial>
3. <https://code.visualstudio.com/docs/java/extensions>
