# GENEL BİLGİLER

\pagestyle{main}
\thispagestyle{empty}

## Giriş

Çalışma yordamsal modelleme yöntemi ile geleneksel Trabzon Ortahisar konutlarının üç boyutlu modellerinin parametrik olarak üretilebilmesini konu almaktadır. Üretimin sağlanabilmesi için gramer tabanlı kural gruplarının oluşturulması gerekmektedir. <!-- Bu bağlamda kuralların oluşturulabilmesi için Trabzon Ortahisar konutlarının özellikleri ve rölöveleri incelenerek konutlar hakkında detaylı bilgi birikimi elde edilmiştir. Mevcut konutlar ve genel olarak geleneksel Ortahisar konutları üzerinden yapılan inceleme sonucunda genel karakteristikler ve bu karakteristikler ile ilişkili mevcut yapılardan elde edilen oranlar kuralların oluşturulmasında kullanılmıştır. -->Yordamsal modellemede kural grupları diye nitelenen ifade üç boyutlu modelleri oluşturan bilgisayar kodlarıdır. Kullanıcının modeli kendisinin oluşturduğu geleneksel modelleme yazılımlarından farklı olarak yordamsal modellemede bir yapının veya yapı türünün semantik tanımlamasının programlama dillerini kullanarak bilgisayara tanıtılması ile modeller üretilmektedir. Bu sadece teknik yönden değil kuramsal olarak da farklılıklar ortaya koymaktadır. Seçilen modelleme yöntemi sadece maliyet ve estetik çıktısını değil; bilginin nasıl seçildiği, işlendiği ve nelerin bilgi olarak değerlendirildiği gibi hususları da etkilemektedir [@Saldana:2015el].

Yordamsal modelleme kural tabanlı otomatik veya yarı otomatik içerik üretmeye yönelik bir yöntem olup çeşitli alanlarda doku, bitki, arazi, nehir, bina, kent, yol ağları gibi modellerin oluşturulmasında kullanılmaktadır. <!-- İçerisinde L-sistemler (Lindenmayer sistemleri), fraktallar, biçim gramerleri ve üretken sistemler gibi birden fazla tekniği barındıran bir ana başlık niteliğindedir. --> 30 yıldan fazla bir süredir üzerine aktif araştırma yapılan konu, çok çeşitli varyasyonları üretebilme potansiyeli ve içerik üretiminde insan gücü etkileşimini azaltması ile mimarlık, oyun ve film endüstrisi sanal ortamlarında cazip bir yöntem olarak görülmektedir [@Schinko:2015gn].

Yordamsal modeller bir binanın tasarım stilini veya kültürel bir dönemin tasarım ve yapım bilgilerini kodlamak için kullanılabilmektedirler. En önemli avantajlarından birisi tekil bir yapının detaylı şekilde rekonstrüksiyonunu yapabilmesidir. Bunun yanında aynı tasarım ve yapım kurallarını paylaşan çok sayıda benzer modelleri üretebilmektedir. Yordamsal modellerin üretiminde Lindenmayer sistemi, fraktal, split gramer, biçim grameri gibi birçok üretken sistem kullanılmaktadır. Yordamsal modelleme ile bina modellerinin oluşturulmasında özellikle yordamsal cephe üretimi kullanılmaktadır. Model üretimi iki boyutlu parsel hattının girdi olarak sisteme tanıtılması ile başlamaktadır.

Yordamsal modelleme tekniğinin bir diğer avantajı ise modellenen bina veya obje hakkında uzman düzeyde bilgiye sahip olunmasını sağlamaktadır. Mimaride kullanılan yapı tiplerine ait sınıflandırma şemalarının ve tablolarının kod içine aktarımı gerekmektedir. Bu da günümüz kentlerinde o veya bu şekilde kaybettiğimiz geleneksel yapıların kurallarının elde edilip, kayıt altına alınmasını sağlamaktadır. Koruma anlamında sunduğu olanağın yanında geleneksel doku içinde tasarım yaparken temel olarak alınacak verileri de sağlamış olmaktadır. Kuşkusuz ki bu yöntem klasik yöntemlere göre geleneksel yapı karakteri üzerine daha fazla bilgi sunmaktadır.

