# Game Ular Tangga 2D/3D

Ini adalah implementasi sederhana dari permainan papan klasik Ular Tangga yang dibuat menggunakan C++ dengan library OpenGL/GLUT. Permainan ini memiliki perspektif 2D dan 3D, mode dua pemain, dan kontrol yang interaktif.

## 👥 Anggota Tim

Proyek ini dikembangkan oleh:

| Nama                    | NPM            |
| ----------------------- | -------------- |
| Moch Sigit Aringga      | 230411100104   |
| Harits Putra Junaidi    | 230411100003   |
| Danendra Mahardhika     | 230411100086   |
| Achmad Lutfi Madhani    | 230411100059   |
| Abdullah Sahl           | 230411100090   |
| Dicky Prasetyo          | 230411100166   |

## 📜 Deskripsi

Program ini adalah permainan Ular Tangga yang dapat dimainkan sepenuhnya. Pemain bergiliran melempar dadu dengan menekan tombol spasi. Bidak pemain akan bergerak sesuai dengan angka dadu yang muncul. Jika pemain mendarat di bagian bawah tangga, bidak akan naik ke atas. Sebaliknya, jika mendarat di kepala ular, bidak akan turun ke ekornya. Pemain pertama yang mencapai kotak terakhir (84) adalah pemenangnya.

Fitur unik dari proyek ini adalah kemampuan untuk beralih antara tampilan 2D tradisional (dari atas) dan perspektif 3D yang lebih imersif.

## ✨ Fitur

* **Gameplay Ular Tangga Klasik**: Semua aturan dasar yang sudah Anda kenal.
* **Mode Dua Pemain**: Bermain bersama teman.
    * **Pemain 1**: Segitiga Hijau
    * **Pemain 2**: Kotak Merah
* **Tampilan 2D dan 3D**: Beralih antara tampilan 2D dan 3D kapan saja.
* **Kontrol Interaktif**: Perintah keyboard sederhana untuk bermain dan mengontrol tampilan.
* **Kamera Dinamis**: Dalam mode 3D, Anda dapat memutar papan permainan untuk melihatnya dari berbagai sudut.
* **Objek Observer**: Mengontrol objek kerucut "pengamat" terpisah di papan.

## 🎮 Cara Bermain & Kontrol

### Kontrol Permainan

| Tombol      | Aksi                                  |
| ----------- | ------------------------------------- |
| **Spasi** | Lempar dadu dan gerakkan bidak Anda.  |
| **R** | Reset permainan ke kondisi awal.      |
| **V** | Beralih antara tampilan 2D dan 3D.    |

### Kontrol Kamera & Observer (Mode 3D)

| Tombol | Aksi                             |
| ------ | -------------------------------- |
| **I** | Putar tampilan papan ke atas.    |
| **K** | Putar tampilan papan ke bawah.   |
| **J** | Putar tampilan papan ke kiri.    |
| **L** | Putar tampilan papan ke kanan.   |
| **W** | Gerakkan observer ke atas.       |
| **S** | Gerakkan observer ke bawah.      |
| **A** | Gerakkan observer ke kiri.       |
| **D** | Gerakkan observer ke kanan.      |

## 🛠️ Instalasi dan Eksekusi

### Prasyarat

* Compiler C++ (seperti g++ atau MinGW)
* Library OpenGL Utility Toolkit (GLUT) sudah terinstal dan terhubung dengan benar.

### Kompilasi

Anda dapat mengompilasi file `main.cpp` menggunakan compiler C++. Pastikan untuk menautkan (link) library OpenGL dan GLUT yang diperlukan.

**Contoh menggunakan g++:**

```bash
g++ main.cpp -o UlarTangga -lglut -lglu32 -lopengl32
