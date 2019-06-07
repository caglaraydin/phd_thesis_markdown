# GENEL BİLGİLER

\pagestyle{main}
\thispagestyle{empty}

## Giriş

Çalışmanın konusu yordamsal modelleme yöntemi ile geleneksel Trabzon Ortahisar konutlarının üç boyutlu modellerinin üretilebilmesi için gerekli kural gruplarının oluşturulmasıdır. Yordamsal modellemede kural grupları diye nitelenen ifade üç boyutlu modelleri oluşturan bilgisayar kodlarıdır. Kullanıcının modeli kendisinin oluşturduğu geleneksel modelleme yazılımlarından farklı olarak yordamsal modellemede bir yapının veya yapı türünün semantik tanımlamasının programlama dillerini kullanarak bilgisayara tanıtılması ile modeller üretilmektedir. Bu sadece teknik yönden değil kuramsal olarak da farklılıklar ortaya koymaktadır. Seçilen modelleme yöntemi sadece maliyet ve estetik çıktısını değil; bilginin nasıl seçildiği, işlendiği ve nelerin bilgi olarak değerlendirildiği gibi hususları da etkilemektedir [@Saldana:2015el].

Yordamsal modelleme kural tabanlı otomatik veya yarı otomatik içerik üretmeye yönelik bir yöntem olup çeşitli alanlarda doku, bitki, arazi, nehir, bina, kent, yol ağları gibi modellerin oluşturulmasında kullanılmaktadır. <!-- İçerisinde L-sistemler (Lindenmayer sistemleri), fraktallar, biçim gramerleri ve üretken sistemler gibi birden fazla tekniği barındıran bir ana başlık niteliğindedir. --> 30 yıldan fazla bir süredir üzerine aktif araştırma yapılan konu, çok çeşitli varyasyonları üretebilme potansiyeli ve içerik üretiminde insan gücü etkileşimini azaltması ile mimarlık, oyun ve film endüstrisi sanal ortamlarında cazip bir yöntem olarak görülmektedir [@Schinko:2015gn].

Yordamsal modeller bir binanın, tasarım stilinin veya kültürel bir dönemin tasarım ve yapım bilgilerini kodlamak için kullanılabilmektedirler. En önemli avantajlarından birisi tek bir yapının rekonstrüksiyonunu detaylı bir şekilde yapabilmesinin yanında, aynı tasarım ve yapım kurallarını paylaşan çok sayıda benzer modeller üretebilmesidir. Yordamsal modellerin üretiminde Lindenmayer sistemi, fraktal, split gramer, biçim grameri gibi birçok üretken sistem kullanılmaktadır. Yordamsal modelleme ile bina modellerinin oluşturulmasında özellikle yordamsal cephe üretimi kullanılmaktadır ve üretim iki boyutlu parsel hattının girdi olarak sisteme tanıtılması ile başlamaktadır.

Yordamsal modelleme tekniğinin bir diğer avantajı ise modellenen bina veya obje hakkında uzman bilgisine sahip olunmasını sağlamaktadır. Mimaride kullanılan yapı tiplerine ait sınıflandırma şemalarının ve tablolarının kod içine aktarımı gerekmektedir. Bu da günümüz kentlerinde o veya bu şekilde kaybettiğimiz geleneksel yapıların kurallarının elde edilip, kayıt altına alınmasını sağlamaktadır. Koruma anlamında sunduğu olanağın yanında geleneksel doku içinde tasarım yaparken temel olarak alınacak verileri de sağlamış olmaktadır. Kuşkusuz ki bu yöntem klasik yöntemlere göre geleneksel yapı karakteri üzerine daha fazla bilgi sunmaktadır.

Yordamsal modeller semantik bir yapıya sahiptirler ve bu özellikleri ile simülasyon ve planlama için geleneksel modellere göre daha uygundurlar. Günümüz kentsel yenileme ve kentsel canlandırma projelerinde kullanımları da birçok varyasyona ve analiz olanağına kısa sürede imkân sağlamaktadır. Aynı şekilde tekil birimler içinde çeşitli öneriler sunması bu önerilerin yeni tasarım yorumları için altlık oluşturmaktadır.

Bu bağlamda gün geçtikçe sayıları azalan Trabzon Ortahisar geleneksel konutları örnek çalışma alanı olarak incelenecektir. Trabzon Ortahisar geleneksel konutlarının CGA (Computer Generated Architecture) gramerinin oluşturulması ve parametrik olarak üretilmesi amaçlanmaktadır. Trabzon kent içinde bulunan geleneksel konutlar üzerinde yapılmış rölöve çalışmaları ve akademik çalışmalar proje için gerekli ana veriyi oluşturmaktadır. Bu veriler üzerinden çalışmanın ilk bölümü için analiz-sentez yöntemi kullanılacaktır. İkinci aşama için biçim gramerleri hazırlanacaktır. Hazırlanan biçim gramerleri üzerinden CGA biçim grameri olarak bilgisayar ortamında kodlanacaktır.

