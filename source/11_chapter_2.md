# YAPILAN ÇALIŞMALAR

\thispagestyle{empty}

## Biçim Gramerleri

Biçim gramerleri 1972 yılında *George Stiny* ve *James Gips* [-@Stiny:1972tt] tarafından tanıtıldı. Tasarımları analiz etmeye ve üretmeye yarayan tasarım amaçlı ilk algoritmik sistem olan biçim gramerleri kurallarını direk biçimler üzerinden tanımlamaktadır. Kompütasyon teorisi ve görsel-mekansal düşünme yöntemi olarak iki farklı düzlemde açıklanmaktadır [@Tepavcevic:2012bl].

Yazı ve sembollere bağlı bir kompütasyon süreci yerine direk olarak biçimi kullanması ve görsel olarak çalışan bir sistem olması diğer üretken sistemlerden temelde ayrışmasını sağlar [@Knight:2012ue]. Kompütasyon sürecini tamamen görsel olarak üretim kuralları üzerinden gerçekleştirmeyi sağlayan biçim gramerleri bir başlangıç biçimi ve kural dizilerinden oluşmaktadır (Şekil \ref{shapegrammarrule}). Biçimler iki boyutlu nokta, çizgi, düzlem olabileceği gibi üç boyutlu hacimler veya bunların kombinasyonları şeklinde de olabilirler. Biçimler ayrıca ek bilgi gösteren etiketlere ve bazı özelliklerinin büyüklüğünü gösteren ağırlıklara sahip olabilirler [@Stiny:1980it]. Kurallar ise aralarındaki ok ile ayrılan bir çift biçimden oluşmaktadır. Kuralların sol kısmında başlangıç biçimi, sağ kısmında ise kural uygulandıktan sonra dönüşeceği biçim tanımlanmaktadır. Halihazırdaki biçimin herhangi bir parçası tanımlı kurallardan birinin sol kısmında belirtilmiş biçimsel şartı sağladığında sağ kısmında tanımlı biçim ile değiştirilerek biçim geliştirilir.

![Örnek biçim grameri kuralı [@Stiny:2006tq]. \label{shapegrammarrule}](source/figures/shape_grammar_rule.pdf){width=100%}

Biçim gramerleri görsel-mekansal düşünmeyi temsil eden bir biçimcilik olarak da tanımlanabilmektedir. Görsel tasarım gramerleri olarak da adlandırabileceğimiz biçim gramerleri dünyaya öğrenilen veya dayatılan tanımlamalar yerine belirli bir zamanda pratik bir anlamı olan tanımlamalardan bakabilme düşüncesidir [@Ozkar:2009ga].

Tanıtımından sonra *Gips* [-@Gips:1975jg] doktora tezinde biçim gramerlerinin bilgisayar uygulamalarını geliştirdi, *Stiny* [-@Stiny:1975fj] ise matematiksel temelleri üzerine yoğunlaştı. *Stiny* [-@Stiny:1976im] tezinin ardından yazdığı *Two exercises in formal composition* adlı makalede biçim gramerlerinin kullanımını iki örnek üzerinden açıkladı ve bu örnekler daha sonra yapılan çalışmalara temel oluşturdu. Bu örneklerden ilki biçim gramerlerinin üretken bir sistem olarak yeni tasarım dili veya tarzı oluşturmak için özgün hali ile nasıl kullanılabildiğini açıklarken ikinci örnek ise mevcut bir tasarım dilinin veya tarzının biçim gramerleri kullanılarak analizinin nasıl yapılabildiğini göstermektedir. Ayrıca hem analitik hem de sentetik kullanıldığı örneklere de rastlamak mümkündür [@Knight:1999uf].

### Analiz Aracı Olarak Kullanımı (Analiz Gramerleri)

Biçim gramerlerinin ilk kez analiz aracı olarak kullanımı *Stiny* [-@Stiny:1977im] tarafından Çin buz ışını pencere tasarımları üzerine yaptığı çalışmada ortaya konuldu. Bu çalışma ayrıca biçim gramerlerinin parametrik tasarım ile entegre edilerek parametrik biçim gramerlerinin tanımlandığı çalışma oldu. Beş adet kuraldan oluşan gramer Çin buz ışını ızgaraların bir araya gelme düzenini açıklamayı, örnek ızgaralar oluşturmayı ve sayısız yeni ızgara düzenleri oluşturmayı başardı. Ertesi yıl *Stiny* ve *Mitchell* [-@Stiny:1978cl] biçim gramerlerini *Pallodio* stili üzerinden test ederek ilk kez bir mimari üslubun analizinde kullandılar. "Palladio Grameri" kurallarını *Andrea Palladio* tarafından 1570 yılında yazılmış *Quattro Libri dell'Architettura*'da bulunan villa planı örneklerini inceleyerek tanımladılar. Parametrik biçim gramerlerini kullanarak villaların zemin kat planlarını önerdikleri sekiz aşamalı bir süreç ile oluşturdular.

Bu çalışmanın ardından gelen yirmi yıllık bir dönemde biçim gramerleri neredeyse tamamen bir analiz aracı olarak mimarların tarzını, yöresel mimariyi, sanat stillerini vb. açıklamada kullanıldı.

Bu çalışmalar arasında *Giuseppe Terragni*, *Frank Lloyd Wright*, *Glenn Murcutt*, *Christopher Wren* gibi mimarların tarzları analiz edildi [@Flemming:1981hm; @Koning:1981bd; @Hanson:1986ty; @Buelinckx:1993io].

Yöresel mimari analizlerine bakıldığında Japon çay odaları, Buffalo'nun bungalovları, Queen Anne evleri, geleneksel Tayvan evleri, geleneksel Türk evleri, sıra evler, klasik Osmanlı dönemi camileri ve Mughul bahçelerinin peyzaj mimarisi çalışmaları bulunmaktadır [@Knight:1981gp; @Downing:1981dx; @Flemming:1987js; @Chiou:1995gj; @Cagdas:1996ft; @Cagdas:1996fe; @Aksoy:2001wz; @Stiny:1980dya].

Sanat stillerinin analizini yapan çalışmalarda *Richard Diebenkorn*, *Georges Vantongerloo* ve *Fritz Glarner*'ın tabloları, *Hepplewhite* tarzı sandalyelerin arkalıklarının tasarımı, *Frank Lloyd Wright*'ın pencere tasarımları ve antik Yunan çömleklerinin süsleme tasarımları incelenmiştir [@Kirsch:1986bi; @Knight:1989ec; @Knight:1980cl; @Rollo:1995bz; @Knight:1986wu]. *Wright*'ın mimari tarzı için hazırlanan gramer ilk üç boyutlu mimari gramer çalışması olması açısından önemlidir.

