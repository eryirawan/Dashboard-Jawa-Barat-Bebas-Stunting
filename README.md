# Project-Lab-BI-Jabar-Bebas-Stunting
This project is to giving the information about cause of stunting, map in west java with some of the metrics, and Correlation between health worker and baby under 2 years old with malnutrition also with pregnant woman with anemia.

## BACKGROUNDS

Stunting atau sering disebut dengan kerdil atau pendek merupakan kondisi gagal tumbuh pada anak berusia dibawah 5 tahun (balita) akibat kekurangan gizi kronis dan infeksi berulang pada 1000 Hari pertama Kehidupan (HPK) yaitu dari janin hingga anak berusia 23 bulan.1 Berdasarkan Conceptual Framework UNICEF setidaknya ada 2 tujuan dari 4 yang dicanangkan oleh UNICEF yaitu To Prevent undernutrition, micronutrient deficiencies, and overweight in early Childhood (The First five years of Live) dan To prevent undernutrition, micronutrient deficiencies, and overweight in mothers, and low birthweight in newborns.2 

Global Nutrition Report 2016, menyebutkan bahwa prevalensi stunting di Indonesia berada pada peringkat 108 dari 132 negara di dunia. Pada kawasan Asia Tenggara Prevalensi stunting di Indonesia merupakan tertinggi kedua setelah kamboja. Hasil Riset Kesehatan Dasar 2018 angka stunting di Indonesia mencapai 30,8%, artinya dari 100 balita yang lahir di indonesia hampir 30 balita dapat mengalami risiko stunting. Sementara di Jawa Barat kasus stunting berada di angka 24,5% dengan yang tertinggi berada di Kabupaten Garut. 

Dengan tingginya angka prevalensi Stunting di Jawa Barat dan permasalahan data yang ada di lapangan, untuk itu diperlukan sebuah kebijakan yang tepat sasaran dengan berdasarkan data yang akurat serta detail pada Provinsi Jawa Barat.  Agar nantinya kebijakan yang dibuat oleh Kepala daerah atau dibawahnya bisa bermanfaat untuk masyarakat luas. 

## OBJECTIVES
Memberikan Dashboard yang informatif secara deskriptif mengenai gambaran daerah dengan bayi bergizi buruk/Malnutrition, Ibu Hamil dengan Anemia serta jumlah tenaga kesehatan pada wilayah yang mengalami masalah tersebut. Selain itu Dashboard ini diharapkan dapat mudah dipahami oleh para stakeholder dengan tujuan dapat saling bekerja sama dalam menangani stunting di Jawa Barat.

## OVERVIEW PROCESS

### METHODS :
1. Eksplorasi data
2. Menentukan metrics yang akan disajikan
3. Menentukan design visualisasi
4. Wrangling data menggunakan sql
5. Membuat user flow dan hi fi prototype
6. Membuat tableau dashboard

### USERFLOW