Yordamsal modeller semantik bir yapıya sahiptirler ve bu özellikleri ile simülasyon ve planlama için geleneksel modellere göre daha uygundurlar. Günümüz kentsel yenileme ve kentsel canlandırma projelerinde kullanımları da birçok varyasyona ve analiz olanağına kısa sürede imkân sağlamaktadır. Aynı şekilde tekil birimler içinde çeşitli öneriler sunması bu önerilerin yeni tasarım yorumları için altlık oluşturmaktadır.

Bu bağlamda gün geçtikçe sayıları azalan geleneksel Trabzon Ortahisar  konutları örnek çalışma alanı olarak incelenecektir. Ortahisar Mahallesi Trabzon'un tarihi kent çekirdeğinin biçimlendiği bölgeyi ihtiva etmektedir. Kentin geleneksel mimari karakterini barındıran bölge kent kimliği ve kültürel mirası açısından önem arz etmektedir.

Bu çalışma geleneksel Trabzon Ortahisar konutlarının bir split gramer türevi olan CGA (Computer Generated Architecture) gramerinin oluşturulması ve parametrik olarak üretilmesini amaçlamaktadır. Trabzon kenti içinde bulunan geleneksel konutlar üzerinde yapılmış rölöve çalışmaları ve akademik çalışmalar proje için gerekli ana veriyi oluşturmaktadır. Bu veriler üzerinden çalışmanın ilk bölümü için analiz-sentez yöntemi kullanılacaktır. İkinci aşama için biçim gramerleri hazırlanacaktır. Hazırlanan biçim gramerleri üzerinden CGA biçim grameri bilgisayar ortamında kodlanacaktır.

<!-- Bunun için mimarların aktif olarak kullandığı ve tanıdığı Rhinoceros programı üzerinde çalışan Grasshopper platform olarak seçilmiştir. Grasshopper için yazılmış birçok eklenti bulunmaktadır ve model üzerinde interaktif olarak analiz yapma olanağı sunmaktadır. Bunun yanında gelişmeye açık bir platform olması da tercih sebebidir. Bu kapsamda Grasshopper üzerinde C\# programlama dili üzerinden geliştirilecek kodlar ile Trabzon evlerinin kurallarını içeren bir eklenti geliştirilecektir. -->

## Amaç ve Kapsam

Önerilen çalışma yordamsal modelleme yöntemi kullanılarak geleneksel Trabzon Ortahisar konutlarının CGA grameri kodlamasını ve tasarım altlığı olarak sunulacak modellerin parametrik olarak üretilmesini amaçlamaktadır.

Hedefler;

<!--Kütlesel cephe ve plan üretiminin beraber yapılacağı bütünleşik bir yöntem geliştirmek.-->

<!--Geliştirilecek yöntem ile kütlesel cephe özelliklerinin yanında plan şeması da oluşturularak iç mekanların kullanım amacına, mekanların birbirleriyle olan orantılarına, aydınlanma ve sirkülasyon gibi özelliklerine ait bilgiler sağlamak.-->

<!--Rhinoceros üzerinde çalışan Grasshopper için geleneksel Trabzon evlerini parametrik olarak üretecek bir eklenti geliştirmek.-->

1. Tarihi dokuda yeni yapılacak binalar için geleneksel dokuya ait referans bilgi sağlamak.

2. Üretilecek modellerin varyasyonlarını yeni tasarımlar için altlık olarak sunmak.

3. Geleneksel Trabzon Ortahisar konutlarına ait kütle ve cephelerin oluşumunu tanımlayan  biçim gramerini oluşturmak.

Bu çalışma kapsamında geleneksel Trabzon Ortahisar konutlarının yordamsal modelleme için kural gruplarının çıkarılması ve modellerinin üretilmesi yer almaktadır. Çalışma kütle ve cephe bazında olup, modeller için plan üretimi yapılmamaktadır. Elde edilen veriler dahilinde yeterli sayıda plan rölövesine ulaşılamadığı için plan üretimi bu çalışma kapsamı dışında tutulmuştur.

