# MVCconcept-fakhri
**Penjelasan dan Pengertian MVC**

MVC (Model View Controller) adalah sebuah pola yang sudah teruji dalam pengembangan aplikasi. Awalnya, MVC digunakan untuk pengembangan GUI desktop, tapi kini telah banyak diadopsi oleh framework-framework aplikasi berbasis web. Jika kita mengembangkan aplikasi tanpa pola MVC, kita berkecenderungan untuk mencampur adukkan kode logika kita dengan kode tampilan serta kode untuk mengambil data ke database. Benar? Nah dengan MVC tidak begitu, karena dengan pola MVC, kita membagi komponen aplikasi kita menjadi 3 bagian yang terpisah namun saling berkaitan, yaitu Model, View dan Controller. **Model** Merupakan komponen dalam aplikasi kita yang berfungsi mengelola akses langsung dengan logika pengelolaan dan sumber data. Model berhubungan erat dengan database yang nanti akan digunakan. **View** adalah komponen dalam aplikasi kita yang berfungsi untuk membuat interface (tampilan) untuk pengguna. Sumber data didapat dari model yang didapatkan melalui controller tidak berinteraksi langsung dengan database. View juga menangkap interaksi dari pengguna yang akan di-redirect ke aplikasi. Yang terakhir, **Controller** Merupakan komponen dalam aplikasi kita yang bertugas untuk menerima input dan memberikan output (request dan response). Controller bertugas untuk menerima request, kemudian memprosesnya dengan memberikan response baik berupa data atau view berisi data dari model.

Berikut merupakan gambaran MVC pada Laravel:

**A.** User mengakses website melalui route tertentu.

**B.** Route tersebut akan mengarah / merujuk kepada controller action.

**C.** Apabila terdapat data yang ingin diakses, maka controller akan menuju model. Bila tidak ada, controller langsung mengembalikan 
       sebuah view tanpa data (langsung ke poin E).

**D.** Model ini akan berinteraksi dengan database untuk mendapatkan sebuah data, menyimpan, merubah, maupun menghapus data.

**E.** Setelah berhasil mendapatkan data dari model, controller akan mengembalikan sebuah view beserta data jika ada.

**F.** Proses terakhir dimana view dilihat oleh user.