Sonraki dönem çalışmalarında Benros vd. üç ayrı tarz olan Pallodio villaları, Malagueira konutları ve Prairie konutlarını oluşturdukları tek gramer, Osmanlı camilerinin ontolojisini kullanan tipolojik tanımlama (description) gramerleri ve tipolojik tanımlama gramerleri için genel gösterim önerisi göze çarpmaktadır [@Benros:2014bx; @Stouffs:2015if; @Stouffs:2016ip].

<!-- [@Aksoy:2001vq] Örneklere buradan bakılabilir -->

### Tasarım Aracı Olarak Kullanımı (Özgün Gramerler)

Biçim gramerlerinin analiz aracı olarak kullanımı yukarıdaki örneklere bakıldığında önemli ölçüde etkin olduğunu göstermektedir. Buna karşı başlangıçtan itibaren tamamen yeni tasarım dilleri oluşturma konusunda şaşırtıcı bir şekilde sınırlı sayıda örneğe rastlanmaktadır. Bu anlamda ilk çalışma *Stiny* ve *Gips* [-@Stiny:1972tt] tarafından tablolar üzerine yapılan biçim gramerleri oldu. *Stiny* ve *Gips*'in tezleri ve beraber yazdıkları *Algorithmic Aesthetics* kitabı da yine aynı konu üzerinde biçim grameri formalizmini örnekliyordu [@Knight:1999uf].

Bu çalışmalar haricinde *Stiny*'nin [-@Stiny:1976im] iki boyutlu formal kompozisyonlar ve ilk üç boyutlu biçim grameri çalışması olan Froebel'in yapı blokları üzerine çalışmaları örnek oluşturmaktadır [@Stiny:1980kq]. Froebel yapı blokları üzerine olan çalışma özgün gramerleri kullanarak sıfırdan yeni bir tasarım dili oluşturmak için izlenecek işleyişi tanımlamaktadır. Yeni tasarım dilini oluşturmak için önerilen işleyişte biçim sözlüğü, mekansal ilişkiler, biçim kuralları, başlangıç biçimi ve biçim gramerlerinin aşamalı olarak oluşturulması gerekmektedir. Bu alanda mimarlık ve diğer dallarda çeşitli çalışmalar kısıtlı sayıda gerçekleştirildi [@Knight:1989ex; @Knight:1992tp; @Knight:1993jka; @Knight:1994hx].

### Analiz Sonucu Tasarım Aracı Olarak Kullanımı (Hibrid Gramerler)

Özgün gramelerin tamamen baştan oluşturulması teori üzerinde olmaktadır [@Knight:1999uf]. Uygulamada ise yeni tasarım dilleri eski ve güncel dillerin değiştirilmesi, geliştirilmesi veya birleştirmesi gibi işlemler ile oluşturulur. Knight [-@Knight:1981ky] önerdiği mevcut tasarım dilleri üzerinden yeni tasarım dilleri üretme yönteminde ilk önce mevcut dil için bir gramer çıkartılarak analiz edilir, çıkarılan gramerin kuralları dönüştürülür ve dönüştürülen kurallar yeni bir gramerin ve dilin temeli haline gelir. Knight bu yöntemin bilinen dillerin tarihsel evrimini başarılı bir şekilde tanımlamak ve yeni tasarımlar geliştirmek için kullanabileceğini belirtmektedir. Bu nedenle bu yöntem hem analitik hem sentetiktir. Knight *Transformations in Design* adlı kitabında bu yöntemi kullanarak Frank Lloyd Wright'ın çalışmalarında, De Stijl resminde ve antik Yunan süsleme tasarımlarında stilistik değişimleri analiz etmek için uygulamaktadır [@Knight:1999uf]. Flemming [-@Flemming:1990tn] Knight'ın yöntemine benzer bir yöntemi bilgisayar üzerinde mimari kompozisyonları öğretebilmek için kullanmmıştır.

Bu gramer yapısının örneklerine baktığımızda Çolakoğlu [-@Colakoglu:2001wi] 18. ve 19. yüzyılda Saraybosna'da Osmanlı tarzında tasarlanan geleneksel “Hayat” evlerinin gramerini oluşturarak tarihi bağlama uygun yeni formların üretimini sağladı. Duarte [-@Duarte:2005gd] 1977 ve 1996 yılları arasında Siza tarafından Malagueira için tasarlanmış otuzbeş konut üzerinden Siza'nın da desteğini alarak oluşturduğu gramer ile Siza'nın tasarım mantığına yatkın çeşitli yeni tasarımlar üretebildi. Marakeş Medine'de *Zaouiat Lakhdar* bölgesi için geliştirilen yerel konut ve kentsel form üreten gramerler, *rabo-de-bacalhau* bina tipolojisindeki evlerin rehabilitasyonu için geliştirilen dönüşüm grameri hibrid gramerlere örnek oluşturmaktadır [@Duarte:2006wg; @Duarte:2007eq; @Eloy:2014kn].

<!--
[@Sonmez:2018jx] Eklenmeyen referans listesi.
[25] Correia R, Duarte J, Leitão A. GRAMATICA: A general 3D shape grammar inter- preter targeting the mass customization of housing. In: Digital physicality: Proceedings of the 30th eCAADe conference, Prague, Czech Republic. 2012. Vol. 1. p. 489-96.
[26] CorreiaRC.DESIGNA-ashapegrammarinterpreter[Ph.D.thesis].TULisbon: Instituto Superior Técnico; 2013.
[27] GeroJS,LouisSJ,KunduS.Evolutionarylearningofnovelgrammarsfordesign improvement. AI EDAM 1994;8(2):83–94. http://dx.doi.org/10.1017/S089006040000069X.
[28] Shea K, Cagan J. Innovative dome design: Applying geodesic patterns with shape annealing. AI EDAM 1997;11:379–94.
[29] RosenmanMA,GeroJS.Evolvingdesignsbygeneratingusefulcomplexgene structures. In: Bentley PJ, editor. Evolutionary design by computers. San Francisco, CA: Morgan Kaufmann; 1999. p. 345–64.
[30] GroblerF,AksamijaA,KimH,KrishnamurtiR,YueK,HickersonC.Ontologies and shape grammars: Communication between knowledge-based and gener- ative Systems. In: Gero JS, Goel AK, editors. Design computing and cognition ’08. Netherlands: Springer; 2008. p. 23–40.
[31] GranadeiroV,DuarteJP,CorreiaJR,LealVMS.Buildingenvelopeshapedesign in early stages of the design process: Integrating architectural design systems and energy simulation. Autom Constr 2013;32:196–209. http://dx.doi.org/10.1016/j.autcon.2012.12.003.
[32] MandićM,TepavčevićB.Analysisofshapegrammarapplicationasatoolfor urban design. Environ Plann B: Plann Des 2015;42(4):675–87. http://dx.doi.org/10.1068/b130084p.
[33] Vitins BJ, Axhausen K. Shape grammars overview and assessment for trans- port and urban design: Review, terminology, assessment, and application. J Transp Land Use 2016;9(1):. http://dx.doi.org/10.5198/jtlu.2016.620.