Üretilen taslak modeller birbirinden bağımsız olarak türetilmektedir ve sokak dokusu üzerine bir çalışma yapılmamıştır. Parsel ile olan ilişkiler ve sokak-komşuluk ünitesi oluşumu için gerekli araştırmalar yapılarak bu çalışmanın üzerine ek olarak geliştirilebilir. <!-- Sokak kütle arasındaki oransal ilişkiler de bu sayede algılanmış olacaktır. -->

## Çalışmanın Özgün Değeri

Kentler tarih boyunca geçirdikleri her dönemin sosyo-kültürel, estetik anlayışları ve teknolojik olanakları tarafından evrilerek şekillenmişlerdir. Bu devinim sürekli olarak devam etmektedir. Kentlerin gelişim ve şekillenişindeki en önemli etkenlerden biri de yeni yapılaşmadır. Kentlerin tarih boyunca oluşmuş  dokusuna yeni yapılaşma yapmak daimi olarak bir tartışma ve araştırma konusu olmuştur.

Ondokuzuncu yüzyılın ikinci yarısından itibaren gözlemlenen teknolojik gelişmeler yapı kültürünün alt yapı, ulaşım, üretim teknolojileri, yapım teknikleri, malzeme vb. faktörlerinde hızlı bir değişime sebep olmuştur. Daha öncesinde kentlere eklemlenen yeni yapılaşmalar farklı dönemlerde sınırlı değişimlere uğrayan geleneksel yöntemler ve malzemeler kullanılarak üretildiğinden ölçek, kütlesel oranlar, malzemeler ve mekansal özellikler bakımından uyumlu bir doku sağlamıştır. Teknolojideki hızlı gelişmeler ile beraber üretilen yeni yapılaşmalar önceki döneme ait kentsel dokular ile aykırılaşmaya ve tartışmalara sebep olmuştur [@Altnoz:2010wm].

Bu bağlamda tarihi dokuları oluşturan ve belirli bir ortak karakter taşıyan yapıların tasarım dillerini analiz eden ve ortaya koyan bir çok çalışma yapılmıştır. İlk olarak Stiny ve Mitchell [-@Stiny:1978cl] Palladio evleri grameri çalışmasını yayınlamıştır. Ardından gelen süreçte Wright'ın Praire evleri [@Koning:1981bd], Buffalo'nun bungalovları [@Downing:1981dx], Queen Anne evleri [@Flemming:1987js], Tayvan yöresel konutları [@Chiou:1995gj], geleneksel Türk konutları [@Cagdas:1996ft], Saraybosna Hayat evleri [@Colakoglu:2005kc], geleneksel Mardin evleri [@Torus:2011hu] gibi çalışmalar tekil ve toplu olarak mevcut dokuların anlamsal değerini sürdürebilmeyi ve kimlik kaybını önlemeyi hedeflemişlerdir.

Bu çalışmada da aynı hedefler göz önünde bulundurularak yeni yapılaşmalar için tarihi dokunun yapılaşma oranlarını ve ölçeğini tasarım altlığı olarak sunabilmek hedeflenmiştir. Önceki çalışmalar bitmiş bir sonuç ürün verirken bu çalışma üzerinde interaktif olarak değişiklik yapılabilir esnek bir tasarım altlığını sonuç ürün olarak vermektedir. Tasarımcıya verilen bu esneklik çeşitli parametreler aracılığıyla sunulmaktadır. Bu sayede tasarımcı çevre dokunun karakterine uygun tasarım yaparken kendi tercihleri doğrultusunda hareket edebilmektedir.

<!--

