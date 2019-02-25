#  BULGULAR VE İRDELEMELER
\thispagestyle{empty}

## Ortahisar’ın Mimari Dil Analizi ve Biçim Grameri

Bu bölümde elde edilen rölöveler üzerinden yapılan analizler ve bunların CGA kodunun oluşturulmasındaki kullanımı anlatılmaktadır. CGA gramerinin oluşturulmasında sırasıyla;

- Taban alanları
- Kat sayıları ve yükseklikleri
- Cephe karakteri
- Cephe çıkmaları (cumbalar)
- Cephe elemanları
- Pencere oranları
- Çatı formu

analiz edilerek incelenmiştir. Bu analizlere ek olarak yapıların kütlesel formları gruplanarak analiz edilmiştir. Ardından bu formları ve türevlerini oluşturabilecek biçim grameri kuralları tanımlanmıştır. Bu kurallar CGA gramerine entegre edilerek kaba kütle üretimi sağlanmaya çalışılmıştır. 

Oluşturulan kütleler kat sayıları ve yükseklik oranlarına göre dilimlenerek katlar oluşturulmaktadır. Cephe karakteri analizi sonucunda ise oluşan katların panel parçalarına ayrılması sağlanmaktadır. Ardından cephe elemanları ve pencereler oranlarına göre panel içinde dilimlenerek yerleri belli edilmektedir. 

### Yapı Taban Alanı Analizi

Seçilen Ortahisar evlerinin taban alanları, derinlikleri, genişlikleri incelendiğinde 

- En küçük yapı taban alanı : 50,38 m^2^
- En büyük yapı taban alanı : 315,67 m^2^ 
- En kısa kenar uzunluğu : 4,888 m
- En uzun kenar uzunluğu : 17,021 m
- Plan derinliğinin genişliğine oranının en küçük değeri 0,346 en büyük değeri 1,513

oldukları bulunmuştur. Bulunan değerler yazılıma girdi olarak verilen taban alanlarının seçimi için kullanılmaktadır. Bu kısıtlar dışında olan girdilerde model oluşumu gerçekleşmeyecektir. Alt sınırlar için model oluşumu gerçekleşmemekteyken, üst sınırlar için parsel kullanım analizi yapılarak parsel içinde taban alanı oluşumu yaptırılması fikri değerlendirilecektir. 

Table: Seçilmiş Ortahisar evlerinin oturum alanları, ortalama derinlik ve ortalama genişlik değerleri tablosu. \label{EvlerAlanlarOrtalamalar}

| **Ada** | **Parsel** | **Ort. Derinlik** | **Ort. Genişlik** | **Der. / Gen.** | **Taban Alanı** | **Parsel Alanı** |
| ------: | ---------: | ----------------: | ----------------: | --------------: | --------------: | ---------------: |
| **110** |     **16** |           7,955 m |          12,628 m |           0,630 |     100,43 m^2^ |      191,09 m^2^ |
| **110** |     **23** |           5,012 m |          10,067 m |           0,498 |      50,38 m^2^ |       84,07 m^2^ |
| **110** |     **39** |          12,678 m |          16,048 m |           0,790 |     194,83 m^2^ |      890,45 m^2^ |
| **110** |     **41** |           8,528 m |          14,385 m |           0,593 |     117,90 m^2^ |      320,49 m^2^ |
| **110** |     **43** |          12,501 m |           8,320 m |           1,503 |     110,31 m^2^ |      124,59 m^2^ |
| **110** |     **44** |          10,284 m |           8,165 m |           1,259 |      74,16 m^2^ |       45,80 m^2^ |
| **110** |    **131** |           6,670 m |          13,247 m |           0,503 |      93,91 m^2^ |    1.639,41 m^2^ |
| **114** |     **30** |          10,975 m |           7,255 m |           1,513 |     100,23 m^2^ |      131,28 m^2^ |
| **118** |      **1** |           9,208 m |          14,904 m |           0,618 |     137,30 m^2^ |      177,17 m^2^ |
| **127** |     **28** |           8,473 m |           9,799 m |           0,865 |      83,43 m^2^ |      205,86 m^2^ |
| **128** |      **7** |           8,473 m |          10,102 m |           0,839 |      92,20 m^2^ |      180,38 m^2^ |
| **128** |     **10** |           4,888 m |          14,111 m |           0,346 |      61,41 m^2^ |      102,06 m^2^ |
| **129** |     **26** |          16,493 m |          15,992 m |           1,031 |     242,79 m^2^ |      203,24 m^2^ |
| **888** |      **7** |          15,746 m |          12,945 m |           1,216 |     199,34 m^2^ |      603,81 m^2^ |
| **888** |      **8** |          14,998 m |          17,021 m |           0,881 |     315,67 m^2^ |      879,21 m^2^ |

