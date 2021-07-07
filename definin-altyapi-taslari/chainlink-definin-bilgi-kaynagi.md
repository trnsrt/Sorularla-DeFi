# Chainlink: DeFi'nin bilgi kaynağı

Bu bölümde, son kullanıcı olarak direkt olarak kullanmadığımız; ancak Merkeziyetsiz Finans için kritik konulardan biri olan Oracle konusuna bakıp, nedir ve neye yarar anlamaya çalışalım:

## Nedir Oracle?

Oracle’in tam Türkçe karşılığı biraz karışık; 'kahin' ya da 'uzman' olarak çevrilebilir. Peki ne işe yarar?

Efendim, Bitcoin ile başlayan merkeziyetsiz dünyanın, Ethereum ile devam eden bir sonraki adımında; karmaşık işlemleri gerçekleştirebilmek için [‘akıllı kontrat’ denen bir yenilik kullanılıyor](https://turansert.com/genel/2018/06/29/bu-kontratlar-cok-akilli-ethereum-ve-akilli-kontratlar.html). Akıllı kontrat dediğimiz, aslında bir kod. Güzelliği ne? Tamamen tarafsız bir şekilde kendisinden ne istenirse onu istendiği zaman yapıyor. Böylece, kontrata taraf olanlar, eğer belirlenen koşullar gerçekleşirse, kontratın yerine getirileceğinden emin oluyorlar.

Çok güzel ancak ufak bir sorun var: Kontratın, kendisini harekete geçirecek bu koşulların oluştuğunu bilmesi gerek. Bunu belirleyen bilgilerin büyük çoğunluğu ise blokzincirin içinde değil, dış dünyadan geliyor. Biri bu bilgiyi kontrata verecek ya da kontrat bu bilgiyi bir kaynaktan alacak.

![](../.gitbook/assets/030305-chainlink-definin-bilgi-kaynagi-labrador-5741850_1280.jpg)

_Biri bilgiyi kapıp gelsin - bunun gibi 😁 Kaynak: Image by_ [_Jana Schmidt_](https://pixabay.com/users/jawika-19109282/) _from_ [_Pixabay_](https://pixabay.com/)

Örneğin; 2020 yılı ABD seçimleri sonucunda kimin seçileceği ile ilgili yapılan tahminlerde, kaynak olarak [Amerikan hükümetinin resmi web sitesinde yeni başkan olarak kimin yazıldığı](https://www.usa.gov/presidents#item-37462) kullanılıyor. İşte akıllı kontratın sonucu bu siteden alarak çalışması ve doğru tahmin edenleri belirlemesi gerekiyor. Peki, akıllı kontrat bunu nasıl alacak?

Bu, en basit ve bariz örnek. İki yıl önce yayınlanan [“Tahmin piyasaları için Blockchain” yazımızda](https://turansert.com/genel/2018/07/13/gelecegi-tahmin-için-blockchain.html), bu kaynakların blokzincir dünyası dışında, tarafsız olduğu kabul edilen bilgi sağlayıcılardan \(örneğin WSJ gazetesi\) alınıp, blokzincire otomatik ya da uzmanlar tarafından manuel olarak girilmesinden bahsetmiştik.

ABD seçimi gibi tek bir olaya bağlı tahminlerde işe yarayabilecek olan manuel bilgi aktarımı, merkeziyetsiz dünyada çok da çalışmayacak gibi görünüyor. Gelin bakalım ne gerekiyor DeFi dünyasına:

### Merkeziyetsiz dünya için neden önemli?

Merkeziyetsiz finans dünyasının oyuncusu olan değişik platformlar, aynı bir legonun parçaları gibi birbirine iç içe geçmiş bir şekilde çalışıyorlar. Yukarıdaki basit örneğin ötesinde, bu lego parçalarının birbirleriyle uyumlu şekilde hareket edebilmeleri için onlarca hatta yüzlerce bilginin akıllı kontratlara akması gerekiyor. Bunu sağlayabilmek için kaynaklardan alınan bilginin hem doğru ve tarafsız hem de çok hızlı bir şekilde toplanması gerekiyor.

Bir örnek verelim. Sentetik türev piyasaları, basitçe herhangi bir ürünün \(örneğin, altın ya da petrol\) aslına sahip olmadan, o ürünün kazancına ya da kaybına ortak olma ve alım-satımını yapmaya imkan veren pazarlar idi \[^1\]. Merkeziyetsiz sentetik türev borsasında ürünün kendisi değil taklidi alındığı ya da satıldığı için, dış dünyadaki orijinal fiyatların buraya aktarılması gerek, hem de çok sık bir şekilde.

İşte oracle dediğimiz uzmanlar, akıllı kontratların ihtiyacı olan bu bilgiyi onlara sağlayan yapılar. Dolayısıyla, her ne kadar direkt temasa etmeseler de kullanıcılar için çok kritik bir altyapı hizmetini yerine getiriyorlar.

### Merkezi kaynak mı istersiniz yoksa merkeziyetsiz mi?

Yukarıda merkeziyetsiz bir oracle örneği verdik ancak hemen belirtmek lazım; bu alanda en büyüklerden bir tanesi ABD’nin en büyük merkezi kripto borsası olan Coinbase tarafından sunulan merkezi bir oracle. [Coinbase Price Oracle](https://blog.coinbase.com/introducing-the-coinbase-price-oracle-6d1ee22c7068) sayesinde, piyasada işlem gören tokenlerin fiyat bilgilerini sürekli bir biçimde elde etmek mümkün.

Merkezi yapılar, DeFi dünyasında genelde hoş karşılanmazlar. Bunun temel nedeni, hep bahsettiğimiz dijital dünyada merkezi yapıların güvenlik açığı yaratma algısı. Zira, tek kaynak olmaları nedeniyle bu yapılara yapılacak saldırılar fiyatların manipüle edilmesine yol açabilir. Bu da, o fiyatları kullanarak hizmet veren platformları zor durumda bırakabilir.

### Merkeziyetsiz platformlar nasıl yapıyorlar bu işi?

Bilgiyi zincir dışından içine taşımak o kadar da basit bir olay değil. Fazla tekniğe girmeden anlatmaya çalışalım \(son kullanıcı olarak ilginizi çekmiyorsa hemen bir sonraki bölüme atlayabilirsiniz 😉\):

Oracle sistemlerinde de dış dünya ile ilişkiyi ağ üyesi makineler kuruyor. Bilgi ihtiyacı olan DeFi yapıları, bir akıllı kontrat aracılığıyla hangi tür teknik bilgiyi istediklerini oracle hizmeti veren ağın içine koyuyorlar. Teknik derken kasıt; hangi bilgi kaynağının kullanılacağından, ne sıklıkla ve hangi hizmet süreleri \(örneğin, %99.99 çalışma gerekliliği\) gibi istekler.

Ağ içindeki üyeler bu tip bir talebi içeren bir akıllı kontrat gördüklerinde, bu hizmeti ne kadar bir ücret karşılığı yerine getirebileceklerini kontrata bildiriyorlar. Bu ücret, genel olarak o ağın kullandığı kriptopara cinsinden belirleniyor.

Anlaşma sağlanıp sistem çalışmaya başladığında, bilgi sağlayıcı üyeler dış dünyadaki kaynaklardan aldıkları bilgileri akıllı kontrata aktarıyor. Diğer üyeler de ağ üzerinden bu bilginin doğruluğunu teyit ediyor.

Sonrasında akıllı kontrat, farklı üyelerden gelen teyid edilmiş bilgilerin ağırlıklı ortalamasını alıp bir değer buluyor ve talep sahibine bildiriyor. Böylece, bir kişiye bağlı kalmadan, istendiği kadar farklı kaynak kullanılarak olabildiğince tarafsız bilgi sağlanmış oluyor. \[^2\]

#### Son zamanlarda önemi arttı mı?

DeFi dünyasının patlamasıyla birlikte doğru ve hızlı veriye olan ihtiyaç da arttı ve bu alandaki servis sağlayıcılar ciddi talep görmeye başladı. Öyle ki, bu alandaki en büyük iki oyuncu olan [Chainlink](https://chain.link/) ve [Nest](https://nestdapp.io/), Eylül 2020’de Ethereum ağını en çok meşgul eden 5. ve 7. uygulamalar arasına girip bir ayda toplam [2.5 milyon ABD Doları işlem ücreti ödediler\(pdf\)](https://static.coindesk.com/wp-content/uploads/2020/10/Huobi-DeFiLabs-Price-Oracle-A-Must-Have-Infrastructure-Oct-8-2020.pdf).

Bu alandaki belli başlı oyuncular; [Chainlink](https://chain.link/), [Band Protocol](https://bandprotocol.com/), [Nest Protocol](https://nestdapp.io/), [DIA](https://diadata.org/), [Tellor](https://www.tellor.io/), [Zap](https://zap.org/) ve [DOS Network](https://dos.network/) olarak sıralanıyor. Hemen belirtelim; Chainlink bu piyasanın neredeyse tek hakimi.

### Sıkıntıları neler?

Merkeziyetsiz Finans dünyasında oracle sistemlerinin en büyük sıkıntısı gecikmeler. Yukarıda bilgi aktarımda bahsetmiştik. Bilgi toplanıyor, blokzincir ağına aktarılıyor, orada teyit ediliyor ve talep edene gönderiliyor. Dijital dünyada aslında saniyeler içinde yapılabilecek bir işlem, ancak burada bilginin teyidi sonrası blokzincire yazılıyor olması nedeniyle, blok oluşturma hızları darboğaz yaratıyor. Örneğin, Ethereum sisteminde her bir blok 10-20 saniye arasında oluşuyor. Bu da bilginin ulaşımında gecikmeler olması demek.

Bunun yanında, bilgiyi tek bir kaynaktan almak da sıkıntı yaratabiliyor. Örneğin, kimi platformların akıllı kontratları, ihtiyaç duydukları token fiyat bilgisini tek bir borsadan çekebiliyorlar. Bazı akıllılar ise, özellikle likiditenin azaldığı durumlarda, bu borsadaki token fiyatını manipüle edip, bu bilgiyi kullanan platformlarda anlık işlemler ile ciddi kazançlar elde edebiliyorlar. Bunu önlemenin yolu, akıllı kontratları iyi dizayn etmek ve bilginin birkaç farklı yerden gelmesini sağlayarak manipülasyonu zorlaştırmak.

Şimdi de Chainlink örneğini daha yakından inceleyerek, farklı ürünler neler olabilir ve bu alan daha nerelere ulaşabilir ona bakalım:

### Nedir bu Chainlink?

En basit şekliyle açıklamak istersek, Chainlink, her tür blokzincir ve DeFi platformuna hizmet veren bir ara yapı. Yaptığı; bu platformların kullandığı akıllı kontratların ihtiyaç duyduğu blokzincir dışı bilgileri bulup kontrata aktarmak.

Normalde akıllı kontratlar blokzincir içinde bulunan bilgiyi çok rahat bir şekilde okuyup işleyebiliyor. Sıkıntı, blokzincir dışı bilgilerde. Bu bilgilerin; birileri tarafından alınıp, işlenip, akıllı kontratın anlayabileceği bir şekilde blokzincir içine, oradan da kontrata aktarılması gerekiyor.

Chainlink işte bu hizmeti veren aracılar içinde en büyüğü. Bir DeFi platformu olarak bilgi ihtiyacınız var ise, bulunduğunuz blokzincir üzerinden bir akıllı kontrat ile Chainlink’e talepte bulunuyorsunuz. Sistem üyeleri \(node/düğüm\) bu hizmete talip oluyorlar. Chainlink, bu üyelerden birkaçını hizmeti vermek için seçiyor. Sonrasında, seçilen üyelerin dış dünyadan topladığı bilgiler, Chainlink tarafından bulunduğunuz blokzincir üzerinden size aktarılıyor. Birçok kaynaktan birkaçının seçilmesi ve bilgilerin toplanarak sunulması, tek bir kaynaktan bilgi alımının doğurabileceği yanlış ya da çarpıtılmış bilgi ihtimalini en aza indirmeye yarıyor.

![](../.gitbook/assets/030309-chainlink-definin-bilgi-kaynagi-chain-1995543_1280.jpg)

_Image by_ [_kalhh_](https://pixabay.com/users/kalhh-86169/) _from_ [_Pixabay_](https://pixabay.com/)\_\_

#### Chainlink’in hikayesi

Hikaye aslında oldukça eskilere \(blokzincir zamanından bahsediyoruz!\), 2014 yılına dayanıyor. Smartcontract.com \(şimdiki adıyla [Chainlink Labs](https://chainlinklabs.com/)\), açık blokzincirler ile dış dünya verileri arasında köprü kurmak amacıyla kurulan bir şirket. Merkezi, Cayman adalarında.

Bu işin nasıl becerilebileceği konusuna uzunca bir süre kafa yoran ve deneysel çalışmalar yapan şirket yönetimi, 2017 yılında yaşanan halka token satma \(İngilizce'de Initial Coin Offering - ICO\) rüzgarından yararlanarak geliştirdiği Chainlink projesine özgü bir token yaratıyor. LINK adı verilen bu tokenin %35’lik kısmı bu ICO ile halka satılarak 32 milyon ABD Doları toplanıyor. Tokenlerin %35’lik kısmı Chainlink sistemine üye bilgi toplayıcılar ve sistemin gelişimine katkı sağlayacak paydaşlara verilmek üzere bir kenara ayrılıyor. Kalan %30 oranındaki token ise kurucu Chainlink Labs’de kalıyor.

ICO sonrasında da devam eden ürün ve platform geliştirme sürecinin devamında, Chainlink nihayet 2019 yılı Mayıs ayında kullanıcılara sunuluyor.

Her ne kadar hizmet verdiği sektör ağırlıklı olarak Merkeziyetsiz Finans olsa da Chainlink için merkeziyetsiz bir platform demek doğru değil. Chainlik ağı üyeleri dağıtık bir şekilde görev yapıyor ama diğer alanlarda sıkı bir merkezilik söz konusu. Örneğin, LINK tokenlerinin herhangi bir yönetim hakkı yok. Zaten, bu tokenlerin ciddi bir kısmı halen Chainlink Labs kasasında. Ağın yönetimi de elbette Chainlink ekibinin elinde.

### Chainlink tokeni LINK

Chainlink tarafından yapılan ICO ile hayata geçirilen LINK esasında iki ana işe yaramakta:

Birincisi, bilgiye ihtiyacınız var ve bunu Chainlink’ten sağlamak istiyorsanız, bu bilgiyi sağlayan Chainlink ağının üyelerine hizmetleri karşılığı ödemeyi LINK ile yapıyorsunuz.

İkincisi ise, Chainlink ağı üyesi iseniz ve hizmet vermek istiyorsanız, elinizdeki LINK tokenları rehin etmeniz gerekiyor. Üstelik ne kadar çok rehin ederseniz, Chainlink ağını yönetenlerin size hizmet verme ihtimali o kadar yükseliyor. \(Hemen belirtelim rehin verme - staking - henüz başlamadı\).

#### LINK ile ilgili eleştiriler

LINK ile ilgili birkaç eleştiri var. Dilerseniz, gelin onlara kısaca göz atalım:

_**LINK tutmak gerekli mi?**_

Kripto alanının önemli araştırma şirketlerinden [Messari](https://messari.io/)‘den [Ryan Selkis](https://twitter.com/twobitidiot)‘in şu eleştirileri önemli:

_“LINK bir ödeme tokeni olduğu için, Chainlink üyelerine ödeme yapmak dışında elde tutmak ve ona bir değer yüklemek anlamsız. Ödemeler için Chainlink kullanıyorsanız, elde daha likit başka tokenleri tutup, ihtiyacınız olduğunda bu daha az likit ve kullanışsız LINK tokenine dönebilirsiniz._

_Konu Chainlink güvenliğini sağlamak için LINK rehin etmek ise, mevcut ücret modeli ne stabil ne de ölçeklenebilir. İşlem başına ücretleme şeklinde bir öneri var; ancak böyle bir uygulama Chainlink hizmetlerini kullanılamayacak kadar pahalı bir hale getirir.”\[^1\]_

_**Chainlink XRP ile aynı akıbeti paylaşır mı?**_

İçinde bulunduğumuz ay içinde, gündemi takip ettiyseniz XRP tokenin başına gelenleri okumuşsunuzdur. Kaçıranlar için hatırlatalım:

XRP, Ripple adlı bir teknoloji şirketi tarafından 2013 yılında yaratılmış bir token. Aslında Ripple’in başı, ABD’nin sermaye piyasası denetleyici kurumu SEC ile uzun zamandır dertte idi ama geçtiğimiz günlerde SEC, Ripple yönetimine [ciddi suçlamalarda bulundu](https://www.sec.gov/news/press-release/2020-338). Özetle, Ripple’in XRP için ICO yaparak aslında izinsiz bir halka arz yaptığını belirterek iki üst düzey Ripple yöneticisine dava açtı.

Şu aralar SEC’in Chainlink \(daha doğrusu kurucusu Chainlink Labs\) için de benzer şekilde suçlamalar getirebileceği konuşuluyor. Zira, Chainlink Labs da 2017 yılında aynı Ripple benzeri bir ICO yaptı ve halen LINK’in %35’ine sahip. Son günlerde bu [dedikoduların arttığını](https://twitter.com/bit_gossip/status/1343214669201371138) da söyleyelim.

_**Chainlink fazla PR mı kullanıyor?**_

Öte yandan, kripto dünyasında hem Chainlink hem de Ripple için getirilen ortak bir eleştiri var ki; o da her iki yapının kullandığı yoğun reklam, pazarlama ve halkla ilişkiler kampanyaları.

Ripple, XRP kullanımı ile ilgili hangi banka ile “test sürümü” deney yapsa, bunu o banka ile partner/ortak olduğu şeklinde yoğun bir PR bombardımanı ile piyasaya sunardı.

Chainlink de aynı şekilde, hangi platform ile hizmet sağlayıcı olarak anlaşsa, bunu çok yoğun bir PR faaliyeti ile sunuyor. Ayrıca hem XRP hem de LINK’in, bu tokenlere ‘gönülden bağlı’ sosyal medya takipçi orduları var.

Bu benzerliklerden dolayı Chainlink, Ripple’a; tokeni LINK XRP’ye benzer mi? Gayet tabii hayır ancak böyle yoğun PR faaliyetleri, bu platformların merkeziyetsiz olmaktan çok, arkada ipleri elinde tutan firmalar bulunduğu ve bu yapıların aslında merkezi bir platform gibi değerlendirilmesi gerektiği algısını güçlendiriyor.

_**LINK fazla mı değerli?**_

Değer konusu oldukça subjektif. Bu yazımızın ana konusu da değil ancak Ryan Selkis’in bir başka eleştirisini de dikkate almakta fayda var:

Şu an için LINK tokenin toplam değerinin, tüm DeFi’nin üzerine kurulu olduğu ETH sisteminin değerinin yaklaşık %6’sı olduğunu görüyoruz. LINK tokenin toplam değeri yaklaşık 5 milyar ABD Doları seviyesinde. Görevi ekosisteme bilgi sağlamak olan bir hizmetin tek bir oyuncusunun değeri bu kadar eder mi?Değerlendirmesi siz sevgili okuyucunun.

_**Chainlink kötü niyetli mi?**_

Chainlink için [Zeus Capital](https://zeus-capital.com/) isimli bir yatırım fonunun 2020 Temmuz’unda yayınladığı bir rapor \([pdf](https://zeus-capital.com/assets/The_Chainlink_Fraud_Exposed.pdf)\) oldukça ilgi çekti.

Hemen baştan belirtelim, rapora göz attığınızda ve Zeus Capital’in [websitesini](https://zeus-capital.com/) incelediğinizde, yazılanların bir çoğunun ve Zeus Capital’in kendisinin de şaibeli olabileceği izlenimine kapılıyorsunuz. O nedenle bu kısımda yazılanları büyük bir soru işareti ile değerlendirmekte fayda var:

Temel olarak bahsedilen; Chainlink’in hizmet sağlayıcı seçiminin şeffaf olmadığı, mevcut hizmet sağlayıcıların ağırlıklı olarak Chainlink ile ilişkili kişiler olduğu ve sistemin, ağ üyelerinden müşterilere hizmet verecek olanları seçerken bu kişileri kayırdığı şeklinde.

İddialardan bir başkası da, bir DeFi platformu olan [bZx](https://bzx.network/)‘in 2020 başında [yaşadıği iki hack olayının](https://cointelegraph.com/news/decentralized-lending-protocol-bzx-hacked-twice-in-a-matter-of-days) arkasında Chainlink olduğu yönünde. Hack olayının ana nedeninin bZx’nin tek bir bilgi kaynağı ile çalışması gösterilmişti. Olayın duyulması ile birlikte, LINK tokenin fiyatı ciddi bir şekilde arttı. Daha sonrasında da bZx, [Chainlink ile çalışmaya başladı](https://coingape.com/bzx-hack-update-exchange-add-chainlink-protocol/).

Zeus Capital’in bu yazısına karşı olarak büyük ihtimal ile Chainlink kaynaklı yayınlanan [bir başka Medium yazısı](https://smartcontentpublication.medium.com/debunking-the-zeus-capital-disinformation-report-on-chainlink-7313d9e1801#e581) olayın bir PR tiyatrosuna dönmüş olduğu izlenimini uyandırıyor.

Son zamanlarda çıkan “Link, XRP gibi mi olacak?” söylentilerinin arkasında da Zeus Capital’in attığı bir [tweet](https://twitter.com/ZeusCapitalLLP/status/1341759410884857856?s=20) olduğunu söylersek sanırım şaşırmazsınız.

Dolayısıyla, yukarıdaki Zeus Capital iddialarını, 'çamur at izi kalsın' olarak mı, yoksa 'ateş olmayan yerden duman çıkmaz' şeklinde mi değerlendirmeli, karar siz okuyucuya kalmış durumda.

### Chainlink ve tokeni LINK üzerine son birkaç söz

Hep bahsettiğimiz emekleme aşamasındaki Merkeziyetsiz Finans dünyasının, ayağa kalkıp yürümesi için gerekli yapı taşlarından biri de oracle servis sağlayıcılar olacak. Şu an için tek bir oyuncunun ağırlığında olması ve merkezi servis sağlayıcıların potansiyel risk barındırması nedeniyle, bu alan aynı hizmet verdiği DeFi platformları gibi henüz olgunlaşmış sayılmaz. Bu alandaki ihtiyacı düşünürsek, önümüzdeki dönemde teknik olarak farklı ürünlerin çıkması ve bu alanın oyuncularının hacim olarak büyümesi kaçınılmaz görünüyor. 

Chainlink, merkeziyetsiz finans platformlarının kritik ihtiyaçları içinde sayabileceğimiz ‘dış dünyadan bilgi sağlama’ görevini yerine getiren oracle servis sağlayıcıların lideri. Kurucusu, şu ana kadar daha çok geleneksel bir şirket gibi hareket etti. Bu hareketler, LINK token denen sistem parasına son birkaç yılda ciddi bir değer kazandırdı. Uzun vadede bu tip geleneksel hareketler gerek kanuni otoriteler gerekse merkeziyetsizlik felsefesi ile yetişen yeni DeFi girişimlerinin eleştiri ve tepkisine yol açabilir.

Her konuda olduğu gibi bu alanda da sağlıklı bir rekabetin olması ekosistemin gelişmesi için önemli. Önümüzdeki dönemde bu alanın nasıl gelişeceğini, rakiplerin pastadan daha büyük pay kapmak, Chainlink’in ise mevcut payını kaptırmamak için yapacağı hamleler konuşulmaya devam edecek.

\[^1\] messari-report-crypto-theses-for-2021.pdf Sayfa 67