* [@Ozdemir:2014tm] Standart ve Parametrik Biçim Grameri Örneklerinin Değerlendirilmesi **MUTLAKA BAK TÜRKİYEDEN ÖRNEKLER**
* [@Knight:1999uf] HISTORY OF APPLICATIONS IN ARCHITECTURE AND THE ARTS
* [@Tepavcevic:2012bl] Shape ten procedural modeling e kadar herşey
* [@Sonmez:2018jx]
* Yenileri ve Türkiye'den örneklerinde eklenmesi lazım

[@Ozkar:2009ga] Islamic patterns sayfa 67 bir göz at
[@Josefsson:2013fy] Foster + Partners Kuwait havaalanı
-->

### Split Grameri

Wonka vd. [-@Wonka:2003bn] mimari modelleri oluşturmak için özel bir set grameri[^1]olan parametrik split gramer yöntemini geliştirmişlerdir. Yazarlar yapıların yatayda ve düşeyde sürekliliğe sahip olan yapı elemanlarından oluştuğunu ve buna benzer bir etkiyi split grameri kontrol ederek elde edilebileceğini belirtmişlerdir. İsmini bölümleme işleminden alan ve iki üretim kuralı olan bu yöntem  basit geometrilerden oluşan üç boyutlu bir kütlenin önce yüzeylere ve yapısal elemanlarına kadar bölümlenip ardından bölümlenen her biçim önceden tanımlanan geometri ve malzemeler ile yer değiştirmesine dayanmaktadır (Şekil \ref{splitGrammar}). Bölümlenme işlemi sonlandırıcı tanımlı biçimlere ulaşana kadar devam etmektedir ve muhtemel düzeni önceden tanımlı-sabit olduğundan dolayı kararlıdır.

[^1]: [@Stiny:1982cn]

Set grameri üretim kurallarını görsel işlem yerine etiketli biçimler üzerinden işleyen, biçim gramerlerinin basitleştirilmiş halidir [@Stiny:1982cn; @Lienhard:2017jv]. Etiketli bir biçim set gramerinin en küçük (atomik) öğesidir ve alt biçimler barındırmaz. Etiketler sembol olarak kullanılarak üretim kurallarının metinsel olarak yazımını ve bilgisayarda algoritma olarak işlenmesine olanak vermektedir. İdeal olarak, bir biçim grameri uygulaması: görsel bilgi işlemeyi desteklemeli, saklı şekillere izin vermeli (emergence), önceden tanımlanmış parçalara dayanmamalı ve parametrik olmalıdır [@Gips:1999ut]. Set gramerleri biçim gramerlerinin bilgisayar üzerinde işlenmesini kısıtlayan ilk üç özelliğini barındırmamaktadır. Literatürde biçim grameri uygulaması olarak adlandırılan bir çok yazılım ve yazılım denemesi aslında set gramerini temel alarak çalışmaktadır.

![Basit bir Split Gramer kuralı ve üretim süreci [@Sonmez:2018jx]. \label{splitGrammar}](source/figures/splitGrammar.jpg){width=50%}

![Bir cephenin katman detay gösterimi [@Sonmez:2018jx].](source/figures/splitGrammar2.jpg){width=50%}

<!--Bir model içerisinde her katı farklı bir tarz ile modellemeyi mümkün kılmaktadır. Buna örnek olarak zeminde ticari, üst katlarda konut işlevi olan binalar gösterilebilir.-->


<!-- [@Huang:2009ig] -->

### CGA Biçim Grameri

Split gramerler Müller vd. [-@Muller:2006fy] tarafından geliştirilerek CGA gramerleri olarak adlandırılmıştır. Geliştirilen bu yöntemde katı kütle modelleme sistemi ve farklı olarak tanımlanmış birçok modelleme kuralının yanında cephe üretimi zor olan karmaşık kütleler içinde eklentiler bulunmaktadır. <!-- Bununla beraber çatı üretimi ve yönlenmiş kütleler için cephe üretimini de olanaklı hale getirmiştir. --> CGA gramer yöntemi çokgen ile belirlenmiş bir parsel hattını yükseltip katlara bölünmüş bir hacim oluşturarak işleme başlamaktadır. Katların cepheleri biçim kuralları kullanılarak duvar, kapı, pencere gibi bölümlere bölünmektedir. Koşullu ya da tahmini kurallar, biçim parametreleri, rastgele numara üretimi bu yöntem içerisinde çeşitlilik oluşturmak için kullanılmaktadır. CGA bir biçim grameri olması ile beraber aynı zamanda bir programlama dilidir. Örnek bir CGA biçim kuralı aşağıdaki gibi yazılmaktadır.

```CGA
başlangıçŞekli -->
					koşul1: sonuçŞekil0 ... sonuçŞekilM ...
					koşulN: ...
```

CGA gramerlerinin tanımlanmasının ardından yordamsal modellemenin kolaylaştırılması ve daha iyi kullanılabilmesi için devamlı gelişmeler gözlendi. Özellikle cephe modelleri oluşturmak için Müller vd. [-@Muller:2007gu] binaların cephe fotoğrafları üzerinden tekrar eden karoların tanımlanması ile gramer kurallarınının bilgisayar tarafından otomatik çıkarılması için bir yöntem geliştirdi. Lipp vd. [-@Lipp:2008hv] CGA kurallarını kod yazarak oluşturmak yerine yaptıkları yazılım sayesinde üç boyutlu model üzerinden etkileşim ile kodları görsel olarak düzenlemeyi başardılar. Ancak bu gelişmelere rağmen birçok yordamsal modelleme projesi kod yazılarak gerçekleştirildi. Bunlardan bazıları;

- Reconstruction of Puuc Buildings [@Muller:2006hz]
- Reconstruction of Ancient Pompeii [@Muller:2005uf]
- Rome Reborn 2.0: A Case Study of Virtual City Reconstruction Using Procedural Modeling Techniques [@Dylla:2010tm]
- Urban Topography of Magnesia on the Maeander [@Saldana:2015wj].

<!--

[@Zhu:2017vm]

[@Jesus:fi] Related work kısmı

-->

<!--

### Yordamsal Modelleme

#### Yordamsal Cephe Üretimi

Binaların yordamsal üretimi yordamsal modellemenin en gelişmiş alanlarından biridir. Bu alanın alt başlıklarından birisi de yordamsal cephe üretimidir [@Muller:2007gu]. Cepheleri üretmek için split gramer, düzgün [@Xiao:2008er] ve ters [@Bao:2013gk; @Zhang:2013il] çözümleme yöntemleri mevcuttur.

Parish ve Müller [-@Parish:2001ge] ürettikleri dikdörtgen kentsel parseller üzerinden cephelerini oluştururken L-sistemleri kullanmışlardır. Greuter vd. (Greuter vd., 2003) ofis binalarını birden fazla temel biçimin oluşturduğu planları farklı yüksekliklerde kütleler üreterek oluşturmuşlardır. Bu L-sistem örnekleri belirli bir veri grubundan detaylı bina modelleri üretmek için kullanılmışlardır.