### Yapı Kat Sayısı ve Yükseklikleri Analizi

![Ortahisar evlerinin kat sayısına göre gruplandırılması. \label{katgruplama}](source/figures/katgruplandirma.pdf){width=100%}

Tablolar incelendiğinde katlarına göre %20'si iki katlı, %6,67'i çatı katı olan iki katlı, %26,66'sı üç katlı, %33,33'ü çatı katı olan üç katlı ve %13,33'u dört katlı olan yapılar bulunmaktadır. Yapılar bodrum, zemin, birinci, ikinci ve çatı katlarından oluşmaktadır. Tablo \ref{katbulunmayuzde} incelendiğinde dört katlı yapılarda çatı katı oluşumu görülmemektedir. Üç katlı ve çatı katı bulunan yapıların %80'inde bodrum katı bulunurken %20'sinde bodrum kat yerine ikinci kat bulunmaktadır. Üç katlı yapıların yarısında bodrum kat bulunurken diğer yarısında bodrum kat yerine ikinci kat bulunmaktadır. 

Tablo \ref{katoranlari} incelendiğinde yapıların bodrum kat zemin kat yüksekliklerine göre daha kısa olduğu, birinci ve ikinci kat yüksekliklerinin ise yakın değerler aldığı görülmektedir. Çatı katı yükseklikleri yapıların 2/3'ünde zemin kata yakın değerler alırken geri kalanında zemin kattan daha kısa olarak bulunmaktadır.

Table: Kat yükseklikleri tablosu.

| **Ada** | **Parsel** | **Bodrum Kat** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | --------------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |        2,369 m |       3,733 m |         3,318 m |        3,760 m |               |
| **128** |     **10** |        2,441 m |       4,046 m |         3,247 m |        3,239 m |               |
| **110** |     **16** |        3,242 m |       3,706 m |         4,021 m |                |       3,325 m |
| **110** |     **39** |        1,935 m |       4,180 m |         4,093 m |                |       2,402 m |
| **110** |     **41** |        1,823 m |       3,693 m |         4,083 m |                |       2,334 m |
| **110** |    **131** |                |       2,766 m |         3,229 m |        3,348 m |       2,547 m |
| **129** |     **26** |        2,002 m |       3,443 m |         3,226 m |                |       3,258 m |
| **110** |     **44** |        2,783 m |       4,663 m |         2,933 m |        2,913 m |               |
| **114** |     **30** |        2,946 m |       3,524 m |         3,252 m |                |               |
| **128** |      **7** |        2,431 m |       4,057 m |         3,807 m |                |               |
| **888** |      **8** |                |       4,227 m |         4,065 m |        4,595 m |               |
| **127** |     **28** |                |       2,897 m |         3,840 m |                |       2,871 m |
| **110** |     **23** |        1,752 m |       3,112 m |         3,189 m |                |               |
| **110** |     **43** |                |       4,305 m |         4,147 m |                |               |
| **888** |      **7** |                |       4,682 m |         3,828 m |                |               |



Table: Kat sayısına göre gruplandırılmış kat oranları tablosu. \label{katoranlari}

