<h1>Cara Penggunaan Git</h1>
<h3>Konfigurasi Git</h3>
<p>Sebelum mengggunakan git, kita harus melakukan konfigurasi terlebih dahulu, dengan perintah berikut ini :

> git config –global user.name “Nama Akun Github Kamu”</br>
> git config –global user.email “Nama Email Kamu yang Terdaftar Di Github”

kemudian enter. </p>

![image](https://user-images.githubusercontent.com/24362384/67117193-3ee16900-f20c-11e9-8de2-f004f3210194.png)

<h3>Membuat Repository Lokal</h3>
<p><ol>
  <li>Membuat Repository
    <ul>
      <li>Buka direktori aktif terlebih dahulu, yang akan kita jadikan tempat penyimpanan file latihan atau project kita dengan   menggunakan windows Explorer. Misalnya di <em>D:\Git_Project.</em></li> 
      <li>Klik kanan pada direktori aktif tersebut, kemudian klik <em>Git Bash Here</em> pada  menu yang muncul, sehingga akan muncul <em>git bash command.</em></li></p>
      
![image](https://user-images.githubusercontent.com/24362384/67117716-9502dc00-f20d-11e9-8a60-a3b5936d072c.png)

   <p><li>Buatlah direktori praktikum project pertama kalian dengan nama <b>Latihan1</b>, caranya adalah dengan mengetik perintah berikut pada <em>git bash command</em> yang tadi kita buka.</li></p>

> Mkdir latihan1</br>
> Cd latihan1

![image](https://user-images.githubusercontent.com/24362384/67118143-84069a80-f20e-11e9-8ea4-d55208aeff9b.png)

   <p><li>Setelah kita memasukkan perintah diatas, maka akan terbuat folder baru dengan nama <b>latihan1.</b></li></p>
   
![image](https://user-images.githubusercontent.com/24362384/67118265-b87a5680-f20e-11e9-8e1e-7f81b116d38f.png)

   <p><li>Jalankan perintah :
  
  > git init
  
  perintah "git init" akan membuat sebuah direktori yang di hidden (disembunyikan) bernama .git di dalam folder project kita.</li></p>
   </ul></li>

![Gambar 14](https://user-images.githubusercontent.com/24362384/67142760-99bba480-f28e-11e9-9999-60d9a4c0e371.PNG)
   
   <li><p>Setelah kita membuat folder yang bernama <b>latihan1</b>, sekarang kita membuat file yang diberi nama <b>README.md</b>, cara membuatnya adalah dengan memasukkan perintah pada git seperti berikut :</p></li>

> Echo “#Latihan 1” >> README.md

![image](https://user-images.githubusercontent.com/24362384/67118589-5e2dc580-f20f-11e9-9e8d-d7b1266fbc98.png)

  <li><p>Dan file <b>README.md</b> pun berhasil dibuat.</p></li>

![image](https://user-images.githubusercontent.com/24362384/67119515-8a4a4600-f211-11e9-8c9b-42e3ad835d30.png)

  <li><p>Setelah kita membuat file <b>README.md</b>, agar file tersebut masuk kedalam repository lokal kita, gunakan perintah :

> Git add README.md
 
 </p></li>

![Gambar 17](https://user-images.githubusercontent.com/24362384/67142794-d7203200-f28e-11e9-868c-b3b29af42b91.PNG)

  <li><p>Untuk menyimpan perubahan yang ada kedalam database repository lokal, gunakan perintah :

> Git commit –m “komentar commit”

</p></li></ol>

![image](https://user-images.githubusercontent.com/24362384/67119726-edd47380-f211-11e9-919a-727d9e682b4b.png)

<h2>Membuat Repository Server</h2>
<ol><p><li>Membuat repository</p>
<ul>
<li>Sesuai dengan namanya, maka kali ini kita akan belajar cara membuat repository di server (Secara online)</li>
  <li>Server yang akan kita gunakan adalah http://github.com</li>
  <li>Pertama kita harus membuat akun terlebih dahulu dengan email dan password yang akan kita gunakan</li>
  <li>Setelah berhasil registrasi, login kedalam http://github.com</li>
  <li>Pada halaman utama http://github.com, klik ikon “+” lalu klik New Repository.</li></br>

![image](https://user-images.githubusercontent.com/24362384/67119952-7226f680-f212-11e9-988c-4d1cdc4e4371.png)

  <li><p>Buatlah repository baru misalnya dengan nama “Latihan 1”, Lalu klik tombol Create Repository.</p></li>
</ul></li>

![image](https://user-images.githubusercontent.com/24362384/67120126-da75d800-f212-11e9-8cb5-42b119450dc3.png)

<li><p>Setelah itu kembali ke <em>Git Bash Command</em> dengan mengetik perintah :</p></li>

> Git remote add origin [url repository github kamu]

<p>Perintah ini digunakan agar repository lokal kita terhubung dengan repository server yang telah kita buat.</p>

![image](https://user-images.githubusercontent.com/24362384/67120283-304a8000-f213-11e9-8c62-b9f99f266020.png)

<li><p>Untuk mengirim perubahan pada lokal repository yang sudah kita commit sebelumnya, gunakan perintah berikut :</p>
  
> Git push –u origin master

![image](https://user-images.githubusercontent.com/24362384/67120307-3d676f00-f213-11e9-93fe-41ad48bfba1e.png)

<ul><li>Saat pertama kali menggunakan perintah ini, maka kita akan diminta memasukan username dan password pada akun http://github.com.</li>
<li>Masukan username dan password sesuai dengan yang kita daftarkan saat membuat akun di http://github.com.</li></br>

![image](https://user-images.githubusercontent.com/24362384/67120417-756eb200-f213-11e9-94f2-3974338912d9.png)

<li>Setelah klik login, tunggulah beberapa saat. Kemudian jendela Git Bash Command akan berubah seperti gambar dibawah ini.</li></br>

![image](https://user-images.githubusercontent.com/24362384/67120461-8b7c7280-f213-11e9-8b55-3849bf2424da.png)
</ul></li>

<li>Untuk melihat berhasil atau tidak file README.md kita upload ke server repository kita, silahkan refresh halaman http://github.com nya, jika tampilannya seperti gambar dibawah ini, maka anda telah berhasil memasukkan file README.md ke dalam server repository yang telah anda buat sebelumnya.</li></br>

![image](https://user-images.githubusercontent.com/24362384/67120531-ac44c800-f213-11e9-8776-a9e34bacc4bb.png)

<p>Kurang lebihnya mohon maaf.</br>
Sekian dan Terima Kasih.</p>