<!-- Bunun için mimarların aktif olarak kullandığı ve tanıdığı Rhinoceros programı üzerinde çalışan Grasshopper platform olarak seçilmiştir. Grasshopper için yazılmış birçok eklenti bulunmaktadır ve model üzerinde interaktif olarak analiz yapma olanağı sunmaktadır. Bunun yanında gelişmeye açık bir platform olması da tercih sebebidir. Bu kapsamda Grasshopper üzerinde C\# programlama dili üzerinden geliştirilecek kodlar ile Trabzon evlerinin kurallarını içeren bir eklenti geliştirilecektir. -->

## Amaç ve Kapsam

Önerilen çalışma yordamsal modelleme yöntemi kullanılarak geleneksel Trabzon konutlarının CGA gramerinin kodlanmasını ve parametrik olarak üretilmesini amaçlamaktadır.

Hedefler;

<!--Kütlesel cephe ve plan üretiminin beraber yapılacağı bütünleşik bir yöntem geliştirmek.-->

<!--Geliştirilecek yöntem ile kütlesel cephe özelliklerinin yanında plan şeması da oluşturularak iç mekanların kullanım amacına, mekanların birbirleriyle olan orantılarına, aydınlanma ve sirkülasyon gibi özelliklerine ait bilgiler sağlamak.-->

<!--Rhinoceros üzerinde çalışan Grasshopper için geleneksel Trabzon evlerini parametrik olarak üretecek bir eklenti geliştirmek.-->

1. Tarihi dokuda yeni yapılacak binalar için geleneksel dokuya ait referans bilgi sağlamak.

2. Üretilecek modellerin varyasyonlarını yeni tasarımlar için altlık olarak sunmak.

3. Trabzon Ortahisar evlerine ait kütle ve cephelerin oluşumunu tanımlayan  biçim gramerini oluşturmak.

Bu çalışma kapsamında geleneksel Trabzon Ortahisar evlerinin yordamsal modelleme için kural gruplarının çıkarılması ve modellerinin üretilmesi yer almaktadır. Çalışma kütle ve cephe bazında olup, modeller için plan üretimi yapılmayacaktır. Elde edilen veriler dahilinde yeterli sayıda plan rölövesine ulaşılamadığı için plan üretimi bu çalışma kapsamı dışında tutulmuştur.

## Çalışmanın Yöntemi

Çalışmada iki kademeli bir süreç işlenmektedir;

1. Biçim gramerinin oluşturulması

   Çalışmanın ilk bölümünde analiz-sentez yöntemi kullanılacak ve ikinci aşama için gerekli olan biçim grameri verileri hazırlanmış olacaktır.

   1. Trabzon geleneksel evlerine ait verilerin toplanması:
      Çalışma için gerekli olan Trabzon geleneksel evlerine ait veriler akademik ve profesyonel çalışmalardan toplanmıştır. Temel Kaynaklar;

       - Trabzon Kültür ve Tabiat Varlıklarını Koruma Bölge Kurulu Müdürlüğü Arşivi
       - KTÜ Mimarlık Bölümü Doğu Karadeniz Arşivi
       - Trabzon geleneksel evleri üzerine yapılmış akademik çalışmalar
       - İstanbul Büyükşehir Belediyesi BİMTAŞ A.Ş. Rölöve çalışmaları
       <!--Trabzon geleneksel evleri üzerine rölöve çalışması yapmış ofis arşivleri-->

   2. Analiz çalışması:
      Evlere ait veriler toplandıktan sonra aşağıdaki listede belirtilen özelliklere göre analizleri yapılmıştır.

       - Yapı taban alanı
         <!--Yapı hacmi, Plan tipi-->
       - Kat sayısı ve yükseklikleri
       - Cephe karakteri
       - Cephe çıkmaları
       - Cephe elemanları
       - Çatı formu ve eğimi

         <!-- Parsel kullanımı, Bahçe içi yerleşim -->

   3. Sentez çalışması:
      Çıkarılan veriler analiz edilen başlıklara göre tablolara dökülerek kural oluşturmak için gerekli sayısal özellikler organize edilmiştir. Bununla beraber kütle ve cephelere ait biçim grameri kuralları hazırlanmıştır.
\newpage
2. CGA gramer kodunun oluşturulması

   İkinci bölümde Ortahisar evleri için hazırlanan biçim grameri kuralları üzerinden CGA grameri kodlaması yapılmıştır. Üretilen kod ESRI firmasına ait CityEngine yazılımı üzerinde çalıştırılmaktadır.

\newpage