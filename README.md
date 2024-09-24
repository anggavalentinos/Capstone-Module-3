# **CUSTOMER LIFETIME VALUE**

### **Contents**

1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

****
## **1. Business Problem Understanding**
### **1.1 Background**

Nilai seumur hidup pelanggan (customer lifetime value atau CLV) merupakan ukuran seberapa berharganya seorang pelanggan bagi perusahaan. Dari nilai ini, perusahaan dapat menentukan berapa besar laba yang diperoleh dari satu penumpang dan biaya yang dikeluarkan untuk memperoleh atau mempertahankan pelanggan baru. Angka ini cukup penting bagi perusahaan untuk mengetahui apakah perusahaan ingin menargetkan pemasaran kepada pelanggan yang berharga secara efektif dan bagaimana pelanggan perusahaan akan berubah di masa mendatang.


Pada kasus perusahaan asuransi, mengetahui besarnya CLV dapat membantu beberapa kinerja perusahaan, diantaranya :
* Marketing bisa menggunakan informasi CLV untuk menentukan mana customer yang kemungkinan jarang melakukan klaim dan membayar premi yang tinggi. Marketing dapat memilih customer yang menghasilkan keuntungan besar untuk perusahaan.
* Customer service bisa menentukan bagaimana metode yang tepat digunakan untuk tiap jenis customernya, sehingga tidak ada biaya yang tinggi digunakan kepada customer yang memiliki nilai CLV yang rendah,
* Bagian finance dan risk management dapat menghitung bagaimana seorang customer dapat memberikan keuntungan dan langkah yang perlu dilakukan ketika customer pergi.
  
## **1.2 Problem Statement**

Menghitung Customer Lifetime Value (CLV) dalam industri asuransi biasanya dilakukan dengan menganalisis riwayat pelanggan, termasuk premi yang dibayarkan, klaim yang diajukan, dan biaya operasional yang dikeluarkan perusahaan selama periode hubungan pelanggan dengan perusahaan. Namun, metode ini memerlukan waktu yang panjang karena bergantung pada data historis yang lengkap, sehingga sering kali hasilnya datang terlambat. Sebagai contoh, pada saat hasil perhitungan siap, perusahaan mungkin sudah kehilangan kesempatan untuk menawarkan perpanjangan polis atau menerapkan strategi pemasaran yang efektif.

Untuk mengatasi hal ini, diperlukan metode yang mampu memperkirakan CLV di masa depan. Dengan menggunakan model prediksi, perusahaan dapat menentukan lebih awal pelanggan mana yang cenderung memiliki nilai seumur hidup yang tinggi dan mana yang tidak. Informasi ini memungkinkan perusahaan untuk fokus pada kegiatan pemasaran yang lebih tepat sasaran, mengarahkan sumber daya pada pelanggan yang bernilai tinggi. Dengan demikian, perusahaan dapat meningkatkan efisiensi dan efektivitas operasionalnya, mengurangi pengeluaran untuk pemasaran pada pelanggan yang kurang potensial.

Namun, manfaat prediksi CLV hanya akan optimal jika model prediksinya akurat. Oleh karena itu, membangun model yang mampu memprediksi CLV dengan baik sangat penting agar strategi bisnis yang diambil dapat memberikan dampak positif dan meningkatkan profitabilitas perusahaan.

## **1.3 Goals**

Pemodelan regresi digunakan untuk memprediksi Customer Lifetime Value (CLV) berdasarkan variabel-variabel pelanggan asuransi. Dengan bantuan machine learning, model prediktif ini akan dibangun untuk memperkirakan CLV secara akurat. Dalam Capstone Project Modul 3, tujuan utamanya adalah mengembangkan model yang mampu mengestimasi CLV bagi pelanggan perusahaan asuransi, guna mendukung strategi bisnis yang lebih efektif dan efisien.


## **1.4 Analytic Approach**

1. Data Understanding (Pemahaman Data)
2. Explantory Data Analysis (EDA)
3. Feature Engineering (Rekayasa Fitur) jika dibutuhkan
4. Data Preprocessing (Pra-pemrosesan Data)
5. Modeling (Pemodelan)
6. Melakukan Hyperparameter Tuning pada model terpilih untuk mendapatkan hasil error yang lebih rendah.

## **1.5 Metric Evaluation**

Evaluasi metrik yang akan digunakan adalah RMSE, MAE, dan MAPE, di mana RMSE adalah nilai rataan akar kuadrat dari error, MAE adalah rataan nilai absolut dari error, sedangkan MAPE adalah rataan persentase error yang dihasilkan oleh model regresi. Semakin kecil nilai RMSE, MAE, dan MAPE yang dihasilkan, berarti model semakin akurat dalam memprediksi harga sewa sesuai dengan limitasi fitur yang digunakan. 

Selain itu, kita juga bisa menggunakan nilai R-squared atau adj. R-squared jika model yang nanti terpilih sebagai final model adalah model linear. Nilai R-squared digunakan untuk mengetahui seberapa baik model dapat merepresentasikan varians keseluruhan data. Semakin mendekati 1, maka semakin fit pula modelnya terhadap data observasi. Namun, metrik ini tidak valid untuk model non-linear.
