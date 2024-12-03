# Beijing Air Quality Analysis 
Dicoding Data Analysis Project ✨
[Explore the Dashboard](https://air-quality-beijing-view.streamlit.app/)

## Project Overview
Project ini adalah project data analisis dari Dicoding untuk menganalisis kualitas udara di Beijing dengan memanfaatkan data historis dari berbagai parameter polutan udara, seperti PM2.5, PM10, SO2, NO2, CO, dan O3. Selain itu, proyek ini juga mempertimbangkan faktor-faktor lingkungan seperti suhu, tekanan udara, kelembapan, curah hujan, arah angin, dan kecepatan angin. Analisis ini bertujuan untuk memberikan wawasan yang lebih dalam mengenai tren kualitas udara di Beijing, hubungan antarparameter, serta dampak potensial terhadap kesehatan masyarakat. Hasilnya diharapkan dapat menjadi acuan untuk pengambilan keputusan yang lebih baik dalam pengelolaan lingkungan dan kebijakan udara bersih.

## Problem Understanding
Kualitas udara yang buruk telah menjadi salah satu tantangan utama di banyak kota besar, termasuk Beijing, dengan dampak signifikan terhadap kesehatan masyarakat dan lingkungan. Untuk memahami akar permasalahan dan mencari solusi yang tepat, analisis data kualitas udara menjadi langkah penting. Proyek ini bertujuan untuk menjawab beberapa pertanyaan kunci terkait polusi udara dan faktor meteorologi yang memengaruhinya, dengan tujuan memberikan wawasan yang berguna bagi pengambilan keputusan.
Terdapat tiga buah masalah yang ingin diselesaikan dalam proyek ini yaitu:
1. Analisis Kualitas Udara: Kota apa yang memiliki udara paling bersih dan paling kotor dari segi partikel udara?
   Analisis ini bertujuan untuk menentukan kota mana yang memiliki kualitas udara terbaik dan terburuk dari segi konsentrasi partikel. Informasi ini akan membantu mengidentifikasi daerah yang paling membutuhkan intervensi, seperti peningkatan regulasi industri atau transportasi untuk mengurangi emisi.
2. Analisis Meteorologi: Kota apa yang memiliki curah hujan paling tinggi dan paling rendah? Bagaimana pengaruh hujan terhadap polusi udara?
   Analisis ini menyoroti faktor meteorologi, khususnya curah hujan, yang berperan penting dalam memengaruhi kualitas udara. Kota dengan curah hujan tinggi cenderung memiliki udara yang lebih bersih karena partikel polutan dibersihkan oleh hujan. Analisis ini bertujuan untuk memahami kota mana yang memiliki curah hujan tertinggi dan terendah serta bagaimana pola hujan memengaruhi tingkat polusi udara. Wawasan ini penting untuk mengintegrasikan kondisi cuaca dalam strategi pengelolaan lingkungan.
3. Analisis Kualitas Udara: Kota apa yang memiliki udara paling bersih dan paling kotor dari segi gas?
   Analisis ini akan mengidentifikasi kota yang memiliki kualitas udara terbaik dan terburuk dari segi konsentrasi gas. Hasil analisis ini dapat memberikan gambaran tentang sumber utama emisi gas, seperti pembangkit listrik atau kendaraan bermotor, dan membantu menyusun kebijakan pengendalian emisi yang lebih efektif.


## Data Understanding
Dataset yang digunakan merupakan dataset kualitas udara dari 12 kota di China, yaitu Aotizhongxin, Changping, Dingling, Dongsi, Guanyuan, Gucheng, Huairou, Nongzhanguan, Shunyi, Tiantan, Wanliu dan Wanshouxigong. Data diambil setiap interval 1 jam dari 1 Maret 2013 sampai dengan 28 Februari 2017. Dataset terdiri dari 17 kolom data dengan rincian sebagai berikut:
1. year: Tahun diambilnya data.
2. month: Bulan diambilnya data.
3. date: Tanggal diambilnya data.
4. hour: Jam diambilnya data.
5. PM2.5: Particulate Matter 2.5, Konsentrasi partikel halus di udara yang berukuran ≤2.5 mikrometer (μg/m³).
6. PM10: Particulate Matter 10, Konsentrasi partikel kasar di udara yang berukuran ≤10 mikrometer (μg/m³).
7. SO2: Sulfur Dioxide, Konsentrasi sulfur dioksida di udara (μg/m³).
8. NO2: Nitrogen Dioxide, Konsentrasi nitrogen dioksida di udara (μg/m³).
9. CO: Carbon Monoxide, Konsentrasi karbon monoksida di udara (μg/m³).
10. O3: Ozone, Konsentrasi ozon di udara (μg/m³).
11. TEMP: Temperature, Suhu udara dalam derajat Celcius (°C).
12. PRES: Pressure, Tekanan atmosfer dalam hPa.
13. DEWP: Dew Point, Titik embun dalam derajat Celcius (°C).
14. RAIN: Rainfall, Curah hujan atau intensitas hujan dalam mm.
15. wd: Wind Direction, Arah angin (dalam singkatan, seperti WNW untuk West-Northwest).
16. WSPM: Wind Speed per Minute, Kecepatan angin dalam m/s.
17. station: Nama stasiun tempat data diambil.

## Analysis & Visualization
![Visualisasi 1](https://raw.githubusercontent.com/prtmaars/Air-Quality-Beijing/master/images/collage1.png)
Berdasarkan pada grafik di atas, Kota Nongzhanguan memiliki curah hujan paling tinggi dan Kota Dingling memiliki curah hujan paling rendah. Jika dibandingkan dengan grafik pada partikel udara, nampaknya bahwa curah hujan yang tinggi tidak terlalu berpengaruh secara signifikan terhadap kualitas udara. Terlihat bahwa kota dengan kualitas udara paling bersih dari segi partikel udara yaitu Kota Dingling berada di urutan paling terakhir dengan curah hujan paling tinggi, sedangkan Kota Gucheng yang merupakan kota dengan kualitas udara paling kotor dari segi partikel udara berada di urutan ke-7. Sehingga dapat disimpulkan bahwa curah hujan masih mempengaruhi kualitas udara walaupun tidak signifikan.
PM2.5 atau Particulate Matter 2.5 merupakan konsentrasi partikel halus di udara yang berukuran ≤2.5 mikrometer (μg/m³), sedangkan PM10 atau Particulate Matter 10 merupakan konsentrasi partikel kasar di udara yang berukuran ≤10 mikrometer (μg/m³). Pada dasarnya, perhitungan pada PM10 sudah mencakup dari perhitungan PM2.5. Dalam hal ini, dapat disimpulkan bahwa kota yang memiliki jumlah PM10 paling banyak merupakan kota dengan kualitas udara paling kotor dari segi partiker udara dan kota yang memiliki jumlah PM10 paling sedikit merupakan kota dengan kualitas udara paling bersih dari segi partikel udara. Maka, dalam rentang waktu 1 Maret 2013 sampai dengan 28 Februari 2017, Kota Dingling merupakan kota paling bersih dan Kota Gucheng merupakan kota paling kotor pada kualitas udaranya dari segi partikel udara.
Setelah dilakukan pengelompokan berdasarkan AQI (Air Quality Index), didapat bahwa 9 dari 12 kota berada pada kategori Sangat Tidak Sehat yaitu Kota Aotizhongxin, Kota Dongsi, Kota Guanyuan, Kota Gucheng, Kota Nongzhanguan, Kota Shunyi, Kota Tiantan, Kota Wanliu dan Kota Wanshouxigong. Sedangkan 3 lainnya berada pada kategori Tidak Sehat yaitu Kota Changping, Kota Dingling dan Kota Huairou.

![Visualisasi 2](https://raw.githubusercontent.com/prtmaars/Air-Quality-Beijing/master/images/collage2.png)
Pada gas SO2 atau Sulfur Dioksida, WHO (World Health Organization) menetapkan ambang batas aman di angka 20 μg/m³. Berdasarkan grafik di atas, konsentrasi gas SO2 di seluruh kota masih berada di bawah ambang batas sehingga dapat dikatakan aman. Meskipun demikian, Kota Nongzhanguan memiliki konsentrasi gas SO2 paling tinggi dan Kota Dingling memiliki konsentrasi gas SO2 paling rendah diantara kota-kota lainnya.
Pada gas NO2 atau Nitrogen Dioksida, WHO (World Health Organization) menetapkan ambang batas aman di angka 10 μg/m³. Berdasarkan grafik di atas, konsentrasi gas NO2 di seluruh kota melebihi ambang batas sehingga dapat dikatakan tidak aman. Kota Wanliu memiliki konsentrasi gas NO2 paling tinggi dan Kota Dingling memiliki konsentrasi gas NO2 paling rendah diantara kota-kota lainnya walaupun masih berada di atas batas aman.
Pada gas O3 atau Ozon, WHO (World Health Organization) menetapkan ambang batas aman di angka 100 μg/m³. Berdasarkan grafik di atas, konsentrasi gas O3 di seluruh kota masih berada di bawah garis ambang batas sehingga dapat dikatakan aman. Meskipun demikian, Kota Dingling memiliki konsentrasi gas O3 paling tinggi dan Kota Wanliu memiliki konsentrasi gas O3 paling rendah diantara kota-kota lainnya.
Pada gas CO atau Karbon Monoksida, WHO (World Health Organization) menetapkan ambang batas aman di angka 4000 μg/m³. Berdasarkan grafik di atas, konsentrasi gas CO di seluruh kota masih berada di bawah garis ambang batas sehingga dapat dikatakan aman. Meskipun demikian, Kota Wanshouxigong memiliki konsentrasi gas CO paling tinggi dan Kota Dingling memiliki konsentrasi gas CO paling rendah diantara kota-kota lainnya.

## Conclusion
Konklusi Masalah 1: Kualitas Udara Berdasarkan Partikel Udara
Berdasarkan analisis kualitas udara dari segi partikel udara, Kota Dingling menempati posisi sebagai kota dengan kualitas udara paling bersih, dengan konsentrasi partikel udara yang relatif rendah dibandingkan kota lainnya. Sebaliknya, Kota Gucheng memiliki kualitas udara yang paling buruk, dengan tingkat polusi partikel yang sangat tinggi. Namun, meskipun Kota Dingling menunjukkan kualitas udara yang lebih baik, hasil analisis lanjutan yang mengelompokkan kota-kota berdasarkan Air Quality Index (AQI) menunjukkan bahwa Kota Dingling masih berada dalam kategori Tidak Sehat, sementara Kota Gucheng masuk dalam kategori Sangat Tidak Sehat. Hal ini menunjukkan bahwa meskipun tingkat polusi partikel di Kota Dingling lebih rendah, kualitas udara secara keseluruhan masih belum memenuhi standar kesehatan yang ideal.

Konklusi Masalah 2: Pengaruh Curah Hujan terhadap Kualitas Udara
Dalam hal pengaruh curah hujan terhadap kualitas udara, ditemukan bahwa Kota Nongzhanguan memiliki curah hujan tertinggi, sementara Kota Dingling memiliki curah hujan paling rendah. Namun, hasil analisis menunjukkan bahwa curah hujan tidak memiliki pengaruh yang signifikan terhadap tingkat polusi udara, terutama dari segi partikel udara. Hal ini mengindikasikan bahwa faktor lain, seperti aktivitas industri atau lalu lintas kendaraan, mungkin memiliki peran yang lebih besar dalam menentukan kualitas udara, ketimbang curah hujan itu sendiri.

Konklusi Masalah 3: Kualitas Udara Berdasarkan Konsentrasi Gas Polutan
Dari segi gas polutan, beberapa kota menunjukkan tingkat konsentrasi gas yang signifikan. Kota Nongzhanguan tercatat memiliki konsentrasi gas SO2 tertinggi, sedangkan Kota Dingling tercatat sebagai kota dengan konsentrasi gas SO2 terendah. Untuk gas NO2, Kota Wanliu menempati posisi dengan konsentrasi tertinggi, sementara Kota Dingling memiliki konsentrasi NO2 terendah. Pada gas O3, Kota Dingling tercatat memiliki konsentrasi O3 paling tinggi, sedangkan Kota Wanliu memiliki konsentrasi O3 paling rendah. Gas CO menunjukkan konsentrasi tertinggi di Kota Wanshouxigong, sementara Kota Dingling kembali mencatatkan konsentrasi CO terendah. Secara keseluruhan, Kota Dingling dapat dikategorikan sebagai kota paling bersih dari segi gas polutan, karena menduduki peringkat terendah dalam konsentrasi SO2, NO2, dan CO. Meskipun demikian, konsentrasi gas O3 di Kota Dingling lebih tinggi, yang menandakan adanya tantangan dalam mengelola semua jenis polusi udara secara menyeluruh.

Secara keseluruhan, hasil analisis ini memberikan gambaran yang jelas mengenai kondisi kualitas udara di berbagai kota. Meskipun beberapa kota menunjukkan kualitas udara yang lebih baik dari segi partikel dan gas polutan tertentu, penting untuk diingat bahwa kualitas udara keseluruhan, seperti yang tercermin dalam AQI, harus dipertimbangkan dalam perumusan kebijakan dan langkah-langkah mitigasi yang efektif.

___
