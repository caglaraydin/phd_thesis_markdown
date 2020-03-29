# SONUÇLAR VE ÖNERİLER

\thispagestyle{empty}

Çalışmanın amacı geleneksel Ortahisar konutlarının CGA gramerinin kodlanması ve parametrik olarak üretilmesidir. Çalışmada sunulan parametrik biçim grameri geleneksel Ortahisar konutlarının ontoloji çalışmasının sonucudur ve konut tipinin analizinin yanında sentezi içinde bir tasarım aracı olarak kullanılabilmektedir. Üretilen gramer geleneksel Ortahisar konutlarının kütle ve cephe karakteri ilişkilerini ve oluşumlarını kural şemaları ile açıklamaktadır. Yapılan ontoloji çalışması taban alanının genişlik-derinlik ilişkisini, kat sayısı ve katlar arası yükseklik ilişkileri, cephe tipi, kapalı ve açık çıkmalar, yatay ve düşey bantlar, pencere ve kapılar ve çatı gibi öğeleri barındırmakta ve birbirleriye olan kompozisyonu ele almaktadır. Geleneksel Ortahisar konutları üzerine yapılan bu ontoloji çalışmasında;

- cephe elemanları ve kat yükseklikleri karşılaştırıldığında aralarında bir korelasyon bulunmadığı,
- taban alanının derinliğinin genişliğine oranı 0,346 ile 1,513 arasında bulunduğu,
- taban alanı büyüklüğünün cephe karakterini etkilediği ve 100m^2^ üzerinde taban alanı bulunan yapıların üç parçalı cepheye sahip olduğu,
- zemin ve birinci kat bütün yapılarda bulunup geleneksel Ortahisar konutları için çekirdek birimi oluşturduğu,
- çatı katı sadece üç parçalı cepheye sahip yapılarda bulunduğu ve kapalı çıkmaya göre biçimlendiği,
- kapalı çıkmaların sokak yönünde açık çıkmaların ise arka cephede bulunduğu, açık çıkmaların sadece kapalı çıkmaya ve çatı katına sahip yapılarda bulunduğu,
- açık çıkmaların derinliğinin kapalı çıkmaların derinliğine oranının %60 olduğu,
- çatı katının cephedeki genişliğinin bir alt katın cephesinin orta parçasının genişliğine eşit olduğu gözlemlenmiştir.

Üretilen gramer diğer biçim gramerleri gibi tasarım bilgisini biçim kuralları ile ifade etmektedir. Bir biçim organizasyonunun bir başkasından nasıl türetileceğini açıklamaktadır ve geleneksel Ortahisar konutlarının kütlesel tasarım sürecini izah etmektedir. 

\newpage

Tasarım elemanlarının ve onların bir araya geliş kurgularının semantik ve biçimsel bilgileri bir set grameri olan CGA grameri ile CityEngine yazılımı üzerinde parametrik olarak tanımlanmıştır. Bu parametreler yazılım içinde bir panelde düzenlenerek, kısıtların interaktif olarak tercihler çerçevesinde değiştirilebilmesine olanak verilmiştir (Şekil \ref{CGAPanel}). Tasarım sürecinde kısıtlar üzerinde yapılacak değişikliklerle kütle ve cephe nitelikleri ile ilgili görsel ve sayısal geri bildirimler sayesinde farklı fikirler arasında geçiş ve yorumlamaya olanak sağlanmaktadır. Böylece tasarım düşünme sürecinde tasarımcının görsel ve emsal tabanlı muhakeme süreçleri üretilen taslak modeller ve sayısal veriler sayesinde desteklenmektedir.

Sunulan yöntemde tasarımcının karar verme süreci gerçek zamanlı veri toplama ve üç boyutlu taslak modeller ile desteklenmektedir. Tercihler çerçevesinde üretilen taslak modeller tasarımcı tarafından kullanılan bir bilgisayar destekli tasarım programı veya üç boyutlu modelleme yazılımına uygun dosya formatı ile aktarılabilmektedir. İstenilen yazılıma aktarılan taslak modeller tasarım altlığı olarak ele alınıp tasarımcı tarafından geliştirilebilir. Bir önceki bölümde gösterilen örnek model çalışmaları da CityEngine yazılımından 3ds Max yazılımına FBX dosya formatı kullanılarak aktarılmıştır (Şekil \ref{Yenimodel}). Taslak modelden elde edilen sayısal veriler tasarımcı tarafından geleneksel çalışma yönteminde kullanılmak üzere de ele alınabilir.

