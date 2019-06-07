# BULGULAR VE İRDELEMELER

\thispagestyle{empty}

Bu bölümde elde edilen rölöveler üzerinden yapılan analizler ve bunların CGA kodunun oluşturulmasındaki kullanımı anlatılmaktadır. CGA gramerinin oluşturulmasında sırasıyla;

- Taban alanları
- Kat sayıları ve yükseklikleri
- Cephe tipi
- Cephe çıkmaları
- Cephe elemanları
- Çatı formu

analiz edilerek incelenmiştir. Bu analizlere ek olarak yapıların kütlesel formları gruplanarak analiz edilmiştir. Ardından bu formları ve türevlerini oluşturabilecek biçim grameri kuralları tanımlanmıştır. Bu kurallar CGA gramerine entegre edilerek kaba kütle üretimi sağlanmaya çalışılmıştır.

Oluşturulan kütleler kat sayıları ve yükseklik oranlarına göre dilimlenerek katlar oluşturulmaktadır. Cephe karakteri analizi sonucunda ise oluşan katların panel parçalarına ayrılması sağlanmaktadır. Ardından cephe elemanları ve pencereler oranlarına göre panel içinde dilimlenerek yerleri belli edilmektedir.

## Ortahisar’ın Mimari Dil Analizi ve Biçim Grameri

Gramer kuralları iki boyutlu bina oturum alanı ve üç boyutlu bloklardan oluşmaktadır. Üç boyutlu bloklar kütlesel hacimlere karşılık gelmekte ve analiz-sentez aşaması sonucunda elde edilen veriler ile parametreleştirilmektedir. CGA gramerinin başlangıcı bir parsel veya bina oturum alanının tanımlanması ile gerçekleşmektedir. Gramerin basitleştirilmesi açısından parametre değer verileri ayrıca tablolar ile açıklanmıştır.

<!-- GRAMER İLE İLGİLİ GENEL NOTLAR BU KISIMA EKLENECEKTİR-->

***Çalışmanın amacı geleneksel konutların oranlarını üretebilen tasarım altlığı oluşturabilmek olduğu için cephelerdeki düzensizlikler göz ardı edilmiştir. Amaç birebir varolan yapıları üretmek değil onların oranlarını gösteren modeller üretebilmektir.***

***Analiz edilen yapıların kendi içlerinde ve birbirleri ile karşılaştırılan yükseklik değerleri arasında bir korelasyon bulunamadığından yükseklikler zemin kat yüksekliği sabit alınarak orantılanmıştır. Karşılaştırma tabloları ekler bölümünde yer almaktadır.***

### Yapı Taban Alanı

Ortahisar geleneksel evleri sokağa göre paralel konumlanmaktadır. Yapıların giriş ve kapalı çıkmasının bulunduğu cephe sokağa doğru bakmaktadır. Kural 1 ve 2 başlangıç için verilen oturum alanını ve sokağın yönünü belirler (Şekil \ref{K1K2}). Kural 1 herhangi bir alanın bir noktasında oturum alanını konumlandırmak için kullanabileceğinden alan planlamasını mümkün kılmaktadır.

![Oturum alanı ve sokak yönünün tanımlanmasını gösteren kurallar. \label{K1K2}](source/figures/K1-K2.pdf){width=100%}

Seçilen Ortahisar evlerinin taban alanları incelendiğinde;

- En küçük yapı taban alanı : 50,38 m^2^
- En büyük yapı taban alanı : 315,67 m^2^
- En kısa kenar uzunluğu : 4,888 m
- En uzun kenar uzunluğu : 17,021 m
- Plan derinliğinin genişliğine oranının en küçük değeri 0,346 en büyük değeri 1,513

oldukları bulunmuştur. Bulunan değerler CGA gramerine girdi olarak verilen taban alanlarının seçimi için kullanılmaktadır. Bu kısıtlar dışında olan girdilerde model oluşumu gerçekleşmemektir. <!-- Alt sınırlar için model oluşumu gerçekleşmemekteyken, üst sınırlar için parsel kullanım analizi yapılarak parsel içinde taban alanı oluşumu yaptırılması fikri değerlendirilecektir. -->
\newpage

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

Seçilmiş geleneksel konutlar kat sayısına göre iki katlı, çatı katı olan iki katlı, üç katlı, çatı katı olan üç katlı ve dört katlı yapılar olarak beş gruba ayrılmaktadırlar. Çatı katları yarım kat olarak hesap edilerek şekil \ref{katgruplama}'de gösterilmiştir. Analiz edilen yapıların katlarına göre yüzdelerine bakıldığında %13,34'ü iki katlı, %6,67'sı çatı katı olan iki katlı, %33,34'sı üç katlı, %33,34'ü çatı katı olan üç katlı, %13,34'ü dört katlı yapılardır. Bu oranlar gramer içerisinde eğer kat sayısı tercihi yapılmaz ise oluşturulacak yapıların oluşturulma oranlarını belirtmektedir.

![Kat sayısına göre gruplandırılmış Ortahisar evleri. \label{katgruplama}](source/figures/katgruplandirma.pdf){width=100%}

<!-- TODO: Zemin katın K6 daki gibi alt tarafına eklenme yapılmayacağına dair bir kural eklenmeli midir? -->

Tablo \ref{katbulunmayuzde}'de yapı tipini belirleyen katların bulunma yüzdeleri gösterilmiştir. Analiz edilen Ortahisar evlerinin hepsinde zemin ve birinci kat bulunmaktadır. Buna ek olarak dört katlı yapılarda çatı katı oluşumu görülmemektedir. Üç katlı ve çatı katı bulunan yapıların %80'inde bodrum katı bulunurken %20'sinde bodrum kat yerine ikinci kat bulunmaktadır. Üç katlı yapıların %60'ında bodrum kat bulunurken %40'ında bodrum kat yerine ikinci kat bulunmaktadır. Bu değerler yapı tipinin hangi kat tipleri ile oluşacağını belirlemektedir.

