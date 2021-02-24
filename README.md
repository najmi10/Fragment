# Fragment
Fragment adalah komponen yang memiliki fungsi untuk menampilkan antarmuka ke
pengguna melalui activity dengan memiliki layout xml sendiri, Fragment digunakan agar
komponen tampillan aplikasi menjadi fleksibel dan dapat digunakan kembali ( reusable).
Fragment juga bisa disebut sub nya activity, satu activity bisa memiliki lebih dari satu fragment.
Fragmen memiliki siklus hidupnya sendiri yang sangat mirip dengan Aktivitas, tetapi memiliki peristiwa 
tambahan yang khusus untuk hierarki tampilan, status, dan lampiran Fragmen ke aktivitasnya.
# Lifecycle Fragment
![AltText](https://github.com/najmi10/Fragment/blob/master/lifecycle%20fragment.png)
- [x] onAttach ():  Instance fragmen dikaitkan dengan instance aktivitas. Metode ini dipanggil pertama 
kali, bahkan sebelum metode onCreate (). Metode ini memberi tahu kami bahwa Fragmen kami telah 
dilampirkan ke suatu aktivitas.
- [x] onCreate ():  Ini akan dipanggil saat membuat fragmen. Ini berarti saat instance fragmen baru 
diinisialisasi, yang selalu terjadi setelah ia menempel ke host.
- [x] onCreateView ():  akan dipanggil saat fragmen menggambar UI (antarmuka pengguna) untuk pertama 
kalinya. Untuk menggambar UI untuk fragmen kita, kita harus mengembalikan komponen View dari metode 
ini yang merupakan root layout fragmen kita. Kita juga bisa mengembalikan null jika fragmen tidak 
menyediakan UI.
- [x] onActivityCreated ():  Metode ini dipanggil setelah metode onCreateView () saat aktivitas host 
dibuat. Metode ini menunjukkan bahwa onCreate () aktivitas telah selesai.
- [x] onStart ():  Metode ini dipanggil setelah fragmen terlihat.
- [x] onResume ():  Metode ini dipanggil saat Fragmen terlihat dan tidak bisa dipecahkan.
- [x] onPause ():  Metode ini adalah indikasi pertama bahwa pengguna meninggalkan fragmen saat ini atau
fragmen tidak lagi dapat berinteraksi. Ini terjadi ketika Fragment Transition diproses atau Fragment 
dihapus.
- [x] onStop ():  Metode ini dipanggil setelah metode onPause (). Fragmen akan dihentikan dengan 
memanggil onStop (). Metode ini memanggil saat Fragmen tidak lagi terlihat. itu terjadi baik setelah 
fragmen akan dihapus atau Transisi Fragmen diproses (ganti Fragmen) atau saat aktivitas host berhenti.
- [x] onDestroyView ():  Metode ini dipanggil saat tampilan dan sumber daya terkait lainnya yang dibuat
dalam metode onCreateView () dihapus dari hierarki tampilan aktivitas dan dimusnahkan.
- [x] onDestroy ():  Metode ini dipanggil untuk melakukan pembersihan akhir status Fragmen tetapi tidak
dijamin akan dipanggil oleh platform Android. Metode ini dipanggil setelah metode onDestroyView ().
- [x] onDetach ():  Metode ini dipanggil setelah metode onDestroy () untuk memberi tahu bahwa fragmen 
telah dipisahkan dari aktivitas hostingnya, artinya Fragmen dilepaskan dari Aktivitas hostnya.
# Hasil 1
![AltText](https://github.com/najmi10/Fragment/blob/master/Fragment1.png)
# Hasil 2
![AltText](https://github.com/najmi10/Fragment/blob/master/Fragment2.png)