|         | **Ada** | **Parsel** | **Zemin Kat** | **Bodrum K. / Zemin K.** | **Birinci K. / Zemin K.** | **İkinci K. / Zemin K.** | **Çatı K. / Zemin K.** |
| -- | ----: | ----: | -----------------: | -----------------: | ------------------: | -----------------: | ---------------: |
| **4**   |         |            |               |                          |                           |                          |                        |
|         | **118** |      **1** |       3,733 m |                    0,635 |                     0,889 |                    1,007 |                        |
|         | **128** |     **10** |       4,046 m |                    0,603 |                     0,802 |                    0,801 |                        |
| **3,5** |         |            |               |                          |                           |                          |                        |
|         | **110** |     **16** |       3,706 m |                    0,875 |                     1,085 |                          |                  0,897 |
|         | **110** |     **39** |       4,180 m |                    0,463 |                     0,979 |                          |                  0,575 |
|         | **110** |     **41** |       3,693 m |                    0,494 |                     1,106 |                          |                  0,632 |
|         | **110** |    **131** |       2,766 m |                          |                     1,167 |                    1,210 |                  0,921 |
|         | **129** |     **26** |       3,443 m |                    0,581 |                     0,937 |                          |                  0,946 |
| **3**   |         |            |               |                          |                           |                          |                        |
|         | **110** |     **44** |       4,663 m |                          |                     0,629 |                    0,625 |                        |
|         | **114** |     **30** |       3,524 m |                    0,836 |                     0,923 |  |                        |
|         | **128** |      **7** |       4,057 m |                    0,599 |                     0,938 |                          |                        |
|         | **888** |      **8** |       4,227 m |                          |                     0,962 |                    1,087 |                        |
| **2,5** |         |            |               |                          |                           |                          |                        |
|         | **127** |     **28** |       2,897 m |                          |                     1,325 |                          |                  0,991 |
| **2**   |         |            |               |                          |                           |                          |                        |
|         | **110** |     **23** |       3,112 m |                    0,563 |                     1,025 |                          |                        |
|         | **110** |     **43** |       4,305 m |                          |                     0,963 |                          |                        |
|         | **888** |      **7** |       4,682 m |                          |                     0,818 |                          |                        |

Table: Kat sayısına göre gruplandırılmış yapılarda katların bulunma yüzdeleri tablosu. \label{katbulunmayuzde}

| **Kat Sayısı** | **Bodrum Kat** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| -------------: | -------------: | ------------: | --------------: | -------------: | ------------: |
|          **4** |            100 |           100 |             100 |            100 |             0 |
|        **3,5** |             80 |           100 |             100 |             20 |           100 |
|          **3** |             50 |           100 |             100 |             50 |             0 |
|        **2,5** |              0 |           100 |             100 |              0 |           100 |
|          **2** |             33 |           100 |             100 |              0 |             0 |

<!-- 110-23 2,5 katlı olarak değerlendirilebilir.-->

\newpage

### Cephe Analizi

![Ortahisar evlerinin cephe kurgusuna göre gruplandırılması. Sol tarafta 3 parçalı ve sağ tarafta 1 parçalı cephe düzenleri. \label{cephegruplama}](source/figures/cephegruplandirma.pdf){width=85%}

\newpage

Yapılar cephelerine göre gruplandığında 100 m^2^ üzerinde olanlar üç parçalı cepheye, 100 m^2^ altında olan yapıların 75%'i üç parçalı ve geri kalanı tek parçalı cepheye sahiptirler. Üç parçalı cephelerde kenar parçalarının genişlikleri bir kaç santimetre farklarla birbirlerinden farklılaşmaktadır. Bu cephe parçalarının orta cephe parçasına göre oranı yapılarda 0,9 ile 1,165 arasında değişmektedir.

Table: Ortahisar evlerinin cephe parçalarının genişlik oranları analizi tablosu.