![Jabar Bebas Stunting](https://user-images.githubusercontent.com/102465817/189682204-c85ba43a-a35d-4b8e-9b76-52c231f7dd58.jpg)

### PROTOTYPE/MOCKUP
![Desktop-1](https://user-images.githubusercontent.com/102465817/189687232-3122fa8f-bf9a-4606-9e22-fe1dd3ed50b7.png)

![Desktop-2](https://user-images.githubusercontent.com/102465817/189687239-b490cb17-ba4d-45c9-9cf1-4e1ad524f688.png)

![Desktop-3](https://user-images.githubusercontent.com/102465817/189687251-4a2e952d-56fa-4197-a7d9-64097a9b1186.png)

## TAMPILAN DASHBOARD

### HALAMAN 1:

![Dashboard 1](https://user-images.githubusercontent.com/102465817/189687755-d2ca4b96-aa05-49c9-a7f3-0d070b191f6b.png)

Pada halaman pertama dashboard disajikan data TOP 10 kabupaten/kota, yang memiliki angka Bayi malnutrisi dan kasus ibu hamil tertinggi dan kabupaten yang memiliki indeks kesehatan terendah. Data 10 kabupaten/kota ini bisa disesuaikan dengan tahunnya. Pada keterangan All itu menunjukan jumlah pada Bayi Malnutrition, Ibu Hamil dengan Anemia, dan Rata-rata Indeks Kesehatan selama 3 tahun (2016-2018). Selanjutnya dapat dipilih berbeda-beda tahun antara 2016, 2017 atau 2018.

Pada pojok kanan atas halaman ini, diperlihatkan dua tulisan yaitu “Map” dan “Correlation”. Tulisan ini apabila di klik oleh cursor mouse akan membawa user kepada halaman Map yang berisi lebih detail jumlah kasus dan metric yang diinginkan, sementara correlation adalah halaman yang berisi hubungan antara kasus bayi Malnutrition dan Ibu Hamil dengan Anemia dengan ketersediaan tenaga kesehatan.

### HALAMAN 2:

![Dashboard 2](https://user-images.githubusercontent.com/102465817/189689004-d6d0e92e-84a9-42a7-96ec-3ff3eee8e9ea.png)

Pada halaman ke-2 ini adalah tampilan Map, terdapat informasi spasial dan juga beberapa metrics yang dapat dilihat berdasarkan filter  per tahun/per kabupaten. Pada halaman ini juga tersedia data rasio tenaga kesehatan dan ibu hamil/bayi lahir. Informasi spasial menunjukan data 3 kasus penyebab Stunting (BBLR, Bayi Malnutrition, dan Ibu Hamil dengan Anemia). Filter diatas spatial map, dapat diganti sesuai dengan tahun yang diinginkan yaitu 2016-2018.

Fitur metrics disitu juga memperlihatkan lebih detail untuk metrics selain 3 kasus sebelumnya yaitu seperti Jumlah kelahiran bayi, Jumlah Ibu hamil, Jumlah Tenaga Kesehatan (Bidan, Dokter, Ahli Gizi, dan Kesehatan Masyarakat).  Pada chart di bawahnya terdapat ratio ibu hamil dan kelahiran bayi terhadap jumlah tenaga kesehatan yang terbagi beberapa tahun dan bisa dijabarkan secara detail menurut daerahnya, apabila user memilih salah satu daerah pada spatial map tersebut. Angka ratio tersebut menunjukan bahwa 1 orang tenaga kesehatan (bidan/dokter/ahli gizi/kesehatan masyarakat) menangani sejumlah ibu hamil dan kelahiran bayi pada wilayah tersebut.

### HALAMAN 3:

![Dashboard 3](https://user-images.githubusercontent.com/102465817/189690495-f0b3c460-19ad-4ac0-8ba7-e62889939c0f.png)

Halaman 3 adalah tabel correlation (pearson) antara dua variabel, kedua variabel tersebut adalah korelasi antara metrics bayi malnutrisi dan ibu hamil anemia dengan jumlah tenaga kesehatan, serta bayi malnutrisi dengan Berat Bayi Lahir Rendah dan Ibu Hamil Anemia. Selain tabel perhitungan angka pearson correlation, ditampilkan juga chart scatter plot antara variabel bayi malnutrition dengan BBLR serta Ibu hamil  Anemia.

Angka-angka pada tabel menunjukan angka yang positif dan negatif, pada angka positif apabila diatas angka 0,2 keatas dapat dikatakan correlation yang moderate positive relationship. Apabila angka diatas 0,4 dapat termasuk strong positive correlation. Sedangkan apabila angka-angka dalam tabel menunjukan angka yang negatif artinya terdapat correlation negative relationship.


## ANALYSIS

Dari korelasi antara bayi malnutrisi dengan tenaga kesehatan berdasarkan jenis profesinya,  jenis profesi bidan menunjukan angka korelasi tertinggi yaitu 0.38  atau dapat dikatakan jumlah tenaga kesehatan khususnya bidan, memiliki pengaruh positif moderat terhadap tinggi rendahnya bayi malnutrisi pertahunnya

Kemudian korelasi antara ibu hamil dengan kondisi anemia dan tenaga kesehatan berdasarkan jenis profesinya,  jenis profesi bidan menunjukan angka korelasi sebesar 0.64. Artinya jumlah tenaga kesehatan khususnya bidan, memiliki pengaruh positif kuat terhadap tinggi rendahnya angka ibu hamil anemia.


## CONCLUSION

Dari grafik korelasi antara bayi malnutrisi dengan tenaga kesehatan berdasarkan profesinya, mayoritas  tidak menunjukan korelasi yang kuat. Maka dapat disimpulkan jumlah bayi malnutrisi dipengaruhi oleh tersedianya jumlah tenaga kesehatan, namun tidak secara signifikan. 

Dari grafik korelasi antara Ibu hamil anemia dengan tenaga kesehatan berdasarkan profesinya, mayoritas  tidak menunjukan korelasi yang kuat. Maka dapat disimpulkan jumlah ibu hamil anemia dipengaruhi oleh tersedianya jumlah tenaga kesehatan, namun tidak secara signifikan mempengaruhi. hanya jenis profesi bidan yang menunjukan pengaruh kuat terhadap jumlah ibu hamil anemia, semakin tinggi jumlah ibu hamil anemia, semakin tinggi pula jumlah bidan yang tersedia pertahunnya.


## DAFTAR PUSTAKA

1. Peraturan Menteri Kesehatan nomor 1995/Menkes/XII/2010.
2. UNICEF Conceptual Framework on the Determinants of Maternal and Child Nutrition. (2020). UNICEF-Nutrition-Strategy-2020-2030 Brief.
3. International Food Policy Research Institute. (2016). 2016 Global Nutrition Report. IFPRI : Washington DC.
4. Riset Kesehatan Dasar (Riskesdas). (2018). Badan Penelitian dan Pengembangan Kesehatan (Balitbangkes), Kementerian Kesehatan.
5. https://databoks.katadata.co.id/datapublish/2022/07/22/prevalensi-balita-stunting-di-kabupaten-garut-tertinggi-se-jawa-barat-pada-2021.

## DATA PENDUKUNG

1. [User flow](https://miro.com/app/board/uXjVPbDf7GE=/?share_link_id=417264863117) 
2. [Mockup/Prototype](https://www.figma.com/file/iLtQDPrLVwPd23vIoWaDyO/Untitled?node-id=0%3A1)
3. [Dashboard](https://public.tableau.com/views/DashboardJabarBebasStunting/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)