Önerilen bu tasarımı destekleyici yöntem tasarımcılar açısından kullanımı kolaydır ve etkileşim kurmak için temel bilgisayar bilgisi yeterlidir. Tasarımcıya alternatif üretme ve değerlendirme kolaylığı sunmaktadır. Tasarım süreci için hem görsel hem de sayısal veriler sunmaktadır. Ayrıca bilgisayarlı ve geleneksel tasarım yöntemlerinin ikisinde de sürece katılabilmektedir. 

Önerilen yöntemde kullanılan CityEngine yazılımı bazı durumlarda kısıtlayıcı olmaktadır. İlk olarak model üretimi hususunda melez çatı formları yazılımın güncel hali ile olanaklı değildir. Biçim gramerleri ile açıklanan kurallar yazılımın bazı teknik kısıtlarından dolayı CGA biçim grameri içinde farklı kodlanarak aynı sonuçlara ulaşılmıştır. Bir diğer yandan yazılımın ticari lisanslı oluşu ulaşılabilecek tasarımcı kitlesini sınırlı kılmaktadır. 

Bu çalışma yöntemi tasarım altlıkları üretmesini ek olarak dört ayrı yönde geliştirilebilir. Bunlardan birincisi geleneksel Ortahisar konutlarının tasarım diline ait kompozisyonsal yönleri hakkında mimarlık eğitiminde bir araç olarak kullanılabilir. İkinci olarak Ortahisar bölgesinin geleneksel dokusunu korumak amacıyla bu bölgede yapılacak yeni yapılar için görsel ve sayısal veriler doğrultusunda bir denetim aracı olarak kullanılabilir. Birden çok modeli aynı anda üretebilme özelliği ile beraber kentsel dönüşüm süreçlerinde kullanılabilir. Bunlara ek olarak Geleneksel Ortahisar konutlarının tahrip olmadan önceki haline dair muhtemel karakteristik özelliklerini üretebilmek için kullanılabilir.

CGA grameri içindeki kurallar üç boyutlu kütle ve cephe karakteristiklerini tanımlamaktadır. Ontoloji çalışmasına katılan örneklem kümesinin genişletilmesi ve örneklerin plan şemalarının çalışmaya dahil edilmesi daha fazla bilgi ve kural tanımlamayı olanaklı kılacaktır. Örneklerin plan şeması analizleriyle iç mekanların kullanım amacına, mekanların birbirleriyle olan orantılarına, aydınlanma ve sirkülasyon gibi özelliklerine ait bilgiler de gramer içine dahil edilebilir.

<!-- Nasıl, hangi süreçler sonucunda, kim tarafından, yönetmeliklerden mi alınır. Hangi süreçler yapılırsa sağlıklı olur. Sen ontolojiyi yaparken ne süreçte bıraktın. Bu detaylı bilgiler nereden alınır. -->

CGA grameri aynı anda bir çok model üretimine olanak sağladığından dolayı mahalle veya kentsel dönüşüm ölçekleri için alternatif üretmesi açısından kullanılabilir. Ancak bu çalışmada sokak dokusu ve komşuluk ilişkileri ele alınamamıştır. Bölgenin bu anlamda çalışılıp analizinin yapılması ile gramer içerisine yapıların birbirleriyle olan konumlanma, yönlenme vb. ilişkileri entegre edilebilir. Ayrıca güncel yönetmelikler ve standartların kısıtları gramer içinde tanımlanması durumunda imara uygun modellerin üretimi sağlanacaktır. Birim inşaat maliyetleri sisteme entegre edilerek bu ölçekte yapılacak çalışmalar için tahmini maliyetlerde karar sürecinde yardımcı olacaktır.

<!-- In order to maintain and support such processes, in addition to the geometric formation of housing units, cost estimation and valuation of the existing housing units can be integrated into the model. Cost estimations can be essential to calculate the budget, funds, and approximate timetable, not only for inhabitants but also for governments. More detailed feasibility studies can be generated by adding construction cost and funding opportunities as a parameter to eventually enhance the bottom-up urban planning and design processes.  -->