Table: Kat sayısına göre gruplandırılmış yapılarda katların bulunma yüzdeleri tablosu. \label{katbulunmayuzde}

| **Kat Sayısı** | **Bodrum Kat** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| -------------: | -------------: | ------------: | --------------: | -------------: | ------------: |
|          **4** |            100 |           100 |             100 |            100 |             0 |
|        **3,5** |             80 |           100 |             100 |             20 |           100 |
|          **3** |             60 |           100 |             100 |             40 |             0 |
|        **2,5** |              0 |           100 |             100 |              0 |           100 |
|          **2** |              0 |           100 |             100 |              0 |             0 |

Oturum alanı ve sokak yönü ilk iki kural ile belirlendikten sonra bahsedilen oranlar ile beraber yapı tipi oluşturulmaktadır. Yapı  katlarının oluşumu K3'ten K9'a kadar olan gramer kuralları ile tanımlanmaktadır (Şekil \ref{K3K7}). Bütün Ortahisar geleneksel konutlarında zemin kat ve birinci kat bulunduğundan ötürü K4 kuralı yapılar için çekirdek birimi oluşturmaktadır. K6, K7 ve K8 de görülen koyu gri tarama mevcut katın üzerine tam kat gelemeyeceğini belirtmektedir. Katlar birbiri üzerine eklenirken dış sınırları aynı olacak şekilde kurallarda işlenmiştir. Sadece K8 kuralında, 110 ada 131 parsel ve 118 ada 1 parselde görüleceği üzere, diğer kurallardan ayrı olarak birinci katın üzerine gelen ikinci kat sınırları arka cephe kısmı hariç olmak üzere üç yandanda büyümektedir.

![Kat oluşumlarını gösteren gramer kuralları. \label{K3K7}](source/figures/K3-K8.pdf){width=100%}

<!-- CITY ENGINE Kurallarına bakarak yazı genişletilebilir -->
K3 kuralındaki hg yükseklik değeri yapı tipine göre en küçük ve en büyük yükseklikler arasından bir değer almaktadır. Örneğin iki katlı bir yapı tipi tablo \ref{katoranlari}'e bakılarak en küçük 4.305 ile en büyük 4.682 arasından bir değer verilerek zemin kat üretilmektedir. Diğer kurallardaki yükseklik parametreleri tablodaki yapı tipine karşılık gelen en küçük ve en büyük oranlar arasından bir değer ile çarpılarak elde edilmektedir. Tablo \ref{katoranlari} incelendiğinde yapıların bodrum kat zemin kat yüksekliklerine göre daha kısa olduğu, birinci ve ikinci kat yüksekliklerinin ise yakın değerler aldığı görülmektedir. Yapılara ait gerçek kat yükseklikleri tablo \ref{katyukseklikleri}'te gösterilmiştir. ***Çatı katı üç parçalı cepheye sahip yapılarda görüldüğü ve kapalı çıkmalara göre biçimlendiği için cephe çıkmaları kurallarından sonra gerçekleşmektedir.***

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
|         | **110** |     **23** |       3,112 m |                    0,563 |                     1,025 |                          |                        |
|         | **110** |     **44** |       4,663 m |                          |                     0,629 |                    0,625 |                        |
|         | **114** |     **30** |       3,524 m |                    0,836 |                     0,923 |                          |                        |
|         | **128** |      **7** |       4,057 m |                    0,599 |                     0,938 |                          |                        |
|         | **888** |      **8** |       4,227 m |                          |                     0,962 |                    1,087 |                        |
| **2,5** |         |            |               |                          |                           |                          |                        |
|         | **127** |     **28** |       2,897 m |                          |                     1,325 |                          |                  0,991 |
| **2**   |         |            |               |                          |                           |                          |                        |
|         | **110** |     **43** |       4,305 m |                          |                     0,963 |                          |                        |
|         | **888** |      **7** |       4,682 m |                          |                     0,818 |                          |                        |

Table: Kat yükseklikleri tablosu. \label{katyukseklikleri}

| **Ada** | **Parsel** | **Bodrum Kat** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | --------------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |        2,369 m |       3,733 m |         3,318 m |        3,760 m |               |
| **128** |     **10** |        2,441 m |       4,046 m |         3,247 m |        3,239 m |               |
| **110** |     **16** |        3,242 m |       3,706 m |         4,021 m |                |       3,325 m |
| **110** |     **39** |        1,935 m |       4,180 m |         4,093 m |                |       2,402 m |
| **110** |     **41** |        1,823 m |       3,693 m |         4,083 m |                |       2,334 m |
| **110** |    **131** |                |       2,766 m |         3,229 m |        3,348 m |       2,547 m |
| **129** |     **26** |        2,002 m |       3,443 m |         3,226 m |                |       3,258 m |
| **110** |     **23** |        1,752 m |       3,112 m |         3,189 m |                |               |
| **110** |     **44** |        2,783 m |       4,663 m |         2,933 m |        2,913 m |               |
| **114** |     **30** |        2,946 m |       3,524 m |         3,252 m |                |               |
| **128** |      **7** |        2,431 m |       4,057 m |         3,807 m |                |               |
| **888** |      **8** |                |       4,227 m |         4,065 m |        4,595 m |               |
| **127** |     **28** |                |       2,897 m |         3,840 m |                |       2,871 m |
| **110** |     **43** |                |       4,305 m |         4,147 m |                |               |
| **888** |      **7** |                |       4,682 m |         3,828 m |                |               |

### Cephe Tipi Analizi