|           | **Ada** | **Parsel** | **Bay Sol** | **Bay Orta** | **Bay Sağ** | **Sol / Orta** | **Sağ / Orta** |
| --------- | ------: | ---------: | ----------: | -----------: | ----------: | -------------: | -------------: |
| **3 Bay** |         |            |             |              |             |                |                |
|           | **118** |      **1** |     5,180 m |      4,480 m |     5,220 m |          1,156 |          1,165 |
|           | **128** |     **10** |     4,580 m |      4,740 m |     4,600 m |          0,966 |          0,970 |
|           | **110** |     **16** |     4,280 m |      4,710 m |     4,420 m |          0,909 |          0,938 |
|           | **110** |     **39** |     5,230 m |      4,960 m |     5,320 m |          1,054 |          1,073 |
|           | **110** |     **41** |     5,360 m |      3,750 m |     5,320 m |          1,429 |          1,419 |
|           | **110** |    **131** |     4,470 m |      4,090 m |     4,680 m |          1,093 |          1,144 |
|           | **129** |     **26** |     5,020 m |      5,340 m |     4,960 m |          0,940 |          0,929 |
|           | **888** |      **8** |     6,420 m |      6,160 m |     6,480 m |          1,042 |          1,052 |
|           | **127** |     **28** |     3,370 m |      3,110 m |     3,260 m |          1,084 |          1,048 |
|           | **110** |     **23** |     3,470 m |      2,990 m |     3,600 m |          1,161 |          1,204 |
|           | **110** |     **43** |     3,960 m |      3,960 m |     3,960 m |          1,000 |          1,000 |
|           | **888** |      **7** |     5,220 m |      3,550 m |     4,660 m |          1,470 |          1,313 |
| **1 Bay** |         |            |             |              |             |                |                |
|           | **110** |     **44** |     7,160 m |              |             |                |                |
|           | **114** |     **30** |     8,850 m |              |             |                |                |
|           | **128** |      **7** |     9,930 m |              |             |                |                |

Table: Sol ve sağ cephe parçalarındaki pencere sayılarının tablosu. 

|           | **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| --------- | ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **3 Bay** |         |            |               |                 |                |               |
|           | **118** |      **1** |             2 |               3 |              3 |               |
|           | **128** |     **10** |             1 |               1 |              1 |               |
|           | **110** |     **16** |             2 |               2 |                |             3 |
|           | **110** |     **39** |             2 |               2 |                |             2 |
|           | **110** |     **41** |             2 |               2 |                |             2 |
|           | **110** |    **131** |             3 |               3 |              3 |             2 |
|           | **129** |     **26** |             2 |               2 |                |             3 |
|           | **888** |      **8** |             3 |               3 |              3 |               |
|           | **127** |     **28** |             2 |               1 |                |             1 |
|           | **110** |     **23** |             1 |               1 |                |               |
|           | **110** |     **43** |             1 |               2 |                |               |
|           | **888** |      **7** |             1 |               3 |                |               |



Table: Orta cephe parçalarındaki pencere sayılarının tablosu. Tek parçalı cepheye sahip evler bu tabloda gösterilmiştir.

|           | **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| --------- | ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **3 Bay** |         |            |               |                 |                |               |
|           | **118** |      **1** |         Giriş |               3 |              3 |               |
|           | **128** |     **10** |         Giriş |               1 |              1 |               |
|           | **110** |     **16** |             2 |               2 |                |             3 |
|           | **110** |     **39** |         Giriş |   Kapalı balkon |                |             2 |
|           | **110** |     **41** |         Giriş |               2 |                |             2 |
|           | **110** |    **131** |         Giriş |               2 |              2 |             2 |
|           | **129** |     **26** |             3 |               3 |                |             3 |
|           | **888** |      **8** |         Giriş |               2 |              2 |               |
|           | **127** |     **28** |         Giriş |               2 |                |             2 |
|           | **110** |     **23** |         Giriş |               1 |                |               |
|           | **110** |     **43** |             1 |               2 |                |               |
|           | **888** |      **7** |         Giriş |               2 |                |               |
| **1 Bay** |         |            |               |                 |                |               |
|           | **110** |     **44** |             2 |               5 |              5 |               |
|           | **114** |     **30** |             6 |               6 |                |               |
|           | **128** |      **7** |             4 |               4 |                |               |

\newpage
### Cephe Çıkmaları Analizi (Cumba)

Genel olarak yapıların %43,75'inde cumba bulunmaktadır. Üç parçalı cephe karakteri gösteren yapılarda cumbası olan orta parça genişliği en az 2,99 metredir. Çatı katı cumbaları bir alt katında bulunan cumbanın derinlik ve genişlik uzunluklarını almaktadırlar. Ayrıca bodrum katı olan yapılarda giriş sahanlığı birinci katta bulunan cumba mesafesi kadar dışarı çıkmaktadır. 110 ada 131 parsel ve 118 ada 1 parselde bulunan yapıların ikinci katları arka cepheleri harici diğer cephelerde dışarı çıkma yapmaktadır. Bu yapıların ikinci katlarında bulunan cumbalar bir alt kat cumbaya göre hem derinlik hemde genişlik olarak ikinci kattaki çıkma mesafesi kadar büyümektedir. 

