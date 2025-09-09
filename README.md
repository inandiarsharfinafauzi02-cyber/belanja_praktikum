# praktikum 2
## Langkah 1: Siapkan project bar
Sebelum melanjutkan praktikum, buatlah sebuah project baru Flutter dengan nama belanja dan susunan folder seperti pada gambar berikut. Penyusunan ini dimaksudkan untuk mengorganisasi kode dan widget yang lebih mudah.
hasil
<img width="169" height="131" alt="image" src="https://github.com/user-attachments/assets/b61fec38-7026-4c34-9c2c-ed45914f81ed" />

## Langkah 2: Mendefinisikan Route
Buatlah dua buah file dart dengan nama home_page.dart dan item_page.dart pada folder pages. Untuk masing-masing file, deklarasikan class HomePage pada file home_page.dart dan ItemPage pada item_page.dart. Turunkan class dari StatelessWidget. Gambaran potongan kode dapat anda lihat sebagai berikut
<img width="1114" height="566" alt="image" src="https://github.com/user-attachments/assets/b8b903a4-369e-4290-84f9-9b0bea10a610" />
<img width="944" height="900" alt="image" src="https://github.com/user-attachments/assets/3a2d39b6-f826-405a-a3ad-f1da2829b403" />
<img width="944" height="678" alt="image" src="https://github.com/user-attachments/assets/321d759d-a1d7-4f46-96f9-c8c219384add" />

## Langkah 3: Lengkapi Kode di main.dart
Setelah kedua halaman telah dibuat dan didefinisikan, bukalah file main.dart. Pada langkah ini anda akan mendefinisikan Route untuk kedua halaman tersebut. Definisi penamaan route harus bersifat unique. Halaman HomePage didefinisikan sebagai /. Dan halaman ItemPage didefinisikan sebagai /item. Untuk mendefinisikan halaman awal, anda dapat menggunakan named argument initialRoute. Gambaran tahapan ini, dapat anda lihat pada potongan kode berikut.
<img width="928" height="826" alt="image" src="https://github.com/user-attachments/assets/e9e510cd-ca91-4d9c-8479-7004c2cebe17" />

## Langkah 4: Membuat data model
Sebelum melakukan perpindahan halaman dari HomePage ke ItemPage, dibutuhkan proses pemodelan data. Pada desain mockup, dibutuhkan dua informasi yaitu nama dan harga. Untuk menangani hal ini, buatlah sebuah file dengan nama item.dart dan letakkan pada folder models. Pada file ini didefinisikan pemodelan data yang dibutuhkan. Ilustrasi kode yang dibutuhkan, dapat anda lihat pada potongan kode berikut.
<img width="1114" height="566" alt="image" src="https://github.com/user-attachments/assets/3410cb0c-da9a-4486-8a9e-99a912f082a0" />
letak
<img width="178" height="73" alt="image" src="https://github.com/user-attachments/assets/d9630165-5174-46e9-8a5d-e3d39ccbe69c" />

## Langkah 5: Lengkapi kode di class HomePage
Pada halaman HomePage terdapat ListView widget. Sumber data ListView diambil dari model List dari object Item. Gambaran kode yang dibutuhkan untuk melakukan definisi model dapat anda lihat sebagai berikut.
<img width="944" height="900" alt="image" src="https://github.com/user-attachments/assets/24461026-3fc9-4d35-8338-fd61ae2b1b44" />

## Langkah 6: Membuat ListView dan itemBuilder
Untuk menampilkan ListView pada praktikum ini digunakan itemBuilder. Data diambil dari definisi model yang telah dibuat sebelumnya. Untuk menunjukkan batas data satu dan berikutnya digunakan widget Card. Kode yang telah umum pada bagian ini tidak ditampilkan. Gambaran kode yang dibutuhkan dapat anda lihat sebagai berikut.
kode
<img width="1670" height="2354" alt="image" src="https://github.com/user-attachments/assets/3421df30-5d25-4f3c-a3b9-8731d9e2f432" />
hasil
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/cf66f6a4-8958-4b86-be08-4db8fd150a70" />


## Langkah 7: Menambahkan aksi pada ListView
Item pada ListView saat ini ketika ditekan masih belum memberikan aksi tertentu. Untuk menambahkan aksi pada ListView dapat digunakan widget InkWell atau GestureDetector. Perbedaan utamanya InkWell merupakan material widget yang memberikan efek ketika ditekan. Sedangkan GestureDetector bersifat umum dan bisa juga digunakan untuk gesture lain selain sentuhan. Pada praktikum ini akan digunakan widget InkWell.
Untuk menambahkan sentuhan, letakkan cursor pada widget pembuka Card. Kemudian gunakan shortcut quick fix dari VSCode (Ctrl + . pada Windows atau Cmd + . pada MacOS). Sorot menu wrap with widget... Ubah nilai widget menjadi InkWell serta tambahkan named argument onTap yang berisi fungsi untuk berpindah ke halaman ItemPage. Ilustrasi potongan kode dapat anda lihat pada potongan berikut.
kode
<img width="1198" height="528" alt="image" src="https://github.com/user-attachments/assets/205de8f3-cdc8-4014-bfca-2a29ecdfb0a6" />
hasil 
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/cd5c551c-58e6-49b3-901c-d5dfc748e54e" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/a08473cf-4f52-4064-8c50-c2e0b57c5101" />