<!-- TODO: Yan cephe tipleri açıklanmalı. Cephe Panelleri kısmında da açıklanabilir.-->

İncelenen Ortahisar geleneksel dokusu üç parçalı ve tek parçalı cephesi olan yapılar olarak iki gruba ayrılmaktadır (Şekil \ref{cephegruplama}). ***Tek parçalı cepheye sahip yapılar şekil \ref{K24K27}'da tanımlanan cephe panelleri kuralları ile oluşumuna devam etmektedir.*** Üç parçalı cepheye sahip yapıların oluşumunu gösteren bölümlenme kuralları şekil \ref{K9K12}'te gösterilmiştir. Kurallardaki kesikli çizgiler bölümlenme hatlarını belirtmektedirler. Yapılar ön cephesinde gösterdiği üç veya tek parçalı cephe tipini arka cephesinde de göstermektedir. K9 kuralı zemin kattaki, K10  kuralı birinci kattaki cephe bölümlenmesini tanımlamaktadır. K11 üzerine tam kat gelmeyen birinci veya ikinci kat cephesinin bölümlenmesini tanımlamaktadır. K12 kuralı ise  bodrum kat cephesinin bölümlenmesini göstermektedir.

![Üç parçalı cephe tipi oluşumunu gösteren gramer kuralları. \label{K9K12}](source/figures/K9-K12.pdf){width=100%}

![Ortahisar evlerinin cephe kurgusuna göre gruplandırılması. Sol tarafta 3 parçalı ve sağ tarafta 1 parçalı cephe düzenleri. \label{cephegruplama}](source/figures/cephegruplandirma.pdf){width=85%}

Cephe tipini belirleyen bir başka koşul ise yapıların taban alanından gelmektedir. İncelenen yapıların taban alanı 100 m^2^ üzerinde olanlar üç parçalı cepheye, 100 m^2^ altında olan yapıların 75%'i üç parçalı ve geri kalanı tek parçalı cepheye sahip oldukları belirlenmiştir. Üç parçalı cephelerde sağ ve sol parçaların genişlikleri bir kaç santimetre farklarla birbirlerinden farklılaşmaktadır. Sağ ve sol cephe parçalarının orta cephe parçasına göre oranı yapılarda 0,909 ile 1,165 arasında değişmektedir (Tablo \ref{genislikoranlari}). Bu küçük ölçü farklarına rağmen bütün yapılar cephe merkezinden geçen zahiri aksa göre simetriktirler.

Table: Ortahisar evlerinin cephe parçalarının genişlik oranları analizi tablosu. \label{genislikoranlari}

|           | **Ada** | **Parsel** | **Sol** | **Orta** | **Sağ** | **Sol / Orta** | **Sağ / Orta** |
| --------- | ------: | ---------: | ----------: | -----------: | ----------: | -------------: | -------------: |
| **3 Parçalı** |         |            |             |              |             |                |                |
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
| **1 Parçalı** |         |            |             |              |             |                |                |
|           | **110** |     **44** |     7,160 m |              |             |                |                |
|           | **114** |     **30** |     8,850 m |              |             |                |                |
|           | **128** |      **7** |     9,930 m |              |             |                |                |

### Cephe Çıkmaları Analizi

İncelenen geleneksel dokuda açık ve kapalı çıkmalara rastlanmaktadır. Kapalı çıkmalar sokak yönünde ve ön cephede bulunmaktayken, açık çıkmalar arka cephede bulunmaktadır. Açık çıkmalar sadece kapalı çıkması ve çatı katı bulunan üç katlı (110 ada 39, 41 ve 131 parseller ile tanımlı) yapılarda görülmektedir. Bu yapılarda rastlanan açık çıkma derinliğinin kapalı çıkma derinliğine oranı %60'tır. 110 ada 39 parselde bulunan yapının ön cephesinin zemin katında birinci katındaki kapalı çıkması gibi bir çıkma bulunmaktadır, ancak bir rüzgarlık gibi işlevlenen bu eleman ön kısmı açık bulunduğundan dolayı bir kapalı çıkma olarak değerlendirilmemiştir.

Tek parçalı cepheye sahip yapılarda açık veya kapalı çıkmaya rastlanmamaktadır. Genel olarak yapıların %43,75'inde, sadece üç parçalı cepheye sahip olanların %58,33'ünde kapalı çıkma bulunmaktadır. Üç parçalı cephe karakteri gösteren yapılarda kapalı çıkması olan orta parça genişliği en az 2,99 metredir. Kapalı çıkmaların genişliğinin derinliğine oranı 2,107 ve 2,696 değişmekteyken, bir yapı bu oranın çok altında 1,270 değeri alırken bir yapı da çok üstünde kalarak 3,247 oranını almaktadır (Tablo \ref{CumbaOran}). Çatı katı kapalı çıkmaları bir alt katında bulunan kapalı çıkmanın derinlik ve genişlik uzunluklarını almaktadırlar. Ayrıca bodrum katı olan yapılarda giriş sahanlığı birinci katta bulunan kapalı çıkma mesafesi kadar dışarı çıkmaktadır. K8 kuralında açıklanan 110 ada 131 parsel ve 118 ada 1 parselde bulunan yapıların ikinci katları arka cepheleri harici diğer cephelerde dışarı çıkma yapmaktadır. Bu yapıların ikinci katlarında bulunan kapalı çıkmalar bir alt kat kapalı çıkmasına göre hem derinlik hemde genişlik olarak ikinci kattaki çıkma mesafesi kadar büyümektedir.

![Cephe çıkmalarının oluşumlarını gösteren gramer kuralları. \label{K13K17}](source/figures/K13-K17.pdf){width=100%}

<!-- TODO: Vectorworkste K18'in hangisi olacağına karar verilmesi Gerekiyor -->