Çolakoğlu, Birgül, “An Informal Shape Grammars for Interpolations of Traditional Bosnian Hayat Houses in a Contemporary Context”, paper presented in Generative Art Conference, December 11- 14, 2002, Milano Polytechnic University. (Generative Art, http://www.generativeart.com/on/cic/papersGA2002/15.pdf, last visited on October 2010) Furthermore, information on her and colleagues’ studies on traditional Mardin tissue and new building design through utilization of shape grammar are available online on Yıldız Teknik Universitesi, http://www.bot.yildiz.edu.tr/_sites/mardin/index.htm, last visited on October 2010. 

Yöresel anlamda bugüne kadar yapılan çalışmalarda neler var?
Sivrihisar geleneksel ve yeni kent dokusunun analizi
Öz Sivrihisar’daki geleneksel ve yeni kent dokusu içinde kamusal, yarı kamusal ve özel alan bağlamında kent kurgusunu ve kentsel elemanlar arasındaki bağıntı ve odakları tespit etmek için biçim grameri ile analiz yapmıştır.
Geleneksel Sille Evleri
Erkış Sille yerleşkesinin konutlarının tipolojilerini çıkarmak üzere biçim grameri metodu kullanılmıştır. Bu yöntem ile belirli algoritmik düzene sahip olan sivil mimarileri analiz ederek kuralları belirlenmiştir.
Amasya Yalıboyu Evleri
Güzelci bu çalışmasında Amasya Yalıboyu evlerinin biçim gramer strüktürünü analiz ederek kural setleri oluşturmuş̧ ve üretim sürecini tanımlamıştır. Amasya Yalıboyu evleri ile aynı dile sahip iç̧ ve dış̧ sofalı yeni evler üretmiştir.
Bodrum Geleneksel ve Güncel Konutlarının Analizi
Karakoyun Bodrum üzerine yaptığı çalışmasında 8 adet tescilli yapının tipolojik ve geometrik analizini yaparak elde ettiği bilgiler üzerinden oluşturduğu biçim grameri kuralları ile güncel konutların geleneksel dokuya uyumunu tespit etmeyi hedeflemiştir.
Çağdaş̧ Mardin konut yerleşimi
Özbek bu çalışmasında analiz ettiği geleneksel Mardin evlerinin biçim gramer kurallarını çıkarıp günümüze uyarlayarak Mardin’de çağdaş konut üretimi için alternatif ürünler ortaya koymuştur.

-->

## Çalışmanın Yöntemi

Çalışmada geleneksel Ortahisar konutlarının CGA grameri kodlaması ve tasarım altlıklarının parametrik olarak üretilmesi amaçlanmaktadır. CGA grameri bir split gramer türevidir ve yordamsal modelleme tekniğinde kullanılan araçlardan biridir. Yordamsal modelleme ile otomatik model üretilebilmesinin yanında kullanıcının üretim sürecinde kısıtları seçebildiği yarı otomatik bir sürece de olanak vermektedir.

CGA grameri kodlanmadan önce geleneksel Ortahisar konutlarının tipolojik tasarım analizi ve sentezi için öncelikle biçim gramerleri bir araştırma aracı olarak kullanılmıştır. Bu sayede konutların tipik özellikleri kurallar yardımıyla açıklanmıştır ve taslak üretmek için zemin hazırlanmıştır. 

Çalışma süreci iki kademeli olarak işlemektedir;

1. Biçim gramerinin oluşturulması

   Çalışmanın ilk bölümünde analiz-sentez yöntemi kullanılmıştır ve ikinci aşama için gerekli olan biçim grameri verileri hazırlanmış olacaktır.

   * Geleneksel Trabzon Ortahisar konutlarına ait verilerin toplanması:
      Çalışma için gerekli olan Trabzon geleneksel evlerine ait veriler akademik ve profesyonel çalışmalardan toplanmıştır. Temel Kaynaklar;

       - Trabzon Kültür ve Tabiat Varlıklarını Koruma Bölge Kurulu Müdürlüğü Arşivi
       - KTÜ Mimarlık Bölümü Doğu Karadeniz Arşivi
       - Trabzon geleneksel evleri üzerine yapılmış akademik çalışmalar
       - İstanbul Büyükşehir Belediyesi BİMTAŞ A.Ş. Rölöve çalışmaları
       <!--Trabzon geleneksel evleri üzerine rölöve çalışması yapmış ofis arşivleri-->

   * Analiz çalışması:
      Evlere ait veriler toplandıktan sonra aşağıdaki listede belirtilen özelliklere göre analizleri yapılmıştır.

       - Yapı taban alanı
         <!--Yapı hacmi, Plan tipi-->
       - Kat sayısı ve yükseklikleri
       - Cephe karakteri
       - Cephe çıkmaları
       - Cephe elemanları
       - Çatı formu ve eğimi

         <!-- Parsel kullanımı, Bahçe içi yerleşim -->

   * Sentez çalışması:
      Çıkarılan veriler analiz edilen başlıklara göre tablolara dökülerek kural oluşturmak için gerekli sayısal özellikler organize edilmiştir. Bununla beraber kütle ve cephelere ait biçim grameri kuralları hazırlanmıştır.

2. CGA gramer kodunun oluşturulması

   İkinci bölümde geleneksel Ortahisar konutları için hazırlanan biçim grameri kuralları üzerinden CGA grameri kodlaması yapılmıştır. Üretilen kod ESRI firmasına ait CityEngine yazılımı üzerinde çalıştırılmaktadır.

Çalışmanın temelini oluşturan veriler Trabzon Büyükşehir Belediyesi ve Trabzon Rölöve ve Anıtlar Müdürlüğü arşivlerinden toplanan rölövelerden elde edilmiştir. Elde edilen rölöveler geleneksel yöntemlerdeki gibi çizimler üzerinden incelenerek ve ölçülerek yapı tektoniği hakkında bilgi edinilmiş ve gerekli sayısal değerler tablolara dökülmüştür. Veriler ve işlenişi ile ilgili bilgi yapılan çalışmalar kısmında daha detaylı anlatılmıştır.

Yapı tektoniğinin incelenmesinin ardından biçim grameri kuralları hazırlanmıştır. Oluşturulan gramer Stiny ve Mitchell [-@Stiny:1978cl] tarafından tanımlanan üç test ile sınanmıştır. Bu testlere göre bir gramerin açıklayıcı ve öngörücü olup olmadığı doğrulanmaktadır. Öncelikle bir gramer, grameri oluşturan yapıların tasarımlarının altında yatan ortak özellikleri ortaya koymalıdır. İkinci olarak grameri oluşturan yapıların dışında bir yapının ortak tasarım diline ait olup olmadığını belirleyen kriterleri sağlamalıdır. Üçüncü olarakta yeni bir yapının nasıl tasarlanacağını belirtmelidir. Sırasıyla bu testler açıklayıcı, analitik ve sentetik test olarak adlandırılmaktadır.

Biçim grameri kuralları oluşturulurken kurallar ile beraber kısıtlar tanımlanmıştır. Bu kısıtlar bazı özel durumların bağlamını ve taslak önerilerini kısıtlamak için ilişkileri tanımlamaktadır. Ayrıca kısıtlar değişkenler arası ilişkileri tanımlamaktadır ve yapılara ait tasarım bilgisini mantık kuralları ile gramer kurallarına aktarmaktadır.

Bu doğrultuda CGA grameri kodlanırken değişkenler CGA grameri içerisinde bazıları sabit bazılarıda alt ve üst limitleri belirtilerek tanımlanmıştır. Limitleri ile tanımlanmış değişkenler tasarımcının kontrolünde değiştirilebilmektedir. Sabit olanlar ise tasarımcının kontrolü dışında bilgisayar tarafından seçilmektedir. 

![Çalışmada izlenen süreç döngüsü. \label{tezsurec}](source/figures/TezSurec.pdf){width=100%}

Çalışmada izlenen süreç şekil \ref{tezsurec}'de görsel olarak aktarılmıştır. Sürecin birinci aşaması biçim gramerlerinin oluşturulması ile sonlanmaktadır. İkinci aşamada ise CGA kodu oluşturulmaktadır. Şekilde model üretimi evresinden tekrar verilerin toplanması evresine doğru bir döngü oluşmaktadır. Bu döngü üretilen modellerde eksiklik yaşanması durumunda tekrardan yeni verilerin eklenerek süreç sonucu üretilecek modellerin geliştirilmesi için bulunmaktadır.

Verilerin toplanması ve verilerin analizi bir sonraki bölümde ele alınmıştır. Biçim gramerleri, split grameri ve CGA grameri, Ortahisar bölgesine ait genel bilgiler ve geleneksel Ortahisar konutlarının özellikleri çalışmanın bir sonraki bölümünde sunulmuştur. 

\newpage