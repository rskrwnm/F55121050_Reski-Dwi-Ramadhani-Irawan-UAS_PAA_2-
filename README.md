# F55121050_Reski-Dwi-Ramadhani-Irawan-UAS_PAA_2-
<h1>Analisis Algorithm untuk mengevaluasi Bubble sort</h1>
Dalam analisis algoritma Bubble Sort terdapat tiga kasus yang berbeda yaitu, kasus terburuk, kasus terbaik, dan kasus rata-rata. Berikut analasis untuk tiap kasus yang ada: <br>
a. Worst case: <br>
Kasus terburuk terjadi ketika elemen-elemen dalam array terurut secara terbalik, dan Bubble Sort harus melakukan perbandingan dan pertukaran pada setiap pasangan elemen. Dalam hal ini, kompleksitas waktu Bubble Sort adalah O(n^2), di mana 'n' adalah jumlah elemen dalam array. Bubble Sort akan melakukan perbandingan sebanyak (n-1) + (n-2) + ... + 1 = n(n-1)/2 kali. Untuk setiap perbandingan, diperlukan pertukaran elemen, sehingga total pertukaran dalam kasus terburuk juga adalah n(n-1)/2. <br>
b. Best case: <br>
Kasus terbaik terjadi ketika array sudah terurut dengan benar. Dalam hal ini, Bubble Sort akan melakukan perbandingan pada setiap pasangan elemen, tetapi tidak perlu melakukan pertukaran karena array sudah terurut dengan benar. Kompleksitas waktu Bubble Sort dalam kasus terbaik adalah O(n), karena setiap elemen hanya akan dibandingkan sekali. <br>
c. Average case: <br>
Kasus rata-rata dalam Bubble Sort sulit ditentukan secara pasti, karena itu melibatkan distribusi yang acak dari elemen-elemen dalam array. Namun, secara umum, kompleksitas waktu rata-rata Bubble Sort adalah O(n^2). Meskipun ada kemungkinan mengurangi jumlah perbandingan dengan menggunakan teknik seperti "short bubble" (menghentikan iterasi jika tidak ada pertukaran dalam satu putaran), tetapi dalam analisis rata-rata, kami menganggap kasus terburuk di mana semua perbandingan dan pertukaran dilakukan. <br>
<h1>Analisis Algorithm untuk mengevaluasi Insertion sort</h1>
Dalam analisis algoritma Insertion sort terdapat tiga kasus yang berbeda yaitu, kasus terburuk, kasus terbaik, dan kasus rata-rata. Berikut analasis untuk tiap kasus yang ada: <br>
a.Worst case:
Worst case pada Bubble Sort terjadi ketika array tersebut sudah terurut secara terbalik atau dalam urutan yang terbalik dari yang diinginkan. Pada setiap iterasi, elemen dengan nilai lebih besar akan terus dipindahkan ke arah akhir array, memerlukan pertukaran pada setiap langkahnya. Dalam hal ini, Bubble Sort akan melakukan iterasi sebanyak (n-1) kali, di mana n merupakan jumlah elemen dalam array. Oleh karena itu, kompleksitas waktu worst case untuk Bubble Sort adalah O(n^2), dengan n adalah jumlah elemen dalam array.
b. Best case:
Best case pada Bubble Sort terjadi ketika array tersebut sudah terurut secara ascending atau dalam urutan yang diinginkan. Dalam hal ini, Bubble Sort akan melalui iterasi sebanyak (n-1) kali seperti pada worst case, tetapi tidak ada pertukaran yang perlu dilakukan pada setiap langkahnya, karena array sudah terurut dengan benar. Oleh karena itu, dalam best case, kompleksitas waktu Bubble Sort adalah O(n), dengan n adalah jumlah elemen dalam array.
c. Average case:
Untuk kasus rata-rata, asumsikan bahwa semua kemungkinan urutan elemen memiliki probabilitas yang sama. Dalam hal ini, Bubble Sort pada rata-rata akan melalui (n-1) iterasi, dengan pertukaran yang mungkin terjadi dalam setiap langkah iterasi. Secara umum, dalam kasus rata-rata, kompleksitas waktu Bubble Sort juga adalah O(n^2), karena dalam banyak kasus, kita masih harus membandingkan dan menukar elemen dalam setiap langkah iterasi.
#Analisis Algorithm untuk mengevaluasi TSP (Travelling Salesman Problem) 
Untuk contoh kasus  dengan, Waktu Komputasi: 1.7194123268127441 detik, Shortest Path: ('A', 'B', 'C', 'E', 'G', 'F', 'D'), Jarak: 49, maka dapat dilakukan analisis sebagai berikut:
a. Worst Case:
Dalam Travelling Salesman Problem (TSP), kasus terburuk terjadi ketika algoritma harus memeriksa setiap kemungkinan permutasi untuk mencari solusi optimal. Dalam kasus ini, terdapat 6 titik (A, B, C, E, G, F) yang harus dikunjungi. Jumlah total kemungkinan permutasi yang harus diperiksa adalah (6-1)! = 5! = 120. Oleh karena itu, kompleksitas waktu kasus terburuk dalam TSP adalah O((n-1)!), di mana n adalah jumlah titik yang harus dikunjungi.
b. Best Case:
Dalam TSP, kasus terbaik terjadi ketika solusi optimal dapat ditemukan langsung tanpa harus memeriksa kemungkinan permutasi tambahan. Dalam kasus ini, algoritma langsung menemukan rute optimal ('A', 'B', 'C', 'E', 'G', 'F', 'D'). Oleh karena itu, kompleksitas waktu kasus terbaik dalam TSP adalah O(1), karena hanya satu rute yang perlu diperiksa.
c. Average Case:
Analisis rata-rata dalam TSP bisa rumit dan melibatkan faktor-faktor seperti struktur grafik, jumlah titik, dan fungsi biaya. Tanpa informasi lebih lanjut tentang distribusi kemungkinan rute atau struktur grafik yang digunakan, sulit memberikan analisis yang akurat untuk kasus rata-rata dalam TSP.
#Analisis Algorithm untuk mengevaluasi Dijkstra
Untuk contoh kasus sebagai berikut, Algoritma Dijkstra
Dengan titik awal: B
Dan titik tujuan: F
Iterasi: Rute ['B'] - Jarak: 0
Iterasi: Rute ['B', 'C'] - Jarak: 8
Iterasi: Rute ['B', 'C', 'E'] - Jarak: 11
Iterasi: Rute ['B', 'D'] - Jarak: 12
Iterasi: Rute ['B', 'A'] - Jarak: 12
Iterasi: Rute ['B', 'C', 'G'] - Jarak: 17
Waktu Komputasi: 0.0018644332885742188 detik
Shortest Path:
['B', 'C', 'E', 'F']
Jarak: 17, maka dapat dilakukan analisis kasus sebagai berikut:
a. Worst Case:
Dalam kasus terburuk, algoritma Dijkstra akan mengunjungi setiap simpul dan setiap sisi dalam grafik. Jadi, dalam kasus terburuk, kompleksitas waktu algoritma Dijkstra akan bergantung pada jumlah total simpul dan sisi dalam grafik. Dalam kasus ini, kita memiliki 7 simpul (B, C, E, F, D, A, G) dan 10 sisi. Sehingga, kompleksitas waktu terburuk adalah O((V + E) log V) = O((7 + 10) log 7) = O(17 log 7).
b. Best Case:
Dalam kasus terbaik, algoritma Dijkstra akan menemukan jalur terpendek langsung dari titik awal ke titik tujuan tanpa harus memeriksa simpul atau sisi tambahan. Dalam kasus ini, algoritma langsung mencapai tujuan melalui rute ['B', 'C', 'E', 'F']. Dalam hal ini, kompleksitas waktu algoritma Dijkstra adalah O(V log V) = O(7 log 7).
c. Average Case:
Dalam kasus rata-rata, kompleksitas waktu algoritma Dijkstra akan bergantung pada struktur grafik dan jarak terpendek antara titik awal dan titik tujuan. Dalam hal ini, tidak ada informasi yang cukup untuk memberikan analisis yang tepat mengenai rata-rata kasus, karena kita hanya memiliki satu contoh jalur terpendek yang dihitung oleh algoritma Dijkstra.