Şekil \ref{K13K17}'daki kurallar sokak yönünü gösteren üçgen sembol tarafında kapalı çıkma ve arka cephede açık çıkma oluşumunu tanımlamaktadır. ***Kapalı çıkmaları tanımlayan kurallar bir yapı için katlar arası ilişkili olarak kurallarda tanımlı katların tamamına uygulanmaktadır veya hiç birine uygulanmaktadır.*** K13, K14 ve K15 kuralları ya hep beraber uygulanmaktadır veya hep beraber uygulanmamaktadır. K13 birinci kat, K14 kuralı üzerine tam kat gelmeyen birinci kat veya ikinci kat, K15 kuralı ise bodrum kat kapalı çıkmalarının oluşumunu göstermektedir. K17 kuralı üzerine tam kat gelmeyen katların arka cephesindeki açık çıkmayı göstermektedir. K16 kuralı ise sadece 128 ada 10 parselde bulunan yapıda görülen, birinci ve ikinci katta oluşan kapalı çıkmaya ek olarak birinci katta ön cephenin yan parçalarının ilave olarak kapalı çıkmanın %41,31'i kadar öne çıkmasını tanımlamaktadır.

<!-- TODO: K16 city engine eklenmeli -->

Table: Kapalı çıkmaların derinlik ölçüleri ve genişlik-derinlik oranı tablosu. \label{CumbaOran}

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** | **Genişlik/Derinlik** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: | --------------------: |
| **118** |      **1** |               |         1,900 m |        2,300 m |               |                 2,358 |
| **128** |     **10** |               |         1,460 m |        1,460 m |               |                 3,247 |
| **110** |     **16** |               |                 |                |               |                       |
| **110** |     **39** |               |         1,840 m |                |               |                 2,696 |
| **110** |     **41** |               |         1,780 m |                |       1,780 m |                 2,107 |
| **110** |    **131** |               |         3,220 m |        3,450 m |       3,450 m |                 1,270 |
| **129** |     **26** |               |                 |                |               |                       |
| **110** |     **44** |               |                 |                |               |                       |
| **114** |     **30** |               |                 |                |               |                       |
| **128** |      **7** |               |                 |                |               |                       |
| **888** |      **8** |               |                 |                |               |                       |
| **127** |     **28** |               |         1,210 m |                |       1,210 m |                 2,392 |
| **110** |     **23** |               |         1,250 m |                |               |                 2,570 |
| **110** |     **43** |               |                 |                |               |                       |
| **888** |      **7** |               |                 |                |               |                       |

### Çatı Katı Oluşumu

Çatı katları sadece üç parçalı cepheye sahip yapılarda bulunmaktadır. Şekil \ref{cephegruplama}'te görüleceği üzere üç parçalı cepheye sahip yapıların yarısında çatı katı oluşumu gözlemlenmektedir. Çatı katı yükseklikleri yapıların 2/3'ünde zemin kata yakın değerler alırken geri kalanında zemin kattan daha kısa olarak bulunmaktadır (Tablo \ref{katyukseklikleri}). Çatı katının cephedeki genişliği bir alt katın cephesinin orta parçasının genişliğine eşit olmaktadır.

![Çatı katı oluşumlarını gösteren gramer kuralları. \label{K18K23}](source/figures/K18-K23.pdf){width=100%}

K18 ve K19 kuralları üzerine tam kat gelmeyen katlar üzerinde çatı katı oluşumu için gerekli bölümlenmeyi tanımlamaktadırlar. K20 kuralı üzerine tam kat gelmeyen üç parçalı cephe tipine sahip kütle üzerine orta parça oranı genişliğinde ve tablo \ref{katoranlari}'teki zemin kat yüksekliğine oranına göre çatı katının eklenmesini göstermektedir. K21 kuralı aynı oluşumu kapalı çıkması bulunan alt kat üzerinde tanımlamaktadır. K22 kuralı 110 ada 131 parseldeki ve K23 kuralı ise 110 ada 41 parseldeki çatı katının yan cephelere doğru genişlemesini göstermektedir.

<!-- TODO: YANLARA DOĞRU OLAN ÇATI GENİŞLEMESİNİN ORANLAR İLE TANIMLANMASI GEREKİYOR-->

<!--
### Form Analizi

Bölgedeki geleneksel konutlar kat sayısına göre kütlesel oluşumu açısından incelendiğinde 5 farklı gruba ayrılmaktadır. Bütün yapılarda zemin kat ve birinci kat vardır. Sadece zemin kat ve birinci katı olan iki yapı bulunmaktadır.

![İncelenen Ortahisar evlerinin tanımlanan kurallar ile kütlesel oluşturuluş şeması. \label{formanalizi}](source/figures/kutlegrameri.pdf){width=100%}
-->
<!-- TODO: Vectorworksten güncel halinin alınması gerekiyor. Vectorworkste Bodrum kattada oluşan kapalı çıkma kısımları eklenmelidir. Giriş katı ve çatı katını belli eden gri tonlama eklenmeli.-->

### Cephe Panelleri

Yapıların kat oluşumları ve cephe bölümlenmeleri tamamlandıktan sonra cephe yüzeylerinin cephe panelleri ile işlenmesi başlamaktadır. İncelenen yapılar doğrultusunda tek parçalı ve üç parçalı cepheye sahip yapılara ait panel yerleşimleri şekil \ref{K24K27} ve \ref{K28K44}'da tanımlanmıştır.

![Tek parçalı cepheye sahip yapılardaki panel oluşumlarını gösteren gramer kuralları. \label{K24K27}](source/figures/K24-K27.pdf){width=100%}