Ontoloji çalışması kütle ve cephe özellikleri ile sınırlı kalmıştır. Bu çalışma üzerine yukarıda bahsedilen önerilere ek olarak yapılardaki malzeme kullanımı, birleşme detayları, bahçe kullanımı vb. özellikleri de analiz edilip kuralları oluşturularak tahrip olmuş geleneksel Ortahisar konutlarının tahrip olmadan önceki haline dair muhtemel karakteristik özelliklerini üretebilmek mümkün olacaktır.

<!-- Tahrip olmadan korunacak başka özellikler neler olabilir, daha detaylı çalışılacak olsa. Ahşap ustası gelip çalışmış olsa onunda grameri yapılana bütünleşebilse vb. tartışılsa. Ne işe yarar bu doktora diye anlatsan. -->

<!--
+ Nasıl altlık olarak kullanılacak?

Bu alana ne kattın
Bu araçtan ne öğrendin, bu araç nelerde kullanılıyor
Bu çalışma yöntemi kullanıldığı takdirde hangi alanlarda geliştirilebilir. 
Bu alanda kullanılırsa nasıl geliştirilebilir
Geleceğe dair bir takım spekülatif öneriler yapmak gerekiyor.
Yapılı çevrede kontrol mekanizması olarak kullanılabilir

+ Ontoloji çalışması olduğu vurgulanmalı. Girişte ve literatürde belirtilmeli. Sonuçlarda ontoloji çalışması tartışılmalı.
Herkes kim, nasıl süreçler söz konusu, alternatif üret tuşu hangi senaryolarda karşımıza çıkar. Açık olmalı
+ CityEngine kısıtlarından bahsedilmeli. Lisanslı olması, Türkiyede satıcısı bulunmuyor herhalde.

+ Altlıklar modern tasarımlara olanak veriyor mu, tasarımcıyı kısıtlıyor mu?
Mevcut yazılımlar ile nasıl çalışacak.



Page 116
the ability to generate many versions of the model underscored that it was to be viewed and treated as a research tool and not as an instance of 'scientific truth'. The goal of the model was to give spatial presence to a range of possibilities, much as I argue the interaction of ritual and landscape must have taken shape within a range of configurations and not as a pre-designed, static diagram. Procedural modeling provided a framework for the incorporation of alternatives and the reasoning behind them. [@Saldana:2015wj]

Page 8
In the present case, the grammar generates a portfolio of simple house designs that follow the typological and cultural continuity of the vernacular architecture of Sarajevo. Here, the grammar serves as a creative design instrument. It does not generate the designs but rather reinterprets them in contemporary terms. Each design in the portfolio can further be transformed according to functional, structural, and aesthetic properties.The grammar-based design method provides an apparatus for the continuing transformation of an existing type leading to the generation of a new type. [@Colakoglu:2005kc]

Geleneksel Trabzon Ortahisar konutları

- Çalışmanın amacı
  - Önerilen çalışma yordamsal modelleme yöntemi kullanılarak geleneksel Trabzon konutlarının CGA gramerinin kodlanmasını ve parametrik olarak üretilmesini amaçlamaktadır.
- Çalışmanın anlamı
- sonunda ne elde edildiği
- kimin bundan faydalanacağı, kime referans-kaynak olacak, kimin işine yarar. Kimler kullanabilir, nasıl bir beceri seti gerektirir.
- Belediyeler de kullanılabilir
- Eğitim amaçlı kullanılabilir

Alternatif üretmek yerine bilgilerin değerlendirilmesi daha önemli.

- Database kurup değerler girilip iyileştirme yapılabilir.
- Planlar bu model sistemine eklenebilir.
- Mahalle-kentsel dönüşüm ölçeği için kullanılabilir. Bunun için yapıların birbiriyle olan ilişkileri (konumlanma, yönlenme, vb.) analiz edilip sisteme entegre edilmeli.
- Dokular ve ince detaylar içerisine eklenerek edilerek VR sistemler ile beraber tanıtımları yapılabilir.
- Kent kütüphanesinde veri-bilgi kümesi olarak üç boyutlu gösterimler ile sunulabilir.
- İnternet ortamında yapay alanlar oluşturulup genel karakter hakkında bilgi verilebilir.
- Geliştirilecek CGA kodu ile beraber tahrip olmuş geleneksel Ortahisar konutlarının tahrip olmadan önceki haline dair muhtemel karakteristik özellikleri üretilebilmek. PENCERE SÖVELERİNİN EKLENMESİ LAZIM

-->