Wonka vd. (Wonka vd., 2003) bina modelleri oluşturmak için özel bir biçim grameri olan split gramer yöntemini geliştirmişlerdir (Şekil \ref{splitGrammar}). Yöntem ismini bölümleme işleminden almaktadır. İki üretim kuralı olan bu işlem büyük biçimlerden küçük biçimlerin oluşturulmasını ve yerlerine ilişkilendirilen yeni biçimlerin yerleştirilmesine dayanmaktadır. Bir model içerisinde her katı farklı bir tarz ile modellemeyi mümkün kılmaktadır. Buna örnek olarak zeminde ticari, üst katlarda konut işlevi olan binalar gösterilebilir.

Bu yöntem Müller vd. (Müller vd., 2006) tarafından geliştirilerek CGA gramerleri olarak adlandırılmıştır. Geliştirilen bu yöntemde farklı olarak tanımlanmış modelleme kuralları ve cephe üretimi zor olan karmaşık kütleler için eklentiler bulunmaktadır. Bununla beraber çatı üretimi ve yönlenmiş kütleler için cephe üretimini de olanaklı hale getirmiştir. CGA gramer yöntemi çokgen ile belirlenmiş bir parsel hattını yükseltip katlara bölünmüş bir hacim oluşturarak işleme başlamaktadır. Katların cepheleri biçim kuralları kullanılarak duvar, kapı, pencere gibi bölümlere bölünmektedir. Koşullu ya da tahmini kurallar, biçim parametreleri, rastgele numara üretimi bu yöntem içerisinde çeşitlilik üretmek için kullanılmaktadır. Biçim gramerleri güncel olarak bina üretimi için en gelişmiş yöntem olarak kullanılmaktadır.

Yong vd. (Yong vd., 2004) Çin’in güneydoğu bölgesindeki yöresel yapıları biçim gramerleri ile oluşturdukları bir yöntem ortaya koymuşlar. Diğer biçim grameri yöntemleri tekil bir parsel hattına uygulanmaktayken bu hiyerarşik gramer kentsel ölçekten başlamakta ve akabinde sokaklar, konut blokları, yollar ve daha detaylı modeller de kapılar, pencereler ve çatıları oluşturmaya kadar devam etmektedir.

##### Yordamsal İç Mekan Çözümleme

Yordamsal yöntemler ile plan üretimi gramer tabanlı cephe üretimi yaklaşımlarına göre farklılık göstermektedir. Plan üretimi birçok araştırmacının ilgisini çekmiş ve bu alanda çeşitli yöntemler ortaya konmuştur. Plan üretiminde kullanılan yöntemler gramer, alt birimlere ayırma, kısıtlama çözümlemesi ve makine öğrenimi olarak sıralanabilmektedirler.

Rau-Chaplin vd. (Rau-Chaplin vd., 1996) biçim gramerlerini kullanarak kat planları üretmişlerdir. Biçim gramerleri ile oluşturulan plan şeması kamusal, özel, yarı-özel gibi fonksiyonel bölgelere gruplandırılmış oda birimleri üretmektedir. Gruplandırılmış oda birimlerine sistemde daha önceden tanımlanmış çözümü yapılmış oda planları kullanıcı tarafından seçilip atanmaktadır. Sistemin üretkenliği sisteme tanımlı oda çözümleri ile sınırlanmaktadır.

Hahn vd. (Hahn vd., 2006) alt birimlere ayırma yöntemini kullanarak ofis yapıları oluşturmayı başarmışlardır. Başlangıçta verilen kütle katlara ayrılmış ve ardından kat planlarında koridor alanları ve odalar oluşturulmuştur. Bir başka alt birimlere ayırma uygulamasını Marson ve Musso (Marson ve Musse, 2010) “squarified treemaps” algoritması kullanarak oluşturmuştur. Kullanıcı tarafından belirlenen oda alanları ve işlevleri ile bina sınır hatları belirlendikten sonra kat planı tekrarlanan bir şekilde küçük alanlara bölünmüştür. Bir sonraki aşamasında koridorlar otomatik olarak oluşturulmuştur.

Martin (Martin, 2006) yapı sınırlarını belirleyip bu alanı odalara bölmek yerine ilk önce odalar arasındaki bağlantı ilişkilerini tanımlayan bir şema oluşturmaktadır. Şemadaki düğüm noktaları odaları ve kenarlar odalar arası bağlantıları temsil etmektedir. Şemanın mekânsal planlamaya dönmesi şemadaki düğüm noktalarına belirli ölçüde “basınç” uygulanarak istenen büyüklüğe kadar genişletilerek yapılmaktadır. Bu yöntem ile istenen büyüklükte ve istenilen bağlantıları olan odalar elde edilmektedir.

Charman (Charman, 1993) mekân oluşturma problemini çözümü için kısıtlama çözümlemesi tekniği hakkında bilgiler vermektedir. Önerilen plan çözücü bir aksa hizalanmış çeşitli ölçü, pozisyon ve yönelim parametreleri olan dikdörtgenler ile çalışmaktadır. Kısıtlama çözümleme yöntemi sonuca ulaştırsa da uygulamada karmaşık ve zor bir yöntemdir.

Merrel vd. (Merrell vd., 2010) konut planları üretmek için Bayes Ağları kullanan bir yöntem önermişlerdir. Makine öğrenimi ile oda alanları, oda oranları ve yakınlıklarının olduğu 120 mimari konut programı kodlanmıştır ve stokastik optimizasyon yöntemi ile kat planları oluşturmuşlardır.

Tutenel vd. (Tutenel vd., 2009) Martin’in uyguladığı genişleyerek oluşan kat planı yöntemini semantik çözümleme ile ilişkilendirmişlerdir. Her bir oda tipini sınıflandırmış ve diğer odalar ile olan ilişkilerini semantik kütüphanesinde tanımlamışlardır. Oluşturulacak kat planı için minimum boyutlarda dikdörtgenler kısıtlamaları karşılayacak şekilde yerleştirilmekte ve her oda birbirine dokunana kadar genişletilmektedir. Diğer yöntemlerdeki gibi odalar, alanları ve kısıtlamaları tanımlanabileceği gibi; semantik çözümleme ile beraber içinde yaşayacak ailenin büyüklüğü, aile ihtiyaçları, arazi boyutu veya kat sayısı gibi değerler de odaların oluşturulmasına yeterli olabilmektedir.

#### Yordamsal Cephe Üretiminde Kullanılan Yöntemler

##### Lindenmayer Sistemi

##### Fraktallar



