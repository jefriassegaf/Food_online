# Food_online
# Online Foodshop

Achmad Jefri Assegaf- 1605552036


## Abstrak

Program pembelian makanan _online_ berbasis CLI atau _Command Line Interface_. Program ini dibangun dengan bahasa pemrograman Java. Java adalah salah satu bahasa pemrograman populer yang digunakan untuk mengembangkan aplikasi _mobile_, _desktop_, hingga website. Kepopulerannya dibuktikan dari jumlah pengembang yang menggunakan bahasa ini, yaitu sekitar 10 juta pengembang dari seluruh dunia.

## UML Class Diagram

UML _Class Diagram_ adalah jenis diagram yang digunakan dalam pengembangan program untuk menggambarkan struktur sistem berorientasi objek. _Class diagram_ menggambarkan kelas, objek, atribut, metode, hubungan antar kelas, dan interaksi antara objek. Berikut adalah UML _Class Diagram_ dari program '**Food_onlinep**':

![UML Food_online](img/UML%20Online%20Food%20Shop.jpg "UML Food_online")


## Alat

Berikut alat yang digunakan untuk membangun program ini:

#### Visual Studio Code

Visual Studio Code atau sering disingkat VS Code adalah sebuah _open source text editor_ yang dikembangkan oleh Microsoft. VS Code dirancang untuk memungkinkan pengembangan dan _debugging_ program dengan mudah dan cepat. Editor ini mendukung banyak bahasa pemrograman, termasuk JavaScript, Python, C++, dan banyak lagi.

[Download Visual Studio Code](http://code.visualstudio.com/download)

#### Extension Pack for Java

Extension Pack for Java adalah kumpulan ekstensi populer yang dapat membantu untuk menulis, mengetes, dan men-_debug_ program Java di Visual Studio Code.

[Download Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)

## Prasyarat

Adapun prasyarat untuk menjalankan program ini adalah sebagai berikut:

-   Java Development Kit minimal versi 11

[Download JDK](https://www.oracle.com/id/java/technologies/downloads/archive/)

## Penggunaan

Untuk menjalankan program ini Anda dapat melakukan langkah-langkah berikut:


#### Command

Untuk menjalankan file JAR tersebut dengan _command_ berikut:

`$ java -jar Food_online.jar`

#### Alur Program

Berikut adalah alur dari jalannya program Food_online.

![Introduction](/img/Introduction.png "Introduction")

###### Login

Pengguna akan diminta untuk memasukkan kredensial agar dapat melanjutkan program. Terdapat dua tipe pengguna yaitu Administrator dan Pelanggan (_Customer_) yang kredensialnya dapat dilihat pada keterangan di bawah.

**Administrator**
`Username   : admin`
`Password   : admin`

**Customer**
`Username   : customer`
`Password   : customer`

![Login](/img/Login.png "Login")

###### Admin

1. **Menu Utama**
   Menu utama saat pengguna merupakan adminstrator dapat dilihat pada gambar di bawah. Dimana admin dapat melihat, menambah, dan menghapus restoran.

![Menu Admin](/img/Menu%20Admin.png "Menu Admin")

2. **Lihat Restoran**
   Admin dapat melihat restoran yang telah ditambahkan atau diregistrasikan dari menu Tambah Restoran. Restoran yang ditampilkan berasal dari kumpulan `Restaurants` yang diinstansiasi di dalam _Array List_ pada class `Data`.

![Lihat Restoran 1](/img/Lihat%20Restoran.png "Lihat Restoran 1")
![Lihat Restoran 2](/img/Lihat%20Restoran%202.png "Lihat Restoran 2")

3. **Tambah Restoran**
   Admin dapat menambahkan restoran baru yang akan disimpan pada Array List `Restaurants` yang terdapat pada class `Data`.

![Tambah Restoran 1](/img/Tambah%20Restoran.png "Tambah Restoran 1")
![Tambah Restoran 2](/img/Tambah%20Restoran%202.png "Tambah Restoran 2")

4. **Hapus Restoran**
   Admin dapat menghapus restoran yang telah teregistrasi dengan memasukkan ID restoran yaitu nomor yang terletak sebelum nama restoran.

![Hapus Restoran 1](/img/Hapus%20Restoran.png "Hapus Restoran 1")
![Hapus Restoran 2](/img/Hapus%20Restoran%202.png "Hapus Restoran 2")

###### Customer

1. **Menu Utama**
   Gambar di bawah adalah tangkapan layar dari menu utama saat pengguna _log in_ sebagai _customer_. _Customer_ dapat melihat retoran serta menambah, melihat, dan menghapus pesanan. _Customer_ juga dapat melakukan pembayaran.

![Menu Customer](/img/Menu%20Customer.png "Menu Customer")

2. **Lihat Restoran**
   _Customer_ dapat melihat restoran yang ada. Eksistensi restoran ini hanya dapat dimanipulasi oleh adminstrator, _customer_ hanya dapat melihat daftar restoran yang ada.

![Lihat Restoran 1](/img/Lihat%20Restoran.png "Lihat Restoran 1")
![Lihat Restoran 2](/img/Lihat%20Restoran%202.png "Lihat Restoran 2")

3. **Tambah Pesanan**
   _Customer_ dapat menambahkan data pesanan. Untuk menambahkan data pesanan, _customer_ harus mengisi beberapa data yang diantaranya adalah ID restoran, ID menu, jumlah pesanan, serta jarak ke lokasi antar (dalam KM). Setelah itu akan ditampilkan pesanan yang _customer_ pesan, total harga sudah termasuk biaya antar.

Keterangan :

```
if (distance < 5) {<br>
    return menuPrice * quantity + 5000;
} else {
    return menuPrice * quantity + 5000 + distance * 1000;
}
```

![Tambah Pesanan 1](/img/Tambahkan%20Pesanan.png "Tambah Pesanan 1")
![Tambah Pesanan 2](/img/Tambahkan%20Pesanan%202.png "Tambah Pesanan 2")

4. **Lihat Pesanan**
   _Customer_ dapat melihat pesanan yang telah ditambahkan pada menu Tambah Pesanan. Sama halnya dengan bagian sebelumnya, total harga yang tertera sudah termasuk biaya antar yang telah dikalkulasikan.

![Lihat Pesanan 1](/img/Lihat%20Pesanan.png "Lihat Pesanan 1")

5. **Hapus Pesanan**
   _Customer_ dapat menghapus pesanan dengan memasukkan ID pesanan. Data pesanan (`Orders`) yang disimpan pada _class_ `Data` akan dihapus sesuai indeks _array_ yang dimasukkan oleh _customer_.

![Hapus Pesanan 1](/img/Hapus%20Pesanan.png "Hapus Pesanan 1")

6. **Pembayaran**
   _Customer_ dapat melakukan pembayaran, dimana akan ditampilkan nota pesanan serta kode pembayaran. Jika _customer_ melanjutkan pembayaran maka seluruh data pesanan akan dihapus.

![Pemabayaran](/img/Pembayaran.png "Pembayaran")

## Penutup

Terimakasih.