Tek parçalı cephe tipine sahip yapılar için K24, K25, K26 ve K27 kuralları ile sırasıyla bodrum kat, zemin kat, birinci kat ve üzerine tam kat gelmeyen birinci veya ikinci kat cephelerine ait panel yerleşimi gösterilmiştir. Bu kurallarda bütün katlar için tek bir panel tipi tanımlanmıştır. Bodrum ve zemin katta yapıların girişi bulunduğundan dolayı K24 ve K25 kurallarında aynı panelin içerisinde kapı bulunduran tipi ile farklılaştırılmıştır.

<!-- Hem bodrum hemde zeminden giriş olunca problem olmayacak mı?-->

![Üç parçalı cepheye sahip yapılardaki panel oluşumlarını gösteren gramer kuralları. \label{K28K44}](source/figures/K28-K44.pdf){width=100%}

Üç parçalı cephe tipine sahip yapılardaki panellerin yerleşimi K28'den K45'e kadar olan kurallar ile tanımlanmıştır. K28'den K32'ye kadar olan kurallar sırasıyla zemin kat, birinci kat, üzerine tam kat gelmeyen birinci veya ikinci kat ve bodrum kat panellerinin yerleşimini tanımlamaktadır. K32 kuralı 110 ada 16 parseldeki gibi bina girişi yan cepheden olan yapıları tanımlamaktadır. K33, K34 ve K35 kuralları kapalı çıkması bulunan yapılardaki panel yerleşimlerini göstermektedir. K36 kuralı üzerine tam kat gelmeyen birinci veya ikinci katlarda arka cephede açık çıkma bulunan cephe tipini göstermektedir. K37'den K41'e kadar olan kurallar çatı katlarının panel yerleşimini göstermektedir.

<!-- YAN CEPHELERİN DE TANIMLANMASI LAZIM
AKSİ Gramerde belirtilmediği durumlarda ya tek düze yada sağır cepheler mevcut
129-26 3 parçalı yan cepheye sahiptir
888-8 2 parçalı cepheye sahiptir
 -->

Yapıların cephe karakteri ağırlıklı olarak ön ve arka cephelerde tanımlanmasından ve yan cephe yüzeylerinde bulunan düzensizliklerden dolayı yan cepheler ön ve arka cepheler ile dil birliği sağlayacak şekilde, incelenen yapılar göz önünde bulundurularak oluşturulmuştur. Bu bağlamda aksi bir kural belirtilmediği takdirde K43 ve K44 kuralları yan cephelerin oluşumunu tanımlamaktadır.

### Cephe Elemanları Analizi

Yapı katlarının cephelerini tanımlayan cephe panelleri cephe elemanlarından oluşmaktadırlar. Cephe elemanları kat silmesi, düşey bant, pencere ve kapı olarak sıralanmaktadırlar. Kat silmesi bütün panellerde bulunurken diğer cephe elemanları panel içinde bulunup bulunmamasına göre şekil \ref{KPaneller}'de gösterildiği gibi panelleri çeşitlendirmektedirler.

![Cephe panellerinin yatay ve düşey bantların oluşumunu gösteren gramer kuralları. \label{KPaneller}](source/figures/KPaneller.pdf){width=100%}

Geleneksel Ortahisar evlerinin cepheleri incelendiğinde düşeyde ve yatayda simetrik olduğu gözlemlenmektedir. Bununla birlikte cephelerde yataylığı ve düşeyliği vurgulayan kat hizalarında kat silmeleri ve onların aralarında yapının ve kapalı çıkmaların dış köşelerinde bulunan düşey bantlar bulunmaktadır. Yatay ve düşey bantların genişlikleri tutarlı bir şekilde birbirine yakın değerler ile tekrar etmektedir. Panellerin alt kısmındaki koyu ince bant kat silmesini tanımlamaktadır. Panel kenarlarında kat silmesine göre daha açık renkte taralı dikey hatlar düşey bantları belirtmektedir. İncelenen yapılardaki bu elemanların ölçüleri tablo \ref{silmebantolcu}'de gösterilmiştir. ***Kat silmeleri kat yüksekliğine göre ölçüsü oranlı bir şekilde değişmeyip cephe boyunca tutarlı bir değer almaktadır. Ayrıca kat sayısına göre gruplandırılan yapılarda yakın değerler göstermektedir.*** Bu sebeple çatı katı olan iki katlı ve çatı katı olan üç katlı yapılarda 0,13m ile 0,21m, diğer yapılarda 0,19m ile 0,44m aralığında değerler almaktadır. ***Köşelerdeki düşey bantların genişlik ölçüleri de kat silmeleri gibi cephe genişlikleri ile bir korelasyon içinde bulunmadığından dolayı gerçek ölçüleri ile değerlendirilmiştir*** ve 0,105m ile 0,571m arasında değişmektedir.

Table: Kat silmeleri ve düşey bant ölçülerinin tablosu. \label{silmebantolcu}

