# GENEL BİLGİLER

\pagestyle{main}
\thispagestyle{empty}

## Giriş

Yordamsal modelleme kural tabanlı otomatik veya yarı otomatik içerik üretmeye yönelik bir yöntem olup çeşitli alanlarda doku, bitki, arazi, nehir, bina, kent, yol ağları gibi modellerin oluşturulmasında kullanılmaktadır. İçerisinde L-sistemler (Lindenmayer sistemleri), fraktallar, biçim gramerleri ve üretken sistemler gibi birden fazla tekniği barındıran bir ana başlık niteliğindedir. 30 yıldan fazla bir süredir üzerine aktif araştırma yapılan konu, çok çeşitli varyasyonları üretebilme potansiyeli ve içerik üretiminde insan gücü etkileşimini azaltması ile mimarlık, oyun ve film endüstrisi sanal ortamlarında cazip bir yöntem olarak görülmektedir [@Schinko:2015gn].

Yordamsal modeller bir binanın, tasarım stilinin veya kültürel bir dönemintasarım ve yapım bilgilerini kodlamak için kullanılabilmektedirler. En önemli avantajlarından birisi tek bir yapının rekonstrüksiyonunu detaylı bir şekilde yapabilmesinin yanında, aynı tasarım ve yapım kurallarını paylaşan çok sayıda benzer modeller üretebilmesidir. Yordamsal modellerin üretiminde Lindenmayer sistemi, fraktal, split gramer, biçim grameri gibi birçok üretken sistem kullanılmaktadır. Binaların modellerinin oluşturulmasında özellikle yordamsal cephe üretimi kullanılmaktadır ve üretim iki boyutlu parsel hattının girdi olarak sisteme tanıtılması ile başlamaktadır.

Yordamsal modelleme tekniğinin bir diğer avantajı ise modellenen bina veya obje hakkında uzman bilgiye sahip olunmasını sağlamaktadır. Mimaride kullanılan yapı tiplerine ait sınıflandırma şemalarının ve tablolarının kod içine aktarımı gerekmektedir. Bu da günümüz kentlerinde o veya bu şekilde kaybettiğimiz geleneksel yapıların kurallarının elde edilip, kayıt altına alınmasını sağlamaktadır. Koruma anlamında sunduğu olanağın yanında geleneksel doku içinde tasarım yaparken temel olarak alınacak verileri de sağlamış olmaktadır. Kuşkusuz ki bu yöntem klasik yöntemlere göre geleneksel yapı karakteri üzerine daha fazla bilgi sunmaktadır. Bu anlamda **gün geçtikçe sayıları azalan Trabzon geleneksel konutları örnek çalışma alanı olarak incelenecektir**.

Yordamsal modeller semantik bir yapıya sahiptirler ve bu özellikleri ile simülasyon ve planlama için geleneksel modellere göre daha uygundurlar. Günümüz kentsel yenileme ve kentsel canlandırma projelerinde kullanımları da birçok varyasyona ve analiz olanağına kısa sürede imkân sağlamaktadır. Aynı şekilde tekil birimler içinde çeşitli öneriler sunması bu önerilerin yeni tasarım yorumları için altlık oluşturmaktadır. Bu doğrultuda çalışmada **Trabzon geleneksel konutlarının CGA** (Computer Generated Architecture) **gramerlerinin oluşturulması ve parametrik olarak üretilmesi amaçlanmaktadır**.

Trabzon kent içinde bulunan geleneksel konutlar üzerinde yapılmış rölöve çalışmaları ve akademik çalışmalar proje için gerekli ana veriyi oluşturacaktır. **Çalışmanın ilk bölümünde analiz-sentez yöntemi kullanılacak** ve ikinci aşama için gerekli olan CGA biçim gramerleri hazırlanmış olacaktır. **İkinci bölümde CGA biçim gramerleri üzerinden kodlama yapılacaktır**. Bunun için mimarların aktif olarak kullandığı ve tanıdığı Rhinoceros programı üzerinde çalışan Grasshopper platform olarak seçilmiştir. Grasshopper için yazılmış birçok eklenti bulunmaktadır ve model üzerinde interaktif olarak analiz yapma olanağı sunmaktadır. Bunun yanında gelişmeye açık bir platform olması da tercih sebebidir. Bu kapsamda Grasshopper üzerinde C\# programlama dili üzerinden geliştirilecek kodlar ile Trabzon evlerinin kurallarını içeren bir eklenti geliştirilecektir.

**Çalışmanın konusu** yordamsal modelleme çalışması ile geleneksel Trabzon konutlarının üç boyutlu modellerinin oluşturulması için gerekli kural gruplarının oluşturulmasıdır. Yordamsal modellemede kural grupları diye nitelenen ifade üç boyutlu modelleri oluşturan bilgisayar kodlarıdır. Kullanıcının modeli kendisinin oluşturduğu geleneksel modelleme yazılımlarından farklı olarak yordamsal modellemede bir yapının veya yapı türünün semantik tanımlamasının programlama dillerini kullanarak bilgisayara tanıtılması ile modeller üretilmektedir. Bu sadece teknik yönden değil kuramsal olarak da farklılıklar ortaya koymaktadır. Seçilen modelleme yöntemi sadece maliyet ve estetik çıktısını değil; bilginin nasıl seçildiği, işlendiği ve nelerin bilgi olarak değerlendirildiği gibi hususları da etkilemektedir [@Saldana:2015el].