\chapter*{Türkiye'den Örnekler}

 Table: Biçim gramerleri üzerine Türkiye'de yapılan tez çalışmaları (https://tez.yok.gov.tr). \label{TürkiyedenÇalışmalar}

| **Yazar**                  | **Yıl** | **Tez Adı**                                                  |
| -------------------------- | ------- | ------------------------------------------------------------ |
| Nurbin Paker               | 1992    | Mimari tasarımda biçim grameri:metro istasyon tasarımı       |
| Suzan Sanlı                | 1993    | Mimari dil bağlamında bir parametrik biçim grameri           |
| Gülnur Düzel               | 1993    | Sıra ev tasarımı için bir biçim grameri modeli               |
| Hülya Gürpınar             | 1993    | Tek katlı konut tasarımında biçim grameri modeli gecekondu tipi üzerine uygulanması |
| Eda Velibaşoğlu            | 1995    | Mimari bir dilin biçim grameri analizi ve bilgisayar ortamında sunumu |
| Bahar Gücüyener            | 1998    | Boğaziçi yalılarında cephenin biçim grameri                  |
| Senem Tekin                | 1999    | A Shape grammar model for Anatolian madrasah architecture    |
| Meltem Aksoy               | 2001    | Varolan tasarım dilleri ve yeni tasarım dilleri bağlamında biçim gramerleri analizi |
| Zeynep Varol Aksoy         | 2001    | Klasik Osmanlı Dönemi Sinan Camilerinin biçim grameri açısından irdelenmesi |
| Utku Karaman               | 2004    | Klasik Osmanlı camileri için kütle grameri algoritması ve eğitim yazılımı |
| Ebru Ulu                   | 2009    | İslami geometrik örüntü türetimi amaçlı bir biçim grameri modeli |
| Aslı Bökü                  | 2009    | Biçim grameri türetme yönteminin Anadolu Selçuklu geometrik bezemeleri üzerinde denenmesi( örüntü türetme yöntemi olarak biçim grameri) |
| Mine Karakoyun             | 2010    | Bodrum geleneksel ve güncel konut mimarisinin biçim grameri yöntemi ile araştırılması |
| Sinan Savaş                | 2011    | Kısıtlı mekan: Mobilya çözümlerinde çağdaş yaklaşımlar       |
| Orkan Zeynel Güzelci       | 2012    | Amasya Yalıboyu evleri üzerine bir biçim grameri çalışması   |
| Volkan Dalağan             | 2012    | İslâmi yıldız geometrik örüntülerin biçim grameri yöntemleri ile kurallı üretimi |
| Bilal İlkay Aslan          | 2012    | Kültür ve konut ilişkisi; çağdaş konutta geleneksel öğelerin izleri |
| Şahika Özdemir             | 2014    | Biçim grameri ile mağaza tasarımına yönelik bir model önerisi |
| Ezgi Baştuğ                | 2015    | Desen üretimi üzerinden tasarım düşüncesini öğrenme: Hesaplamalı bir çerçeve |
| Şadiye Didem Boztepe Erkış | 2016    | Geleneksel Sille evleri üzerine bir biçim grameri çalışması  |

\chapter*{Bilgisayar uygulamaları}

İdeal olarak, bir biçim grameri uygulaması: (1) görsel bilgi işlemeyi desteklemeli, (2) saklı şekillere (emergence) izin vermeli, (3) önceden tanımlanmış parçalara dayanmamalı ve (4) parametrik olmalıdır [@Gips:1999ut].

[@Li:2018hu]

[@Wortmann:2018bp] Algorithmic complexity of shape grammar implementation

[@Terzidis:2006ud]

[@Knight:2012ue]

Table: Genel yorumlayıcı yazılım listesi [@Eloy:2018hh].

| **Genel Yorumlayıcılar**       | **Referanslar**                               |
| ------------------------------ | :-------------------------------------------- |
| Shape grammar interpreter(SGI) | Krishnamurti (1982)                           |
| Shape generation system        | Krishnamurti and Giraud (1986)                |
| SG interpreter                 | Chase (1989)                                  |
| GRAIL                          | Krishnamurti (1992)                           |
| Shape grammar system           | Stouffs (1994)                                |
| GEdit                          | Tapia (1999)                                  |
| Shape grammar editor           | Work by Shelden in 1996, cited by Gips (1999) |
| GraphSynth                     | Anon (n.d.)                                   |
| U13 shape grammar              | Chau et al. (2004) implementation             |

Table: Spesifik tasarım alanı yorumlayıcı yazılım listesi [@Eloy:2018hh].

| **Spesifik tasarım alanı yorumlayıcıları**      | **Referanslar**                               |
| ----------------------------------------------- | --------------------------------------------- |
| Shepard–Metzler analysis                        | Gips (1974)                                   |
| Simple interpreter                              | Gips (1975)                                   |
| Palladio grammar                                | Stiny and Mitchell (1978)                     |
| Queen Anne houses                               | Flemming (1987)                               |
| Genesis                                         | Heisserman (1991)                             |
| Grammatica                                      | Carlson (1993)                                |
| Genesis (Boeing)                                | Heisserman (1994)                             |
| Basic grammar                                   | Duarte and Simondetti (1997)                  |
| EifForm                                         | Shea (2000)                                   |
| 3D shape grammar                                | Piazzalunga and Fitzhorn (1998)               |
| SG-Clips                                        | Chien et al. (1998)                           |
| 3D Shaper                                       | Wang (1998)                                   |
| Coffee maker grammar                            | Agarwal and Cagan (1996)                      |
| MEMS grammar                                    | Agarwal et al. (2000)                         |
| Shaper 2D                                       | McGill (2002)                                 |
| Yingzao fashi grammar                           | Li (2002)                                     |
| Harley Davidson                                 | Pugliese and Cagan (2002)                     |
| Grammar use and interaction                     | Chase (2002)                                  |
| Buick                                           | McCormack and Cagan (2004)                    |
| Coca-Cola grammar                               | Chau et al. (2004)                            |
| Cross-over vehicle grammar                      | Orsborn et al. (2006)                         |
| Digital camera design parametric grammar        | Lee et al. (2012).                            |
| Malagueira                                      | Duarte (2005), Duarte and Correia (2006)      |
| Shape designer                                  | Wong et al. (2005)                            |
| Marrakech Medina grammar                        | Duarte et al. (2007)                          |
| Tibet Tangka grammar                            | Zhang and Lin (2008)                          |
| Baltimore Row-house                             | Aksamija et al. (2010)                        |
| QI curves                                       | Jowers (2006), Jowers and Earl (2011)         |
| Design synthesis and shape generation           | McKay et al. (2011)                           |
| Urban grammar for Praia                         | Beirão et al. (2009)                          |
| Shape grammar and Tangible augmented reality    | Chen et al. (2009)                            |
| Humanoid grammar                                | Fiedler and Ilčík (2009)                      |
| Shape Grammar Machining Planning                | Ertelt and Shea (2010)                        |
| Interactive 3D Spatial Grammar System (Spapper) | Hoisl and Shea (2011)                         |
| Grappa                                          | Grasl (2012)                                  |
| Thonet chair grammar                            | Barros et al. (2011)                          |
| SG parsing via reinforcement learning           | Teboul et al. (2011)                          |
| Rabo-de-Bacalhau grammar                        | Eloy and Duarte (2015), Strobbe et al. (2016) |
| Entelechy grammar                               | Ligler and Economou (2015)                    |
| Dirksen grammar                                 | Park and Economou (2015)                      |
| Multipurpose chair grammar                      | Garcia and Romão (2015)                       |

[@Sener:2008uh]

**Shape Emergence**

[@Knight:2001ca]



Page 44 [@Gu:2012cg]
**Computational Design Methods and Technologies**
Importantly, shapes in shape grammars are treated as nonatomic and ambiguous. They do not have definite parts and can be freely decomposed and recomposed by the user of a grammar, as a design is being generated. Shape ambiguity in shape grammars goes hand in hand with another singular property of shape grammars – shape emergence. An emergent shape is a shape that is not predefined in a grammar, but one that arises through rule applications. Further, emergent shapes can not only be generated by rule applications, they can also be recognized and used in subsequent rule applications.

Page 65 [@Terzidis:2006ud]
shape grammars contribute rationality, consistency, and traceability where finite production rules are applied. Shape grammars can be associated with linguistic patterns and therefore illustrate meaningful statements that may in turn produce languages of design. However, as shape grammars are based on a clearly defined set of rules leaving no place for ambiguity, they have been used extensively for the generation of patterns, diagrams, and floor layouts.

Semboller yerine biçimleri kullandığından dolayı süreç içinde muğlaklık söz konusu olmaktadır.

 Shape grammars were invented over twenty-five years ago by Stiny and Gips. They were one of the earliest algorithmic systems for creating and understanding designs directly through computations with shapes, rather than indirectly through computations with text or symbols. Over the years, shape grammars have been explored through applications addressing a variety of design problems. The history of these applications in architecture and the arts is sketched in this paper. The roles of shape grammar applications in education and practice are outlined. New and ongoing issues concerning shape grammars in education and practice are discussed. [http://www.mit.edu/%7Etknight/IJDC/frameset_abstract.htm](http://www.mit.edu/~tknight/IJDC/frameset_abstract.htm)



[@Stiny:2006tq] Page 58
I’ve never been an authority on the proper use of shapes—when my first research paper was published, with James Gips.4 This was the official beginning of the subject. Gips and I were doctoral students at Stanford and UCLA, respectively, interested in how you could calculate with shapes. We worked out the idea for shape grammars together, with surprises in mind. That’s what we called ambiguity. But this was a problem when it came to putting shape grammars on a computer. Gips developed a couple of neat programs, but neither of them allowed for ambiguity.5 You could calculate with shapes on a computer only if you could describe them with symbols. You had to segment shapes into lowest-level con- stituents to start. Then there was the combinatorial play with simple things to make complex ones. Meanwhile, I worked out the details of embedding, so that you could calculate with shapes in the same way you see.6 Symbols were unnecessary for shape grammars—on a computer or not.

 Page 4 [@Sonmez:2018jx]
Alternatively, SGs can be interpreted as computing environments, in which the basic elements are shapes, instead of symbols [10]. However, it is not straightforward to implement such systems for automatic derivation through symbolic computation [11]. In a regular SG, all the rules whose left hand sides are satisfied can become activated simultaneously. In the original SG formulation, there is no explicit mechanism to control the application sequence of these rules [12]. For this reason, traditional SG applications have been operated manually or interactively, while recent applications moved towards restricted SGs, which are usually coupled with optimization approaches or other control mechanisms. The latter mostly proceed from a single representation to automatically extract a generative model (Fig. 3). This capability may be exploited for automated problem setting.

 p.171: [@Tepavcevic:2012bl]
In the late 1980s, Harvard Graduate School of Design introduced the first programming course obligatory for architects. TopDown software suitable for architects, was written mainly at UCLA by Robin Liggett and William Mitchell and it partly dealt with shape grammars logic. The course did not achieve expected success because students were asked to engage in the actual coding process [6]. -- Highlighted 19 May 2018

autodesk 1986 da piyasaya sunulduğunda *Lisp* scripting dili ile beraber gelmişti sonrasında **mimarlıkta shape grammar ile görsel kompütasyon** var ancak bilgisayar bunu sağlayamıyor [@McCullough:2006dl] s. 13

 

 

1. Antoni Gaudi ve Nurbs kullanımı [@Karabag:uy; @Burry:2016ij; @Frazer:2016bs]
2. **Bilgisayara yüklenen insan rolleri** [@Vardouli:2012tp; @Terzidis:2006ud] bilgisayarı negroponte associate olarak görmekte terzidis otherness olarak adlandırmakta.

> Menges:2011tm s.11 son paragrafta sibernetiğin gelişmesi ile bilgisayarın insan gibi davranması durumları. Bunu insan rollerine bağlamakta mümkün negroponte ve diğerlerini anlatırken

1. **Güncele doğru kompütasyon araçları** [@Davis:2013vn]

**Mimari tasarımda bilgisayarın rolü 2 alanda toplanmaktadır.** [@Terzidis:2006ud] Page 8

Mimari tasarımda bilgisayarın rolü iki kategoride açıklamak mümkündür. İlk kategori genellikle bir çok mimari

**Biçim Grameri**

[@Knight:2015cq] 1972 den itibaren Stiny ile gelişen biçim grameri tarihi

Geleneksel Türk Evleri (Karaman, 2004) Klasik Osmanlı Camileri için Kütle Grameri (Sharon Sung ve Tseng, 2016) Türkiye’den örnekler (Özkaraduman, 2007) (Torus, 2008) (Güzelci, 2012) (Karabağ, 2010)

-->

## Çalışma Alanının Seçimi

Kentsel gelişim sürecinde kent kimliği hayati bir öneme sahiptir. Küreselleşmenin de etkisiyle şehirler gelişim ve dönüşüm süreçlerinde özgün kimliklerini kaybetme problemiyle karşılaşmaktadır. Bu gelişim ve dönüşüm süreçleri düzgün işletilemediğinde kent okunabilirliğini, kentliler kent hafızasını ve algısını kaybetmektedir. Bu durum kentin tarihi ve kültürel mirasını korumayı güçleştirmektedir.

Ekonomik, sosyal, teknolojik, kültürel değişimler ve yanlış planlama kararları sonucunda Trabzon kenti tarihi kent dokusunda tahribatlara ve kimlik kaybetme tehlikesine maruz kalmıştır. Kentin bir çok bölgesinde, kentsel sit alanları da dahil olmak üzere, bu tahribat ve kayıplar yaşanmakta ve geleneksel konut mirasına ait ürünler gün geçtikçe azalmaktadır.

Bu bağlamda Trabzon kentinin geleneksel dokusuna ait karakteristik örnekleri bir arada bulunduran ve tarih boyunca kent çekirdeğinin biçimlendiği bölge olan Ortahisar mahallesi çalışma alanı olarak seçilmiştir. Çalışma bu bölgedeki geleneksel konut karakterine ait bilgileri yordamsal modelleme yöntemi için gerekli CGA grameri ile kayıt altına almayı ve bölgede yapılması planlanan yeni yapılar için tasarım altlığı oluşturmayı hedeflemektedir.

## Çalışma Alanına İlişkin Bilgiler <!-- Ortahisar’ın Genel Karakteri -->

<!--Bu bölümde alan üzerine yapılan çalışmalar yer alacaktır. Kaynaklardan bölge ve konutlar hakkında bilgiler verilecektir. Ayrıca rölöveler ve fotoğraflarda bu bölümde yer alacaktır. Bu bölümde elde edilen bilgiler ile analizler yapılıp, gramer oluşturulmuştur.-->

![Trabzon'un konum haritası. ](source/figures/TrabzonTurkiye.png){width=100%}

Trabzon Doğu Karadeniz sahil şeridinde doğal bir liman olan Asya ve Ortadoğu transit yolunun başında kurulmuştur. Liman ve ticaret kenti olarak özellikle 7. yüzyıldan sonra ekonomik anlamda bölgenin önemli merkezi olmuştur . Kuzeyde Karadeniz, doğu ve batıda ise derin vadiler ile çevrili kent coğrafi olarak korunaklı bir bölgede konumlandırılmıştır. Güney kısmında doğal bir sınırının olmaması ve savunma ihtiyacından ötürü kent önce Yukarıhisar diye adlandırılan güneydeki en yüksek kısmından başlanarak kuzeye doğru sırayla Ortahisar ve Aşağı hisar kısımlarının inşaa edildiği söylenebilir [@Uspenski:2003ta].

![Ortahisar bölgesinin kentin 1223 yılı öncesi ve 1869 yılına kadar olan tarihlerde konumunu gösteren harita [@Bryer:2011ul]. ](source/figures/TrabzonMap.png){width=100%}

Çalışma alanı olarak seçilen Ortahisar, Zağnos ve Tabakhane vadileri arasında kalan, Trabzon kentinin tarihi çekirdeğinin bulunduğu yerleşim bölgesidir. Mimari yapı kültürü M.Ö. 7. yüzyıla kadar dayanmaktadır ve tarih boyunca kentin idari, dini ve yaşam merkezi olarak hizmet etmiştir [@Tuluk:2010ud]. Tarihi surlar ile çevrelenmiş bölge, farklı dönemlere ait geleneksel sivil mimari örneklerinin yanında anıtsal yapıları da barındırmaktadır. Günümüze ulaşmış Ortahisar sınırları içinde kalan sivil mimari dışındaki önemli yapılar aşağıdaki listede sıralanmıştır.

\newpage

- Askeri Mimari
    - Kent surları
- Dini Mimari
	- Panaghia Chrysokephalos Kilisesi (Ortahisar veya Büyük Fatih Cami)
	- Musa Paşa Cami
	- Ortasaray Mescidi - Saraçzade Medresesi
	- Şirin Hatun Mescidi
- Endüstriyel Mimari
	- Tabakhane Köprüsü
	- Zağnos Köprüsü
- Su Mimarisi
	- Çifte Hamam
	- Çarıkçı-Zade Hacı İsmail Çeşmesi
	- Çeşme (Ortahisar Cami güneyinde)
- Kamusal Mimari
	- Hüseyin Kazaz Kültür Merkezi (Eski Cezaevi Binası)
	- Trabzon Kültür Müdürlüğü (Eski Hükümet Konağı)
	- Gazi Paşa İlköğretim Okulu

![Ortahisar dini mimari örnekleri. Solda Ortahisar Cami ve sağda yıkılmış Şirin Hatun Mescidi [@Ozen:2009wo].](source/figures/DiniMimari.png){width=100%}

![Ortahisar endüstriyel mimari örnekleri. Solda Tabakhane Köprüsü ve sağda Zağnos Paşa Köprüsü. Kaynak: www.eskiturkiye.net](source/figures/EndustriyelMimari.png){width=100%}

![Ortahisar su mimarisi örnekleri. Solda yıkılmış Çifte Hamam ve sağda Ortahisar Cami güneyindeki çeşme [@Ozen:2009wo].](source/figures/SuMimarisi.png){width=100%}

![Ortahisar kamusal mimari örnekleri. Solda Hüseyin Kazaz Kültür Merkezi ve sağda Trabzon Kültür Müdürlüğü binası [@Ozen:2009wo].](source/figures/KamusalMimari.png){width=100%}

Listelenmiş yapılardan kent surlarının yapım tarihi net olarak bilinmemekle beraber 257 yılından önce mevcut olduğu kaynaklarda belirtilmiştir [@Bryer:2011ul]. Surlardan sonra bölgedeki en eski yapı olan ve Ortahisar Cami olarak adlandırılan Panaghia Chrysokephalos Kilisesi 914 yılında inşa ettirilmiştir [@Miller:2007uq]. Bölgedeki diğer anıtsal yapıların inşa tarihleri 13. ve 16. yüzyıl, sivil mimarlık örneklerinin inşa tarihlerinin ise 19. yüzyıl sonları ve 20. yüzyılın ilk çeyreği olduğu bilinmektedir [@Aysu:1977wt; @Kuloglu:1994uy; @Tuluk:2010ud]. Mevcut yapıların korunması ve yeni yapıların sınırlandırılması amacıyla bölge 1985 yılında 2 Nolu Ortahisar Kentsel Sit Alanı olarak tescillenmiştir.

![Ortahisar'ın yeni kent merkezine göre konumunu gösteren harita [@Var:2015vx].](source/figures/ortahisar.jpg){width=100%}

![Ortahisar uydu fotoğrafı.](source/figures/OrtahisarUyduIzli.jpg){width=100%}

1938 yılında *Jacques H. Lambert* tarafından hazırlanan Trabzonun ilk imar planı Ortahisar bölgesinin mevcut yapıları ile beraber olduğu gibi korunmasını önermiştir. 1968 yılında açılan yarışma ile başlayan ikinci planlama çalışmalarında da kentin eski yerleşkelerinin korunması hedeflenmiştir. Bu çalışmalarda şehrin genişleyebilmesi için Ortahisar'ın güney kısmından teğet geçmesi önerilen Tanjant Yolu 2002 yılında surlar üzerinden ve tarihi kent merkezini ortasından ikiye ayıracak şekilde uygulamaya konulmuştur. Bu değişiklik bölge dokusunda yıkımlara ve büyük tahribata sebep olmuştur.

### Ortahisar Konutlarının Özellikleri

Ortahisar'da bulunan geleneksel konutlar yaklaşık bir asır öncesine dayanan tarihleriyle ağırlıklı olarak Osmanlı dönemine ait yapılardır. Yapım malzemesi ve teknolojisinin imkan verdiği koşullar ile ahşap-kagir yapılar 2-2,5 kat, taş yığma yapılar 3-3,5 kat olarak inşa edilmiştirler. Belli bir geometrik düzeni olmayan parseller içinde olan geleneksel konut dokusu;

* Surlara yakın veya üzerinde, veya bir duvarı ya da terası surların bir parçası olarak
* Kuzey güney aksında bitişerek gelişmiş ve vadilere yönelmiş
* Yoldan yüksek duvarlarla soyutlandırılan bahçe-avlu karışımı bir alandan geçilerek oluşturulmuş konut grubu
* Parsel sınırları içinde yönlere ve kullanışlara göre bir veya iki kenarı parsel sınırına ya da komşu binaya dayanarak geliştirilmiş konut grubu
şeklinde bir araya gelmişlerdir. <!-- Liste paraphrase edilmeli -->

<!-- TODO: BURAYA FOTOĞRAF EKLENMELİ KONUT ÖZELLİKLERİ İLE İLGİLİ-->

Ortahisar konutları plan şeması olarak karnıyarık diye adlandırılan iç sofalı düzenlemeye sahiptirler. Az sayıda da olsa dış sofalı plan şeması örnekleri de bölgede bulunmaktadır. İç sofalı plana sahip evlerde çıkmalı ve çıkmasız olarak örnekleri varken, dış sofalı konutlarda açık ve kapalı olma durumları söz konusudur [@Birlik:1999ux].

![Çıkmalı ve çıkmasız iç sofa örnekleri olarak Nilay Soley ve Resul Özerk evleri [@Ozen:2009wo].](source/figures/SofaliPlanlar.jpg){width=100%}

![Açık ve kapalı dış sofa örnekleri olarak Bekir Gerçek ve Salih Türkmen evleri [@Kuloglu:1994uy].](source/figures/disSofaliPlanlar.jpg){width=100%}

<!--
Zemin katı taşlık, kiler, mutfak gibi yardımcı elemanlardan, esas hayatın geçtiği üst katı da sofa etrafında yer almış odalardan meydana gelen bu eski evlerin Rumlar zamanında yapılmış olanlarının taş, Osmanlılar devrinde yapılmış olanlarının da zemin katı taş ve üst katı ahşap karkas-dolgu sisteminde üretilmiş olduğu, fakat zaman içinde bu duvarların eski özgün karakterini kaybettiklerinden ve derz yüzeyleri büyüdüğünden sonradan sıva ile
kaplandığı görülmektedir. Döşeme ve tavanı ahşap olan bu binaların aynı
zamanda alaturka kiremit kaplı çatılara da sahip olduğu belirtilmesi gereken bir diğer noktadır.

[@Birlik:1999ux]
-->

Geleneksel dokuda ve çevresinde bulunan mimari örnekler yapım dönemine göre bazı özelliklerinde farklılıklar göstermektedir. Ancak Fallmerayer [-@Fallmerayer:2011vq] Ortahisar konutları için Bizans'a bağlı Komnenos Hanedanlığı döneminden itibaren mimari üslup bakımından değişime uğramadığını hatta ölçü ve yönlenme gibi özelliklerinin de değişmediğini belirtmektedir. Yapı stoğu incelendiğinde bölgede Rum dönemi, Osmanlı dönemi, Cumhuriyet sonrası dönem olmak üzere üç döneme ait yapılara rastlanmaktadır. Rum ve Osmanlı dönemi yapıları birbirlerinden yapı malzemesi kullanımında ayrışmaktadır. Rum dönemi yapıların inşaasında yapı malzemesi olarak genellikle taş kullanılırken Osmanlı dönemi yapılarında ağırlıklı olarak ahşap kullanılmıştır. Osmanlı dönemi ve önceki dönemlerin benzer özellikleri;

* Cephe;
	* Yapı cepheleri genel olarak yatayda ve düşeyde simetriktir,
	* Cephede köşe noktalarda düşey, kat aralarında yatay bantlar kullanılmıştır,
	* Cephede açık ve kapalı çıkmalar görülmektedir, bu çıkmalar iç mekanda bulunan oda veya sofa genişliğindedir,
	* Cepheler sokağa paraleldir,
	* Beşik çatı ve ağırlıkla kırma çatı tipi hakimdir,
	* Zemin katlar su basman seviyesinde yükseltilerek bodrum katların aydınlatılması için pencereler kullanılmaktadır,
* Giriş;
	* Genellikle cephenin simetri ekseninde, diğer durumlarda yapının köşesine yakın bulunurlar,
	* Basamaklar ve hemen üzerindeki çıkmalar ile vurgulanmışlardır,
* Pencereler;
	* Dikdörtgen formda ve düşey hatlıdırlar,
	* Sokak cephesinde diğer cephelere göre daha çok pencere bulunmaktadır.

![Geleneksel konut cephesi örnekleri. Solda İsmail Taşkın evi sağda Mustafa Saltoğlu evi [@Ozen:2009wo].](source/figures/KonutCepheleri.jpg){width=100%}

Cumhuriyet sonrası dönem yapıları kargir-yığma ve betonarme olarak inşaa edilmişlerdir [@Kuloglu:1994uy]. Osmanlı dönemi sonrası yapılan bu yapılar hızlı gelişen ekonomik, sosyal, teknolojik ve kültürel değişimlerin sonucu olarak geleneksel dokuya uyum sağlayamamıştır.

## Verilerin Toplanması
<!-- Toplam 73 tescilli yapı var çalışma alanında-->
Ortahisar geleneksek konutlarına ait rölöveler iki arşivden derlenerek oluşturulmuştur. Trabzon Büyükşehir Belediyesi arşivlerinden Trabzon Büyükşehir Belediyesi ve Bimtaş A.Ş. tarafından 2012 yılında Ortahisar'da LIDAR teknolojisi kullanılarak yapılan çalışmadan bölgenin sokak silüetleri elde edilmiştir. Ayrıca Trabzon Rölöve ve Anıtlar Müdürlüğü arşivlerinden elde edilen veriler ile bir araya getirilerek 25 tescilli yapıya ait rölöveler derlenmiştir. Yapıların bir kısmının sokak silüetlerinden ön cepheleri elde edilebilmiş ve geri kalan cephelerinin rölövelerine ulaşılamamıştır. Bir kısmı ise tescilli olmasına rağmen geleneksel dokuyu yansıtmadığından dolayı çalışmaya katılmamıştır. Çalışma 15 adet yapıya ait rölöveler üzerinden elde edilen veriler ile yürütülmüştür.

![Ortahisar bölgesi vaziyet planı. Plan üzerinde sadece tescilli yapılar gösterilmiştir. Arka planı koyu renkli olan yapılar rölövelerine ulaşılabilenleri ifade etmektedir. Ölçek 1/1500.](source/figures/vaziyetplanitescilli.pdf){width=100%}

\newpage