| **Ada** | **Parsel** | **Kat Silmesi** | **Sol Köşe Bant** | **Cumba Sol Köşe Bant** | **Cumba Sağ Köşe Bant** | **Sağ Köşe Bant** |
| -------:| ----------:| ---------------:| -----------------:| -----------------------:| -----------------------:| -----------------:|
| **118** | **1**      | 0,200 m         | 0,339 m           |                         |                         | 0,349 m           |
| **128** | **10**     | 0,340 m         | 0,296 m           | 0,296 m                 | 0,285 m                 | 0,169 m           |
| **110** | **16**     | 0,170 m         | 0,243 m           | 0,180 m                 | 0,180 m                 | 0,244 m           |
| **110** | **39**     | 0,170 m         | 0,360 m           |                         |                         | 0,340 m           |
| **110** | **41**     | 0,210 m         |                   | 0,105 m                 | 0,127 m                 | 0,571 m           |
| **129** | **26**     | 0,170 m         | 0,320 m           |                         |                         | 0,280 m           |
| **110** | **131**    | 0,130 m         | 0,190 m           | 0,170 m                 | 0,190 m                 | 0,190 m           |
| **888** | **8**      | 0,440 m         | 0,508 m           | 0,424 m                 | 0,424 m                 | 0,487 m           |
| **110** | **23**     | 0,190 m         | 0,191 m           | 0,212 m                 | 0,212 m                 | 0,191 m           |
| **110** | **44**     | 0,190 m         | 0,220 m           |                         |                         | 0,190 m           |
| **114** | **30**     | 0,280 m         | 0,212 m           |                         |                         | 0,212 m           |
| **128** | **7**      | 0,340 m         | 0,230 m           |                         |                         | 0,210 m           |
| **127** | **28**     | 0,170 m         | 0,233 m           | 0,233 m                 | 0,254 m                 | 0,233 m           |
| **110** | **43**     | 0,250 m         | 0,339 m           | 0,191 m                 | 0,191 m                 | 0,339 m           |
| **888** | **7**      | 0,440 m         | 0,550 m           |                         |                         | 0,157 m           |

<!--
### Pencere Genişlikleri ve Yükseklikleri Analizi
-->

İncelenen yapıların cephe panellerinde panel ve pencere büyüklüğüne bağlı olarak farklı sayıda pencere bulunmaktadır. Yapılar pencerelerin yüzey büyüklüğüne göre cephe panellerinde tek pencere ve birden fazla pencere bulunan olarak iki grupta ayrıştırılabilirler. Yapıların %19,75'inde cephe panellerinde tek pencere bulunmaktadır ve bu yapılar üç parçalı cepheye sahiptirler. Geriye kalan %81,75'inde iki veya daha fazla pencere bulunmaktadır. Tablo \ref{PKenar}'de üç parçalı cepheye sahip yapıların kenar parçalarında bulunan pencere sayıları gösterilirken tablo \ref{POrta}'da üç parçalı cepheye sahip yapıların orta kısmı ve tek parçalı cepheye sahip yapıların cephelerindeki pencere sayıları gösterilmiştir.

Table: Üç parçalı cepheye sahip yapıların kenar cephe parçalarındaki pencere sayılarının tablosu. \label{PKenar}

|               | **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------------- | ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **3 Parçalı** |         |            |               |                 |                |               |
|               | **118** |      **1** |             2 |               3 |              3 |               |
|               | **128** |     **10** |             1 |               1 |              1 |               |
|               | **110** |     **16** |             2 |               2 |                |             3 |
|               | **110** |     **39** |             2 |               2 |                |             2 |
|               | **110** |     **41** |             2 |               2 |                |             2 |
|               | **110** |    **131** |             3 |               3 |              3 |             2 |
|               | **129** |     **26** |             2 |               2 |                |             3 |
|               | **888** |      **8** |             3 |               3 |              3 |               |
|               | **127** |     **28** |             2 |               1 |                |             1 |
|               | **110** |     **23** |             1 |               1 |                |               |
|               | **110** |     **43** |             1 |               2 |                |               |
|               | **888** |      **7** |             1 |               3 |                |               |

Table: Üç parçalı cepheye sahip yapıların orta cephe parçalarındaki ve tek parçalı cepheye sahip yapıların cephelerindeki pencere sayılarının tablosu. \label{POrta}

|               | **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------------- | ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **3 Parçalı** |         |            |               |                 |                |               |
|               | **118** |      **1** |         Giriş |               3 |              3 |               |
|               | **128** |     **10** |         Giriş |               1 |              1 |               |
|               | **110** |     **16** |             2 |               2 |                |             3 |
|               | **110** |     **39** |         Giriş |           Giriş |                |             2 |
|               | **110** |     **41** |         Giriş |               2 |                |             2 |
|               | **110** |    **131** |         Giriş |               2 |              2 |             2 |
|               | **129** |     **26** |             3 |               3 |                |             3 |
|               | **888** |      **8** |         Giriş |               2 |              2 |               |
|               | **127** |     **28** |         Giriş |               2 |                |             2 |
|               | **110** |     **23** |         Giriş |               1 |                |               |
|               | **110** |     **43** |             1 |               2 |                |               |
|               | **888** |      **7** |         Giriş |               2 |                |               |
| **1 Parçalı** |         |            |               |                 |                |               |
|               | **110** |     **44** |             2 |               5 |              5 |               |
|               | **114** |     **30** |             6 |               6 |                |               |
|               | **128** |      **7** |             4 |               4 |                |               |

Şekil \ref{KPaneller2}'deki kurallar panellerin içindeki pencere ve kapı yerleşim düzenlerini göstermektedir. Sağ üst köşesinde "•" simgesi bulunan paneller iç düzenlerinde kapı olacağını, bu simge bulunmayan panellerde sadece pencereler olacağını ifade etmektedir. İç bölümlenmesi tanımlanan panellerde görülen "*" simgesi bulunduğu bölmenin panel içinde yeterli genişlik bulunmadığında yok sayılmasını veya yeterli genişlik bulunduğunda bir veya daha fazla sayıda tekrar ettiğini göstermektedir. Panel içlerinde "e" ile tanımlı bölümler içerisinde herhangi bir cephe elemanı bulunmayan duvar yüzeylerini göstermektedir. Bu bölümler panel genişliğine diğer bölümlerin yerleşmesinden sonra arta kalan kısmı doldurmaktadır.

![Cephe panellerinde kapı ve pencere yerleşimini gösteren gramer kuralları. \label{KPaneller2}](source/figures/KPaneller2.pdf){width=100%}

