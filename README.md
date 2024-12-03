# Beijing Air Quality Analysis 
Dicoding Data Analysis Project ✨
[Dashboard](https://air-quality-beijing-view.streamlit.app/)

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

## Visualization

## Analysis

___

## Setup Environment - Anaconda
```
conda create --name main-ds python=3.9
conda activate main-ds
pip install -r requirements.txt
```

## Setup Environment - Shell/Terminal
```
mkdir proyek_analisis_data
cd proyek_analisis_data
pipenv install
pipenv shell
pip install -r requirements.txt
```

## Run steamlit app
```
streamlit run dashboard.py
```