Table: Cumbaların derinlik ölçüleri tablosu.

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |               |         1,900 m |        2,300 m |               |
| **128** |     **10** |               |         1,460 m |        1,460 m |               |
| **110** |     **16** |               |                 |                |               |
| **110** |     **39** |       1,840 m |         1,840 m |                |               |
| **110** |     **41** |               |         1,780 m |                |       1,780 m |
| **110** |    **131** |               |         3,220 m |        3,450 m |       3,450 m |
| **129** |     **26** |               |                 |                |               |
| **110** |     **44** |               |                 |                |               |
| **114** |     **30** |               |                 |                |               |
| **128** |      **7** |               |                 |                |               |
| **888** |      **8** |               |                 |                |               |
| **127** |     **28** |               |         1,210 m |                |       1,210 m |
| **110** |     **23** |               |         1,250 m |                |               |
| **110** |     **43** |               |                 |                |               |
| **888** |      **7** |               |                 |                |               |

###  Cephe Elemanları Analizi

Yapılarda bulunan kornişlerin ve köşe taşlarının ebatlarının analizleri eklenecektir.

<!-- 

### Yapı Kademelenmesi Analizi

118-1 ve 110-131 de ikinci katın dışarı taşmaları ele alınmalı. 110-39 ve 110-131 deki çatı katı oluşumu incelenmeli. 
-->

### Pencere Genişlikleri ve Yükseklikleri Analizi

Yapıların %81,25 inde cephe parçalarında iki veya daha fazla pencere bulunurken geri kalanında tek pencere bulunmaktadır. Cephe parçalarında iki veya daha fazla pencere bulunan yapılarda pencere yüksekliğinin genişliğine oranı 1,493 ile 1,881 arasında değişmektedir. Cephe parçasında tek pencere bulunan yapılarda bu oran 0,854 ile 1,050 arasındadır. Pencere yüksekliklerinin zemin kat yüksekliğine göre oranlarına bakıldığında ise 1,439 - 2,378 değer aralığı bulunmaktadır. 110 ada 44 parseldeki yapının zemin katı diğer yapılara göre farklılık gösterdiğinden bu değer aralığı dışında tutulmuştur.

Table: Pencere yüksekliklerinin genişliklerine göre oranları tablosu.

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |         1,881 |           1,579 |          1,579 |               |
| **128** |     **10** |         0,854 |           0,854 |          0,827 |               |
| **110** |     **16** |         1,520 |           1,667 |                |         1,722 |
| **110** |     **39** |         1,605 |           1,618 |                |         1,076 |
| **110** |     **41** |         1,772 |           1,805 |                |         1,341 |
| **110** |    **131** |         1,811 |           1,755 |          1,755 |         1,600 |
| **129** |     **26** |         1,595 |           1,595 |                |         1,595 |
| **110** |     **44** |               |           1,842 |          1,861 |               |
| **114** |     **30** |         1,705 |           1,705 |                |               |
| **128** |      **7** |         1,493 |           1,585 |                |               |
| **888** |      **8** |         1,736 |           1,836 |          1,860 |               |
| **127** |     **28** |         1,050 |           1,792 |                |         0,653 |
| **110** |     **23** |         0,991 |           1,031 |                |               |
| **110** |     **43** |               |           1,860 |                |               |
| **888** |      **7** |         1,550 |           1,827 |                |               |


Table: Kat yüksekliklerinin pencere yüksekliklerine göre oranları tablosu.

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |         1,645 |           1,550 |          1,757 |               |
| **128** |     **10** |         2,152 |           1,727 |          1,780 |               |
| **110** |     **16** |         1,626 |           1,608 |                |         1,630 |
| **110** |     **39** |         1,659 |           1,611 |                |         1,953 |
| **110** |     **41** |         1,694 |           1,839 |                |         1,415 |
| **110** |    **131** |         1,608 |           1,673 |          1,735 |         1,675 |
| **129** |     **26** |         1,439 |           1,348 |                |         1,362 |
| **110** |     **44** |         2,970 |           1,577 |          1,549 |               |
| **114** |     **30** |         1,602 |           1,478 |                |               |
| **128** |      **7** |         1,861 |           1,511 |                |               |
| **888** |      **8** |         1,691 |           1,715 |          1,795 |               |
| **127** |     **28** |         1,123 |           1,607 |                |         1,806 |
| **110** |     **23** |         1,454 |           1,490 |                |               |
| **110** |     **43** |         1,538 |           1,700 |                |               |
| **888** |      **7** |         2,378 |           1,903 |                |               |