Yapılardaki pencerelerin yükseklikleri katlar arasında yedi yapıda farklılık göstermezken geri kalan yapılarda %5 ile %13 oranında değişmektedir. Katlar arası kat yükseklikleri de yapılarda farklılık göstermektedir. Ancak pencere ve kat yüksekliklerinin değişimleri arasında bir bağıntı bulunmamaktadır. Bu sebepten dolayı yapıların zemin kat yüksekliklerinin zemin katlarında bulunan pencere yüksekliklerine oranları üzerinden gramer oluşturulmuştur. Zemin kat yüksekliğinin pencere yüksekliğine göre oranlarına bakıldığında 1,439 - 2,378 değer aralığı bulunmaktadır (Tablo \ref{PKOran}). 110 ada 44 parseldeki yapının zemin katı diğer yapılara göre farklılık gösterdiğinden değer aralığı dışında tutulmuştur.

Table: Kat yüksekliklerinin pencere yüksekliklerine göre oranları tablosu. \label{PKOran}

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

Yapılardaki pencerelerin genişlikleri cephe panelinde tek pencere ve iki veya daha fazla pencere bulunan iki gruba göre ayrıştırıldığında cephe parçalarında iki veya daha fazla pencere bulunan yapılarda pencere yüksekliğinin genişliğine oranı 1,493 ile 1,881 arasında değişmektedir. Cephe parçasında tek pencere bulunan yapılarda ise bu oran 0,854 ile 1,050 arasındadır (Tablo \ref{POran}). Cephe paneline tek pencere sığan yapılar K54, K58 ve K61 kurallarını kullanmak zorundadırlar. Bir başka deyişle bu üç kural pencere yüksekliğinin pencere genişliğine oranının 1,051'den küçük olduğu yapılarda uygulanmaktadır. Cephe panelinde iki veya daha fazla pencere bulunan yapılar şekil \ref{KPaneller2}'deki bütün kuralları kullanabilirler.

Table: Pencere yüksekliklerinin genişliklerine göre oranları tablosu. \label{POran}

| **Ada** | **Parsel** | **Zemin Kat** | **Birinci Kat** | **İkinci Kat** | **Çatı Katı** |
| ------: | ---------: | ------------: | --------------: | -------------: | ------------: |
| **118** |      **1** |         1,881 |           1,579 |          1,579 |               |
| **110** |     **16** |         1,520 |           1,667 |                |         1,722 |
| **110** |     **39** |         1,605 |           1,618 |                |         1,076 |
| **110** |     **41** |         1,772 |           1,805 |                |         1,341 |
| **110** |    **131** |         1,811 |           1,755 |          1,755 |         1,600 |
| **129** |     **26** |         1,595 |           1,595 |                |         1,595 |
| **110** |     **44** |               |           1,842 |          1,861 |               |
| **114** |     **30** |         1,705 |           1,705 |                |               |
| **128** |      **7** |         1,493 |           1,585 |                |               |
| **888** |      **8** |         1,736 |           1,836 |          1,860 |               |
| **110** |     **43** |               |           1,860 |                |               |
| **888** |      **7** |         1,550 |           1,827 |                |               |
| **110** |     **23** |         0,991 |           1,031 |                |               |
| **128** |     **10** |         0,854 |           0,854 |          0,827 |               |
| **127** |     **28** |         1,050 |           1,792 |                |         0,653 |

![Cephe panellerinde kapı ve pencere detaylarının oluşumunu gösteren gramer kuralları. \label{KPaneller3}](source/figures/KPaneller3.pdf){width=100%}

Şekil \ref{KPaneller3}'de tanımlı kurallar paneller içerisinde bulunan pencere ve kapı detaylarının oluşumunu göstermektedir. Pencere ve kapıların kendileri ve diğer cephe elemanları ile aralarında bulunan duvar kısımlarının ve pencere denizlik kısımlarının yerleşimini belirtmektedir. Bu bölmelerin bir araya gelirken kullandıkları oranlar tablo \ref{PKDOran}'de gösterilmiştir. Daha doğru modeller üretebilmek için bulunan değerlerin yoğunlaştığı aralıkların gruplanması sonucunda değerler aşağıdaki gibi olmaktadır;

- Kat yüksekliğinin denizlik yüksekliğine oranı yapıların %66,67'sinde 5,068 ile 7,511, %20'sinde 3,675 ile 4,077 arasında değerler alırken geri kalan iki yapı için en 2,665 ve 11,406 uç değerlerini almaktadır.
- Pencere genişliğinin duvar genişliğine oranı yapıların %60'ında 0,208 ile 0,369, %13,33'ünde 0.058 ile 0.074 aralıklarındadır ve geri kalan bir yapıda 0,567 uç değerini almaktadır.
- Kapı genişliğinin pencere genişliğine oranı cephe panelinde tek pencere bulunan yapılarda 0,607 ile 0,823, birden fazla pencere bulunan yapıların %45,45'inde 1,500 ile 1,614, %36,36'sında 1,070 ile 1,213 ve geri kalan %18,18'inde  0,827 ile 0,877 değer aralığındadır.

Table: Pencerelerin aralarındaki duvar boşluklarına ve kapılara, denizlik yüksekliğinin zemin kat yüksekliğine oranları tablosu. \label{PKDOran}

