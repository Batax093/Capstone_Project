# Capstone Project Infinite Learning
Berikut adalah Repositori Project [Analisa Pandemi Virus Covid-19 di Indonesia Menggunakan Algoritma Regresi](https://github.com/Batax093/Capstone_Project/blob/main/Capstone_IL.ipynb)
Dataset dapat diakses di link Kaggle berikut [Covid-19 Indonesia Dataset](https://www.kaggle.com/datasets/hendratno/covid19-indonesia)

## Pengerjaan project dimulai dengan Data Exploration, Data Preprocessing, Training Model, Model Visualization, dan Evaluation
1. [Data Exploration](#A-data-exploration)
2. [Data Preprocessing](#B-data-preprocessing)
3. [Model Training](#C-model-training)
4. [Model Visualization and Evaluation](#D-model-visualization-and-evaluation)
5. [Kesimpulan](#E-kesimpulan)

### A. Data Exploration
Pada tahap pengerjaan Data Exploration disini saya menganalisa data yang akan 
saya pakai untuk digunakan di dalam projek Analisis Pandemi Covid-19 di 
Indonesia Menggunakan Algoritma Regresi ini. Pada tahap ini juga data yang akan 
saya gunakan juga akan diminimalisasi dan dioptimalkan dengan tujuan 
mempermudah projek ini untuk mencapa hasilnya dan di tahap ini juga saya akan 
menganalisa data yang akan dipakai dari segi kualitasnya.

1. Import Libraries yang diperlukan di dalam project
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Datex1.png)

2. Identifikasi isi dari dataset yang dimiliki
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Datex2.png)

### B. Data Preprocessing
Di dalam tahap Data Preprocessing, data akan dilatih dan akan dilakukan 
pengetesan terhadap data agar dapat digunakan untuk pembuatan model. Sebelum 
melakukan pelatihan data atau Data Training, data akan sebelumnya di cek terlebih 
dahulu kekosongan data yang ada atau bisa disebut juga proses Data Cleaning.

1. Saya mengubah format dari kolom date agar bisa dengan mudah mengakses index per index
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec1.png)

2. Saya menghapus duplikat data yang ada agar pemodelan bisa berjalan dengan baik nantinya
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec2.png)

3. Disini juga saya menyortir data berdasarkan kolom lokasi dari depan tetapi tidak untuk lokasi Indonesia
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec3.png)

4. Saya juga menyempatkan untuk melihat data yang telah disortir
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec4.png)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec4_.png)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec5.png)

5. Melakukan duplikasi dataframe dari 5 provinsi teratas agar bisa dilakukan percobaan
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec6.png)

6. Perbadingan antara beberapa provinsi
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec7.png)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec8.png)

7. Korelasi antara kolom dari skala 0 sampai 1 (semakin tinggi semakin bagus)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec9.png)

8. Membuat dataframe baru yang berisikan kolom-kolom yang akan dipakai
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec10.png)


### C. Model Training
Dalam tahap Training Model, ada beberapa proses yang akan dilakukan seperti 
memisahkan data yang akan digunakan untuk training atau pelatihan dan untuk 
testing atau pengetesan, menyiapkan model regresi yang akan digunakan. Setelah 
itu, dilanjutkan dengan menyiapkan model dengan menggunakan pipeline yang 
berfungsi untuk mempermudah menggabunggkan beberapa algoritma dalam satu 
pipeline. Lalu akhirnya dilakukan pengetesan model.

1. Linear Regression
Memasukkan data x dan y yang dimana x berisi data-data kolom yang akan diprediksikan menurut variabel y. Lalu memisahkan data yang akan dilatih dan yang akan diuji, tidak lupa memakai library pipeline dikarenakan terdapat pada variabel x yang memiliki lebih dari satu kolom data sehingga pipeline berfungsi untuk menggabungkan beberapa langkah pemrosesan agar lebih mudah. 
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Motra1.png)

2. Grafik Prediksi Linear Regression
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Motra2.png)

3. SVR (Support Vector Regression)
Karena menggunakan pipeline sehingga untuk pemrosesan algoritma lainnya dipermudah
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Motra3.png)

4. Grafik Prediksi SVR
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Motra4.png)


### D. Model Visualization and Evaluation
Model Visualization and Evaluation adalah tahap yang dimana sesuai dengan 
Namanya yaitu memvisualisasikan model yang telah di training dan melakukan 
evaluasi terhadap beberapa algoritma yang paling optimal.

1. Pembuatan fungsi cross validation, evaluate (mae, mse, rmse, r2 score), dan display hasil evaluate
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev1.png)

2. Hasil evaluasi SVR
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev2.png)

3. Hasil evaluasi Lasso Regression
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev3.png)

4. Hasil Evaluasi Random Forest Regression
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev4.png)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Dapec6.png)

6. Hasil perbandingan algoritma regresi
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev5.png)
![image](https://github.com/Batax093/Capstone_Project/blob/main/Dokumentasi/Modev6.png)

### E. Kesimpulan
1. Mean Absolute Error (MAE) adalah metrik yang mengukur rata-rata kesalahan 
prediksi model dalam satuan yang sama dengan variabel dependen. Semakin 
rendah MAE, semakin baik modelnya dalam melakukan prediksi. Dalam hal 
ini, "Random Forest Regression" memiliki MAE yang paling rendah 
(3.070987), menunjukkan bahwa model ini memiliki kinerja yang baik dalam 
membuat prediksi yang mendekati nilai sebenarnya.
2. Mean Squared Error (MSE) adalah metrik yang mengukur rata-rata dari 
kuadrat kesalahan prediksi. Semakin rendah MSE, semakin baik modelnya 
dalam membuat prediksi yang mendekati nilai sebenarnya. Dalam hal ini, 
"Random Forest Regression" juga memiliki MSE yang paling rendah 
(183.158492).
3. Root Mean Squared Error (RMSE) adalah akar kuadrat dari MSE dan 
mengukur kesalahan prediksi dalam satuan yang sama dengan variabel 
dependen. Seperti sebelumnya, semakin rendah RMSE, semakin baik 
modelnya dalam membuat prediksi yang mendekati nilai sebenarnya. "Random 
Forest Regression" memiliki RMSE yang paling rendah (13.533606).
4. R-squared (R2) Square adalah metrik yang mengukur seberapa baik model 
cocok dengan data. Nilai R2 berkisar dari 0 hingga 1, dan semakin mendekati 
1, semakin baik modelnya dalam menjelaskan variasi dalam data. Dalam hal 
ini, "Random Forest Regression" memiliki R2 yang paling tinggi (0.960372), 
menunjukkan bahwa model ini memiliki kemampuan yang baik dalam 
menjelaskan variasi dalam data.
5. Cross Validation adalah metode untuk mengukur kinerja model dengan 
menggunakan validasi silang. Nilai negatif pada kolom "Cross Validation" 
mungkin menunjukkan bahwa model-model ini mungkin mengalami 
overfitting atau masalah lainnya, terutama pada model "Linear Regression," 
"Lasso Regression," dan "Random Forest Regression." Nilai yang negatif 
biasanya tidak diinginkan dalam validasi silang, dan ini bisa menjadi indikasi 
bahwa model-model ini perlu disesuaikan lebih lanjut.

Dari pemodelan yang dibuat, tampaknya "Random Forest Regression" adalah 
model yang paling baik dalam hal kinerja berdasarkan beberapa metrik yang 
diberikan, seperti MAE, MSE, RMSE, dan R2 Square.