Table: Pencere denizlik yüksekliklerinin tablosu.

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |       0,497 m |         0,751 m |        0,741 m |               |
| **128** |     **10** |       1,101 m |         0,677 m |        0,698 m |               |
| **110** |     **16** |       0,603 m |         0,847 m |                |       0,688 m |
| **110** |     **39** |       0,635 m |         0,656 m |                |       1,016 m |
| **110** |     **41** |       0,550 m |         0,868 m |                |       0,550 m |
| **110** |    **131** |       0,698 m |         0,700 m |        0,635 m |       0,677 m |
| **129** |     **26** |       0,529 m |         0,402 m |        0,402 m |       0,402 m |
| **110** |     **44** |       0,656 m |         0,592 m |        0,508 m |               |
| **114** |     **30** |       0,529 m |         0,614 m |                |               |
| **128** |      **7** |       0,741 m |         0,614 m |                |               |
| **888** |      **8** |       1,037 m |         0,847 m |        0,847 m |               |
| **127** |     **28** |       0,254 m |         0,677 m |                |       0,804 m |
| **110** |     **23** |       0,614 m |         0,614 m |                |               |
| **110** |     **43** |       0,571 m |         0,783 m |                |               |
| **888** |      **7** |       1,757 m |         0,804 m |                |               |



### Çatı Formu ve Eğimi Analizi

Ortahisar evlerinin çatı eğimleri 17° ile 34° arasında değişmektedir. Çatı katı olmayan yapılar %77.7'si kırma çatıya %11,1'i beşik çatı ve geri kalanı kırma ve beşik melez bir çatıya sahiptir. Çatı katı olan yapılarda alt kat çatısı eşit oranlarda kırma, beşik ve melez çatıya sahiptir. Çatı katı olan yapıların çatı katı %16,6'sı kırma, %66,6 beşik ve %16,6'sı melez çatıya sahiptir. CityEngine üzerinde CGA kodu ile melez çatı oluşturulması mümkün olmamaktadır.

Table: Ortahisar evlerinin çatı formu ve eğimi tablosu.

| **Ada** | **Parsel** | **Çatı Eğimi** | **Alt Kat** | **Çatı Kat**  |
| ------: | ---------: | -------------: | ----------- | ------------- |
| **118** |      **1** |            20° | Kırma       |               |
| **128** |     **10** |            20° | Beşik       |               |
| **110** |     **16** |            23° | Beşik+Kırma | Kırma         |
| **110** |     **39** |            18° | Kırma       | Beşik         |
| **110** |     **41** |            18° | Beşik       | Beşik + Kırma |
| **110** |    **131** |            18° | Kırma       | Beşik         |
| **129** |     **26** |            19° | Beşik+Kırma | Beşik         |
| **110** |     **44** |            18° | Kırma       |               |
| **114** |     **30** |            17° | Kırma       |               |
| **128** |      **7** |            20° | Kırma       |               |
| **888** |      **8** |            18° | Kırma       |               |
| **127** |     **28** |            34° | Beşik       | Beşik         |
| **110** |     **23** |            28° | Kırma       |               |
| **110** |     **43** |            30° | Beşik+Kırma |               |
| **888** |      **7** |            18° | Kırma       |               |

### Form Analizi

![Ortahisar evlerinin kat sayısına göre kütle oluşumlarının analizi. \label{katgruplama}](source/figures/kutlegrameri.pdf){width=90%}

\newpage

### Biçim Grameri

![Ortahisar evlerinin kütlesel biçim grameri dili. \label{bicimgrameri}](source/figures/bicimgrameri.pdf){width=100%}



## CGA Biçim Gramerinin Oluşturulması

CGA gramer kodu CityEngine yazılımında yazılmaya başlanmıştır ve büyük oranda tamamlanmıştır.  

![CityEngine üzerinde CGA kodu ile üreliten modeller.](source/figures/OrtahisarCGA.png){width=100%}



\newpage