| **Ada** | **Parsel** | **Kat Yüksekliği / Denizlik Yüksekliği** | **Pencere Genişliği / Duvar Genişliği** | **Kapı Genişliği / Pencere Genişliği** |
| ------: | ---------: | ---------------------------------------: | --------------------------------------: | -------------------------------------: |
| **118** |      **1** |                                    7,511 |                                   0,074 |                                  1,070 |
| **128** |     **10** |                                    3,675 |                                         |                                  0,823 |
| **110** |     **16** |                                    6,146 |                                   0,293 |                                  1,213 |
| **110** |     **39** |                                    6,582 |                                   0,369 |                                  1,132 |
| **110** |     **41** |                                    6,715 |                                   0,325 |                                  1,122 |
| **110** |    **131** |                                    3,963 |                                   0,273 |                                  1,538 |
| **129** |     **26** |                                    6,508 |                                   0,567 |                                        |
| **110** |     **23** |                                    5,068 |                                         |                                  0,607 |
| **110** |     **44** |                                    7,109 |                                   0,208 |                                  1,614 |
| **114** |     **30** |                                    6,662 |                                   0,058 |                                  0,827 |
| **128** |      **7** |                                    5,475 |                                   0,338 |                                  1,145 |
| **888** |      **8** |                                    4,077 |                                   0,248 |                                  1,529 |
| **127** |     **28** |                                   11,406 |                                         |                                  0,672 |
| **110** |     **43** |                                    7,540 |                                   0,282 |                                  0,877 |
| **888** |      **7** |                                    2,665 |                                   0,227 |                                  1,500 |

<!--
Table: Pencere denizlik yüksekliklerinin tablosu. \label{PDenizlik}

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
-->

### Çatı Formu ve Eğimi Analizi

İncelenen Ortahisar yapılarında kırma, beşik ve ikisinin birleşimi olan melez çatılara rastlanmaktadır. Melez çatılar genellikle kapalı çıkma üzerinde üçgen alınlık oluşturan kırma çatılardır. Çatı katı üzerine gelen çatılar beşik çatı olarak şekillenmektedir. Eğerki çatı katı yan cephelere doğru genişliyorsa bu parçaların üzeri kırma veya beşik çatı ile örtülmektedir. Sadece 110 ada 16 parseldeki yapının çatı katı kırma çatı ve çatı katı altında kalan katı örten çatı melez çatı ile örtülmektedir. Tablo \ref{Cati}'de yapıların çatı eğimlerine bakıldığında %80'i %17 ile %23 arasında geri kalanı %28 ile %34 arasındadır. Üç katlı yapıların tamamı kırma çatı ile örtülmüştürlerdir.

<!--
Ortahisar evlerinin çatı eğimleri 17° ile 34° arasında değişmektedir. Çatı katı olmayan yapılar %77.7'si kırma çatıya %11,1'i beşik çatı ve geri kalanı kırma ve beşik melez bir çatıya sahiptir. Çatı katı olan yapılarda alt kat çatısı eşit oranlarda kırma, beşik ve melez çatıya sahiptir. Çatı katı olan yapıların çatı katı %16,6'sı kırma, %66,6 beşik ve %16,6'sı melez çatıya sahiptir.
-->

Table: Kat sayısına göre gruplandırılmış yapıların çatı formu ve eğimi tablosu. \label{Cati}

|         | **Ada** | **Parsel** | **Alt Kat**   | **Çatı Katı** | **Çatı Eğimi** |
| ------: | ------: | ---------: | ------------- | ------------- | -------------: |
|   **4** |         |            |               |               |                |
|         |     118 |          1 | Kırma         |               |            20° |
|         |     128 |         10 | Beşik         |               |            20° |
| **3,5** |         |            |               |               |                |
|         |     110 |         16 | Beşik + Kırma | Kırma         |            23° |
|         |     110 |         39 | Kırma         | Beşik         |            18° |
|         |     110 |         41 | Beşik         | Beşik + Kırma |            18° |
|         |     110 |        131 | Kırma         | Beşik         |            19° |
|         |     129 |         26 | Kırma         | Beşik         |            18° |
|   **3** |         |            |               |               |                |
|         |     110 |         23 | Kırma         |               |            28° |
|         |     110 |         44 | Kırma         |               |            18° |
|         |     114 |         30 | Kırma         |               |            18° |
|         |     128 |          7 | Kırma         |               |            17° |
|         |     888 |          8 | Kırma         |               |            20° |
| **2,5** |         |            |               |               |                |
|         |     127 |         28 | Beşik         | Beşik         |            34° |
|   **2** |         |            |               |               |                |
|         |     110 |         43 | Beşik + Kırma |               |            30° |
|         |     888 |          7 | Kırma         |               |            18° |

Şekil \ref{KCati}'de çatı oluşumu ile ilgili kurallar tanımlanmıştır. K72'den K76'ya kadar olan kurallar çatı katı altında kalan katı ve çatı katı olmayan yapılarda bulunan en üst katı örten çatıların oluşumunu tanımlamaktadırlar. K74 kuralı 127 ada 28 parselde bulunan yapıdaki beşik çatıyı, K75 kuralı ise 110 ada 16 parselde bulunan yapıdaki melez çatıyı tanımlamaktadırlar. K76 ve K77 kuralları çatı katı bulunmayan ancak kapalı çıkmaya sahip yapılardaki kapalı çıkma üzerindeki çatı oluşumunu belirtmektedirler. K78, K79, K80 ve K81 kuralları çatı katı üzerindeki çatı oluşumunu tanımlamaktadır. CityEngine üzerinde CGA kodu ile melez çatı oluşturulamadığından dolayı bu tür çatılar CGA kodu içerisinde bulunmamaktadır.

![Çatı oluşumunu gösteren gramer kuralları. \label{KCati}](source/figures/KCati.pdf){width=100%}

<!-- 
### Biçim Grameri

![Ortahisar evlerinin kütlesel biçim grameri dili. \label{bicimgrameri}](source/figures/bicimgrameri.pdf){width=100%}

## CGA Biçim Gramerinin Oluşturulması

CGA gramer kodu CityEngine yazılımında yazılmaya başlanmıştır ve büyük oranda tamamlanmıştır.  

![CityEngine üzerinde CGA kodu ile üretilen modeller.](source/figures/OrtahisarCGA.png){width=100%}
-->

\newpage
