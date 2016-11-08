Latar Belakang Masalah
Data Geospasial Adalah pengetahuan yang mempelajari tentang titik koordinat dari suatu peta atau juga mempelajari tentang geografis yang ada di muka bumi. Dan saya akan menjelaaskan secara teori apa itu ESRI pada Retrive Geospasial. Dalam geospasial kita bisa mengitung secara rinci data record pada file.
Penjelasan
Apa itu Retrieve data geospasial:  Retrieve data geospasial merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.
Dan apa itu SHP: SHP yaitu salah satu file yang berada didalam shapefile tujuan nya untuk menyimpan data geometri.
Didalam file shp terdapat data-data seperti:
1.       Bbox : sebuah boundary box (koordinat 4 titik) atau koordinat batas view yang ada pada peta, Lebih tepat nya titik antar sisi dari peta.
2.       Point : titik suatu koordinat dalam peta.
3.       Shapetype : jenis data geometri yang mempunyai standar nomor yang ditetapkan oleh ESRI seperti nomor 1 untuk poin, 2 untuk polygon, 3 untuk polyline, dll. 
Contoh ada pada link: shapefile.esri


Apa itu DBF: Dbf adalah sebuah file yang menyimpan file tabular dan juga menyimpan data attribut.
Membaca Jumlah data geometri dengan python:
-          Membaca data shp
>> import shapefile
>> sf = shapefile.Reader(“namafile.shp”)
>> sf.shapes()
>> a = sf.shapes()
>> len(a)

-          Membaca data DBF
>> import shapefile
>> sf.records()
>> sf.records(n)
Kesimpulan:
Dalam data Retrieve ini kita dapat melakukan select/view dan menghitung jumlah record. Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.
Saran:
                Sebaiknya lebih banyak lagi orang yang mempelajari dan menggunakan data-data yang seperti diatas. Dan mempraktekannya, banyak orang yang mengerti tentang data retrieve pada data geospasial.
