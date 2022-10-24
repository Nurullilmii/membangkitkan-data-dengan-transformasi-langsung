# Membangkitkan-Data-dengan-Transformasi-Langsung

  Membangkitkan bilangan acak merupakan metode yang terdapat dalam komputasi statistika, khususnya simulasi komputer. Bilangan acak yang dibangkitkan bersifat pseudorandom (acak yang semua). Sebutan lainnya adalah PNG atau pseudorandom number generation adalah algoritma yang membangkitkan sederet bilangan acak yang sifatnya tidak benar-benar acak. (Ramadhan,2011).
  
  Karena pada dasarnya bilangan tersebut bukan bilangan acak yang sesungguhnya, maka untuk menyerupai bilangan acak, Paul Coddington dalam Monte Carlo Simulation for Statistical Physics mengatakan bahwa syarat penting yang harus dipenuhi oleh bilangan acak adalah dapat diulang, keacakan, periode panjang dan tidak peka seed. Salah satu metode membangkitkan bilangan acak adalah dengan transformasi langsung. Terdapat beberapa jenis membangkitkan data dengan transformasi langsung diantaranya adalah dari distirbusi Normal, keluarga distribusi gamma, t, F, normal nivariat dan normal multivariat.( I Made Tirta,2003). Semua metode pembangkitkan bilangan acak tergantung dari pembangkitan bilangan acak uniform. 
	
  Pada pembahasan kali ini yang akan kita lakukan adalah membangkitkan data dari G (α, β). Salah satu keluarga distribusi gamma yang dapat dibangkitkan dari distribusi normal adalah χ2. Distribusi normal standar dapat ditransformasikan menjadi distribusi χ2 dengan transformasi kuadrat. Jika Z~N (0,1) , maka Y= Z2 berdistribusi χ21
	
  Selanjutnya jumlah beberapa χ2 yang saling independen akan menghasilkan χ2 dengan derajat kebebasan yang merupakan jumlah dari derajat kebebasan masing masing. Untuk membangkitkan data dari χ21 dapat dilakukan langkah-langkah berikut:
1.	Bangkitkan data dari Z~N (0,1) seperti algoritma sebelumnya;
2.	Tentukan Y= Z2
Maka, Y adalah data dari χ21.

#Langkah Analisis

untuk membangkitkan data dari   dapat dilakukan langkah-langkah berikut :
1.	Bangkitkan Z dari N (0,1) seperti pada algoritma yang telah dipelajari pada pertemuan sebelumnya.
2.	Tentukan Y = Z2

#Hasil Analisis

![image](https://user-images.githubusercontent.com/116244436/197428277-86de7133-3a73-4771-b2ef-cee143f1c1a6.png)

![image](https://user-images.githubusercontent.com/116244436/197428308-5165fe12-f311-4b3c-8f8d-576c9394fb26.png)

![image](https://user-images.githubusercontent.com/116244436/197428365-9de4617d-2412-4619-92ba-bdba5876f7c6.png)

![image](https://user-images.githubusercontent.com/116244436/197428402-b2278036-97eb-4cb8-b162-307a5d70461d.png)

![image](https://user-images.githubusercontent.com/116244436/197428434-f6578107-fe49-430b-b206-ef0e7d41f3e0.png)

#Pembahasan

  Dalam membangkitkan biilangan, terlihat pada syntax pertama sebelum mebangkitkan bilangan acak chi-square, terlebih dahulu harus membangkitkan bilangan dari distribusi normal, hal ini karena distribusi chi-square berasal dari Z2 oleh karena itu diawali dengan mebangkitkan Z, N(0,1). (I Made Tirta,2003). Setelah membangkitkan bilangan acak dari normal, variabel yang digunakan kemudian dipangkat 2 kan sehingga menjadi chi square. 
  
  Begitu pula untuk syntax kedua yang nilai m nya diganti menjadi 100 (2*n) yang pada akhirnya dipangkat 2 kan menjadi sebaran chi-square. Terlihat nilai i akan berjalan mulai dari 1 hingga 100 dengan rumus sebaran normal yang kemudian nilai i akan ditransformasi kedalam sum x atau total dari variabel x.