## Amaç ve Kapsam

Önerilen çalışma yordamsal modelleme yöntemi kullanılarak geleneksel Trabzon konutlarının CGA gramerlerinin oluşturulmasını ve parametrik olarak üretilmesini amaçlamaktadır.

Hedefler;

<!--Kütlesel cephe ve plan üretiminin beraber yapılacağı bütünleşik bir yöntem geliştirmek.-->

<!--Geliştirilecek yöntem ile kütlesel cephe özelliklerinin yanında plan şeması da oluşturularak iç mekanların kullanım amacına, mekanların birbirleriyle olan orantılarına, aydınlanma ve sirkülasyon gibi özelliklerine ait bilgiler sağlamak.-->

1. Rhinoceros üzerinde çalışan Grasshopper için geleneksel Trabzon evlerini parametrik olarak üretecek bir eklenti geliştirmek.

   <!--Geliştirilecek eklenti ile tahrip olmuş geleneksel Trabzon evleri için tahrip olmadan önceki haline dair muhtemel karakteristik özellikleri üretilebilmek.-->

2. Tarihi dokuda yeni yapılacak binalar için geleneksel dokuya ait referans bilgi sağlamak. Üretilecek modellerin varyasyonlarını yeni tasarımlar için altlık olarak sunmak.

Proje kapsamında geleneksel Trabzon kent içi evlerinin yordamsal modelleme için kural gruplarının çıkarılması ve modellerinin üretilmesi yer almaktadır. Bu doğrultuda Grasshopper programı üzerinde çalışan C\# programlama dili ile yazılmış modelleri üretecek bir eklenti geliştirmek ve üretilecek modellerde cepheleri çözümleyebilmeyi kapsamaktadır.

## Çalışmanın Yöntemi

Araştırma da iki kademeli bir süreç işlenecektir;

1. Birinci Bölüm

   Çalışmanın ilk bölümünde analiz-sentez yöntemi kullanılacak ve ikinci aşama için gerekli olan CGA (Computer Generated Architecture) biçim grameri verileri hazırlanmış olacaktır.
   1. Trabzon geleneksel evlerine ait verilerin toplanması: Çalışma için gerekli olan Trabzon geleneksel evlerine ait veriler akademik ve profesyonel çalışmalardan toplanacaktır. Temel Kaynaklar;

       -   Trabzon Kültür ve Tabiat Varlıklarını Koruma Bölge Kurulu Müdürlüğü Arşivi
       -   KTÜ Mimarlık Bölümü Doğu Karadeniz Arşivi
       -   Trabzon geleneksel evleri üzerine yapılmış akademik çalışmalar
       -   Trabzon geleneksel evleri üzerine rölöve çalışması yapmış ofis arşivleri

   2. Analiz çalışması: Evlere ait veriler toplandıktan sonra aşağıda belirtilen özelliklere göre analizleri yapılacaktır.

       - Yapı taban alanı

         <!--Yapı hacmi, Plan tipi-->

       - Kat sayısı ve yüksekslikleri

       - Cephe karakteri

       - Cephe çıkmaları

       - Pencere genişlikleri ve yükseklikleri

       - Çatı formu ve eğimi

         <!-- Parsel kullanımı, Bahçe içi yerleşim -->

   3. Sentez çalışması: Çıkarılan veriler gruplar halinde tablolara dökülerek kural oluşturmak için gerekli sayısal özellikler organize edilecektir. Bu sayısal veriler eklenti oluştururken izlenecek veri akış şemasının oluşturulmasında kullanılacaktır.

2. İkinci Bölüm

   İkinci bölümde CGA biçim gramerleri üzerinden kodlama yapılacaktır. Bunun için mimarların aktif olarak kullandığı ve tanıdığı Rhinoceros programı üzerinde çalışan Grasshopper platform olarak seçilmiştir. Grasshopper için yazılmış birçok eklenti bulunmaktadır ve model üzerinde interaktif olarak analiz yapma imkanı sunmaktadır. Bunun yanında gelişmeye açık bir platform olması da tercih sebebidir.

Scripting

   Rhinoceros üzerinde veya Grasshopper üzerinde çalışacak eklenti için öncelikle veri akış şeması ve pseudocode hazırlanacaktır ve C\# programlama dili kullanılarak Microsoft Visual Studio’da eklenti geliştirilecektir.

<!--**Alternatif yöntemler**-->

<!--Bilgisayar yazılımcısı yardımı-->

<!--C\# programlama dili kullanılırken karşılaşılabilecek olumsuzluklarda bir bilgisayar yazılımcısına başvurulacaktır.-->

<!--Esri City Engine-->

<!--Programlama dili kullanılarak istenilen sonuca ulaşılamaması durumunda Esri firmasına ait City Engine yazılımında CGA kod kurallarını yazarak geleneksel yapılara ait cephe çözümlemeleri oluşturulacaktır.-->

<!--Çalışma Alanı: Trabzon geleneksel kent içi konutları hakkında yeterli hazır bilgiye ulaşılamaması durumunda. Saka (Saka, 1996) tarafından hazırlanmış tez üzerinden Akçaabat geleneksel konutları çalışma alanı olarak tercih edilebilir.-->