# MakerDAO: Kişiye özel merkez bankası

Önceki bölümde finans dünyasında yeni başlayan DeFi hareketine değinmiş ve para transferi ile başlayan aracılık hizmetlerinin makinelere aktarılması işinin daha başka hangi alanlara yayılabileceğine değinmiştik. İşte karşınızda bu alanlardan ilki olan kredili işlemlerin en yaygın kullanılanı MakerDAO..

## MakerDAO nedir? <a id="makerdao-nedir"></a>

### TL; DR:

MakerDAO kullanıcıların kendi başlarına kredi yaratabilecekleri bir platform. Kullanıcılar sahip oldukları kripto paraları teminat olarak veriyorlar ve karşılığında sistemin sabit parası olan DAI’yi yaratıyorlar. Sonra bu DAI’yi borsalarda bir ABD Doları karşılığı satıp o parayı istedikleri gibi kullanıyorlar. Yarattıkları \(yani borç aldıkları\) bu DAI’yi belli bir faiz ödeyerek istedikleri süre tutuyorlar - yeter ki teminatları borçlarını karşılasın. Sonrasında istedikleri zaman borsadan DAI satın alıp bu DAI’yi yakarak borçlarını kapatıyor ve başlangıçta koydukları teminatlarını geri alabiliyorlar. Sistemin işleyişi için gerekli önemli kararlar \(örneğin faiz oranları gibi\) yine bir merkezden ziyade kullanıcılar tarafından oylama yöntemi ile alınıyor.

### Nasıl çalışıyor? <a id="nas&#x131;l-&#xE7;al&#x131;&#x15F;&#x131;yor"></a>

~~Elinizdeki KriptoPara’yı \(şu an için yalnız Ethereum parası ETH geçerli\) teminat olarak gösteriyorsunuz, buradaki deyişiyle ETH’lerinizi sistem içine kilitliyorsunuz.~~ Gönderdiğiniz her 150 birim para için 100 birime kadar Dai yaratabiliyorsunuz. Sonrasında bu DAI’yi istediğiniz noktada borsada bire bire yakın bir değerden ABD Doları’na çeviriyor ve kullanıyorsunuz. Bu para için bir maliyet ödüyorsunuz, sonrasında ise dilediğiniz noktada tekrar Dai satın alarak yok ediyor ve ETH’nize geri kavuşuyorsunuz.

### Neden insanlar kullanıyor? <a id="neden-insanlar-kullan&#x131;yor"></a>

Diyelim ani olarak paraya ihtiyacınız var, mevcut paranızı da ETH’ye yatırdınız. ETH’nin yükseleceğini düşünüyorsunuz ya da başka herhangi bir nedenle ETH’lerinizden ayrılmak istemiyorsunuz. Bu sistemi kullanarak hem nakit ihtiyacınızı karşılayabilir hem de ETH’nin getireceği kardan yararlanabilirsiniz.

### Kredi maliyeti ne? <a id="kredi-maliyeti-ne"></a>

Şu anda inanılmaz ucuz. Yıllık 0.5% bir faiz maliyeti var \(buna stabilize ücreti deniyor ve bu ücreti ayrı bir para ile ödüyorsunuz ama şu aşamada çok da gerekli değil bunu bilmek - en altta notta teknik detayı var\).

|  |
| :--- |
| _Yıllık %0.5 maliyet mi? Ver, hepsini ver… \(Kaynak:_ [_Giphy_](https://media.giphy.com/media/6nXIRmdkjett6/giphy.gif)_\)_ |

### Ya ETH çok düşer de teminatımın altına inerse? <a id="ya-eth-&#xE7;ok-d&#xFC;&#x15F;er-de-teminat&#x131;m&#x131;n-alt&#x131;na-inerse"></a>

Buna dikkat etmek gerekiyor işte. Zira ETH’nin değeri düşerse ekstra ETH yüklemeniz yapmanız lazım. Ya da baştan ihtiyacınız olan nakitten daha fazla ETH koymakta fayda var. Aksi takdirde sistem ETH’nizi “bozuyor” ve %13 gibi bir ceza sonrası kalan paranızdan borcunuzu düşüp size geri veriyor.

Şu anda sistemde kilitli tutulan teminat rakamının kullanılan krediye oranının yaklaşık %200 olduğunu görüyoruz. Yani insanlar gerekli minimum limit olan %150’nin üzerine bir %50’lik bir ekstra teminat koymuşlar kullandıkları krediler için.

### Kim borç veriyor bu sisteme? <a id="kim-bor&#xE7;-veriyor-bu-sisteme"></a>

Aslında kimse kimseye borç vermiyor. Siz elinizdeki ETH’yi teminat gibi kullanıp Dai yaratıyorsunuz. Buradaki soru şu olabilir? Dai’yi satıp ABD Doları aldınız. Kime satıyorsunuz Dai’yi? Genel olarak SabitPara kullanmak isteyen insanlara \(ya da daha önce kredi almış ve şu anda borcunu kapatmak için Dai almak isteyenlere\). Neden SabitPara kullanmak ister insanlar konusunu daha detaylı önceki yazılarımızda [incelemiştik](https://turansert.com/genel/2019/02/15/%28https://ademimerkezi.com/genel/2018/07/20/Orasi-cok-dalgali-sakin-sulara-gel-sabitparalar.html%29).

### Dai parası nasıl sabit kalıyor peki? <a id="dai-paras&#x131;-nas&#x131;l-sabit-kal&#x131;yor-peki"></a>

Dai, bir ABD dolarına sabitlenmiş. Ama alım satım yapıldığı borsada baktığınızda fiyatı aşağı ya da yukarı gidebiliyor. MakerDAO yaratıcıları fiyatın iniş ve çıkış olduğu durumda tekrar 1 ABD dolarına gelmesinin otomatik olacağını düşünüyorlar. Şöyle ki:

Diyelim, Dai fiyatında bir düşüş oldu. Böyle bir durumda geçmişte Dai yaratıp borç almış olanlar, aldıkları borcu yine Dai ile ödeyecekleri için kredilerini ucuza kapatma fırsatı bulabilecekler ve Dai satın alacaklar.

Aynı şekilde Dai fiyatında bir artış olduğunda \(1 ABD dolarından daha yüksek bir fiyata geldiğinde\) insanlar ellerindeki ETH’leri sisteme gönderip 1 ABD doları karşılığı olacak şekilde Dai yaratacak ve bu Dai’yi piyasada 1 ABD Doları’nın üzerinde bozdurma şansı yakalayacaklar. Bu da piyasada 1 Dai’nin 1 ABD Doları’na yaklaşmasını sağlayacak.

Bunun yanında Dai fiyatında ekstrem bir düşüş olduğu durumlar için de acil durum senaryoları hazırlanmış ama şu aşamada çok teknik kaldığı için ilgilenenleri [White Paper](https://makerdao.com/en/whitepaper/)‘ı okumaya davet ederek konuyu kapatıyoruz.

## Peki başarılı olmuş mu MakerDAO? <a id="peki-ba&#x15F;ar&#x131;l&#x131;-olmu&#x15F;-mu-makerdao"></a>

MakerDAO tamamen otomatik bir sistem. Arada herhangi bir aracı yok. Karmaşık anlaşmalar yok - kağıt imza vs yok. Sistem tamamen kodlanmış makineler aracılığıyla işliyor. Teminatınızı koyuyorsunuz, paranızı alıyorsunuz. Teminatınız %150’nin altına düşerse de ETH’niz bozduruluyor ve kredi borcunuzun üzerindeki teminatınız hesabınıza yatıyor. Bu nedenle kredi vermenin getirdiği kağıt ve bürokrasi masrafından kurtulma sistemin en önemli avantajlarından biri.

~~Şu ana kadar iyi gittiklerini söylemek mümkün. Zira halihazırda iki milyon ETH’e yakın miktar MakerDAO sistemi üzerinden borçlandırılmış \(CDP - Collaterized Debt Positions\). ETH’nin şu aralar 120 ABD Doları civarında olduğu düşünülürse yaklaşık 240 Milyon ABD doları bir rakama denk geliyor bu. Ethereum’un kullanım olarak en işlevsel platformlarından biri MakerDAO.~~

Sistem şu ana kadar sıkıntı yaşamadan ilerledi. ETH sene içinde çok ciddi değer kaybetti ama buna rağmen Dai’de ciddi bir sıkıntı olmadı. Bu ileride de olmayacak anlamına gelmiyor tabii. O da bunun riski. ETH’nin aniden %33’değer kaybetmesi durumunda 150 birimlik teminatlar 100 birime düşebilir ve sistem bu ETH’leri satana kadar kredi miktarının altına da inebilir. \(şu an %200 olması biraz daha sistemi rahatlatsa da\). Şu an için MakerDAO sistemi daha çok küçük - ama çok daha büyümesi durumunda tüm ETH değerini bile etkileyecek hale gelebilir olası ani düşüşler.

## MakerDAO her derde deva mı? <a id="makerdao-her-derde-deva-m&#x131;"></a>

Tabii ki hayır. Ancak, bir ürünü ne kadar basit ve istisnaları dışarıda bırakarak şekillendirirseniz o kadar otomatik \(insan eli değmeden\) yürütebilirsiniz tezine güzel bir örnek. Şu anki rakamlar cesaret verici olsa da ileride gerçekten finans piyasalarını sarsıcı bir devrim haline dönüşür mü? Bunu şimdiden tahmin etmek oldukça zor. Neden?

Öncelikle, kriz anlarında test edilmiş bir ürün değil. Test edebilmenin tek yolu da ancak bir kriz yaşamaktan geçiyor - tabii ki stres test benzeri çalışmalar var ama hiçbiri kriz anında ne olacağını tam gösteremiyor. Yukarıda da yazdığımız gibi ETH 2019 yılında değer kaybetti ve MakerDAO’ya hiç bir sıkıntı yaratmadı bu durum. Peki ya ani düşüşler?

En büyük konulardan biri de teminat miktarı. Oldukça yüksek. Ama başta da yazdığımız gibi kredi sisteminin en masraflı ve karmaşık yonlerinden biri kredi derecelendirme ve geri ödememe oranları. Basitlik en başta bu iki özelliği budamaktan geliyor. Tabii ki bunun bir karşı maliyeti olacak, o da yüksek teminat oranları.

## MakerDAO için sonraki adımlar neler? <a id="makerdao-i&#xE7;in-sonraki-ad&#x131;mlar-neler"></a>

MakerDAO özelinde baktığımızda sonraki adımlarda, sistemin organik olarak büyümesi var. Halihazırda tüm ETH miktarının %2’si MakerDAO sistemine kilitlenmiş durumda - bu da onu Ethereum sisteminin en büyük oyuncularından biri yapıyor. Ancak MakerDAO sadece ETH ile işler diye bir kural yok. Başlangıç noktaları bu ancak diğer altyapı protokolleri ile de çalışabilmek onları daha geniş kitlelere yayacak.

Bunun yanında sistemin daha geniş kitlelere yayılması için aslında farklı yatırımcıların ihtiyaçlarına hitap edecek çözümler üst seviye olarak ortaya çıkabilir \(bir nevi Bitcoin üzerine ödemeleri hızlandırmak için kurulan Lightning Network gibi\). Örneğin kredi derecelendirmesi gibi daha karmaşık çözümler. Ve bu çözümler merkezi yapılar da olabilir - zira karmaşık çözümler için merkezi yapılar daha efektif olabiliyor. Dolayısıyla altta merkezi olmayan ve bunun getirdiği kolaylıklardan yararlanan ama üstte daha karmaşık isteklere hitap eden merkezi yapılar \(DeFi -Decentralized Finance- üzeri CeFi -Centralized Finance-\) ilginç açılımlar getirebilir. Tanner Hoban’ın şu [yazısı](https://medium.com/@tehoban/defi-constructing-the-foundation-of-a-new-microeconomy-cb7f21f1c6dd) bu anlamda çok daha detaylı bilgi veriyor ilgi duyanlara.

Not: Teknik olarak çok detaya girmedik ancak DAI dışında MakerDAO’nun bir parası daha var o da MKR. DAI’yi sistemin parası, MKR’yi ise sistemin sermayesi \(equity\) olarak düşünebiliriz. Para alışverişleri DAI ile yapılırken ve DAI ABD Dolarına sabitlenmiş bir para iken, bu para üzerindeki faiz MKR üzerinden ödeniyor. MKR sahibi olanlar aynı zamanda sistemin yönetiminde söz sahibi oluyorlar - örneğin teminat oranlarının belirlenmesi ya da sistemdeki ani düşüşlerde çalıştırılacak mekanizmaların prensiplerinin belirlenmesi gibi. Bu arada olası bir kriz durumunda MKR bir nevi acil durumda kırılacak cam gibi de çalışıyor. Eğer teminat rakamları kredi rakamlarını karşılamaz ise o zaman açık MKR bozularak karşılanıyor - bu da MKR için olumsuz bir durum. Dolayısıyla MKR sahipleri ellerindeki değer azalmasın diye teminat oranı vb rakamlarda olabildiğince konservatif davranmak zorundalar. Bir nevi sistem bu alanda da bir otokontrol getiriyor.

## Bir yılda neler değişti? <a id="bir-y&#x131;lda-neler-de&#x11F;i&#x15F;ti"></a>

Aradan geçen zamanda neler oldu? Bu önemli - özellikle gelişen yeni teknolojilerde ‘zaman’ aslında bu platformların geniş kitlelerce adaptasyon konusunda önlerindeki en büyük engel. Zira insanlar yeni olana kuşkuyla bakıyorlar. Aynı, örneğin Bitcoin örneğinde olduğu gibi. On yıl önce ilk çıktığında kuşkuyla bakanların büyük bir çoğunluğu, bu süre içinde sistemin hiç durmaksızın tıkır tıkır çalıştığını görünce artık Bitcoin’in üstünlüğünü kabul etmiş görünüyorlar. Dolayısıyla, ‘zaman’ bu ürünlerde en önemli test alanı. Bu bir yılda ne gibi sorunlar çıktı, bunlar nasıl giderildi \(ya da giderilebildi mi?\), kullanımı arttı mı, yeni ürünler geldi mi? - bu ürünlerin olgunlaşması hep önemli sorular bunlar.

## Adaptasyonu arttı mı? <a id="adaptasyonu-artt&#x131;-m&#x131;"></a>

DeFi ürünlerinin geçtiğimiz bir yıl içinde kullanımının arttığını rahatlıkla söyleyebiliriz. Mayıs 2020 ortası itibariyle bir önceki yıla göre DeFi içindeki para miktarı neredeyse iki katına çıkarak 860 milyon ABD Dolarına ulaşmış. Bunun yaklaşık yarısı MakerDAO’nun sistemi içinde.

|  |
| :--- |
| _DeFi piyasasının son bir yıllık gelişimi_ [_Kaynak_](https://defipulse.com/) |

Rakamlar başka kripto paralara bakıldığında küçük gelebilir. Ancak şunu unutmayın: bu tip özellikle de para gibi değer taşıyan ve sorun çıktığında kayıpların potansiyel büyük olduğu konularda kullanıcı adaptasyonunun başlangıçta yavaş olması gayet normal. Ancak ‘zaman’ geçip ortaya çıkan sorunlar ve krizler aşıldıkça bu tip ürünlere güven artacak bu da ürünlere olan talebe olumlu bir etki yapacak.

## Sorunlar/krizler çıktı mı? <a id="sorunlarkrizler-&#xE7;&#x131;kt&#x131;-m&#x131;"></a>

Peki aradan geçen zamanda hiç kriz yaşadı mı MakerDAO? Gayet tabii.. Ancak öncelikle şunu belirtmekte fayda var. Bu tip ürünler/platformlar deneysel ve yeni.. Sorun çıkması gayet normal. Neden? Birincisi - nihayetinde bunlar birer yazılım. Yazılımları insanlar yazıyor. Tamam kullanılmadan önce gözden geçiriliyor olsa da hata olması çok normal. Bir diğer neden ise, sistemin tasarımcıların her tür senaryoyu öngörmelerinin mümkün olmaması. İşte zaman içinde kullanıldıkça ortaya sorunlar çıkıyor ve bu sorunlar yine zamanla gideriliyor, sistem “kurşun geçirmez” bir hale geliyor.

MakerDAO da benzer bir krizi 2020’nin Şubat ayı içinde yaşadı. ETH piyasa değerinin bir günde %53 oranında düşmesi kimsenin beklemediği bir senaryo idi.

|  |
| :--- |
| _ETH’nin yıllık değişimi ve 12 Mart günü %53 düşmesi_ [_Kaynak_](https://www.coindesk.com/price/ethereum) |

Bunun üzerine bir de sistem içindeki bir açık nedeniyle yaklaşık 5 milyon ABD Doları tutarında kontrat iptal oldu \(o zamanki sistemde bulunan hesapların yaklaşık %1.5’u kadar\). Sistemin güvenliğini sağlayan topluluk bu parayı karşılayarak bireylerin mağdur olmasını önledi. \(Teknik detayı en sondaki dipnot’ta bulabilirsiniz\).

## Yeni ürünler eklendi mi? Gelişimler ne yönde? <a id="yeni-&#xFC;r&#xFC;nler-eklendi-mi-geli&#x15F;imler-ne-y&#xF6;nde"></a>

Oldu tabii. Sistem yukarıda anlattığımız tek bir ürünle basit bir şekilde kuruldu ancak nihai vizyonu kendi kendine çalışan bir merkez bankası olmak. İlk kurulduğunda MakerDAO para olarak yalnızca ETH kullanıyor idi. 2019 Kasım ayında ETH dışında çok paralı bir sisteme geçtiler. Böylelikle teminat olarak ETH değil başka kripto paraların da sisteme konabilmesinin yolu açıldı. İlk aşamada BAT \(Brave Token\) ve USDC \(ABD Dolarına sabitlenmiş bir başka kripto para\) da teminat olarak kabul ediliyor artık.

Bunun yanında artık DAI yatırıp bununla faiz kazanma imkanına da kavuştu bireyler. Bunu bir nevi paranızı dolar vadeli hesaba yatırmak olarak düşünebilirsiniz. Yapılan bu ekleme ile aslında MakerDAO kendi başına bir merkez bankası gibi çalışmaya başladı. Çünkü ilk çıktığında yazının başında bahsettiğimiz kullanıcılara borçlanarak DAI yani para arzı yarattıran ve kullanıcının ödeyeceği faizi değiştirerek esasında bu para arzını kontrol edebilen bir sistem idi MakerDAO. Şimdi bu yeni gelen yenilik ile kullanıcılara yaratılmış DAI’yi yatırım olarak değerlendirme hakkı veriyor ve bu yatırım karşılığı kullanıcıya ödenecek faiz oranını değiştirerek aslında bir nevi para talebini de kontrol ediyor. Böylece hem arz hem talep alanında aslında bir merkez politikasının gösterge faizler ile oynayarak yarattığı sistemin bir benzerini kuruyorlar. Bu başlı başına bir yazı konusu ve ayrı bir yazıda daha kapsamlı değerlendireceğiz. Ancak hemen bir parantez açarak, DAI yatırım hesabı olarak adlandırılan bu fonksiyonun deneme aşamasında olduğunu ve şu an için durdurulduğunu belirtelim.

## Gelecek nasıl görünüyor? <a id="gelecek-nas&#x131;l-g&#xF6;r&#xFC;n&#xFC;yor"></a>

DeFi yani merkeziyetsiz finansın geniş kesimlerce benimsenmesi için birkaç alanda gelişme kaydetmesi gerekiyor:

* Kullanıcı dostu arayüzlerin gelişmesi
* Daha geniş kesimlerce ulaşılabilir olması
* Likiditenin artması
* Volatilite’nin \(değerdeki beklenmedik iniş-çıkışların\) azalması
* Türev olarak kullanılan alt varlıkların olgunlaşması \(örneğin ETH’de yaşanan yukarıda anlattığımız kriz\)
* Ürünlerin üzerine kuruldukları altyapı teknolojilerinin çok daha kusursuz hâle gelmesi

Yazıyı uzatmamak için maddeler halinde bırakalım bu gelişmeleri - yukarıdaki her bir başlık kendi içinde birer yazı konusu çünkü.

## Sonuç <a id="sonu&#xE7;"></a>

MakerDAO, tamamen dijital dünyada kurulmuş bir merkez bankası deneyi esasında. Şu an için deneysel olarak ilerliyorlar, kâh hızlanıyorlar, kâh tökezliyorlar. Ancak şu ana kadar iyi idare ettiler. Eğer başarılı olurlar ise, önümüzdeki yıllarda ismini çok daha sık duymaya başlayacağımıza emin olabilirsiniz.

Her zaman söylediklerimiz ile bitirelim o zaman. Aracılar kullanıcıların beklediğini vermekte zorlandıkça bu tip hizmetlere talep de giderek artacak. Nedir insanların bu hizmetler ile ilgili beklentileri? Herkese açık olsun \(yalnızca parası olana değil finansal sisteme erişimi olmayan milyarlarca insan da kullanabilsin\), pratik olsun \(onlarca doküman, belge istemesin kullanmadan önce\) ve ucuz olsun \(kullanıcılar hizmet verenlerin oturdukları plazaların kiralarını ödemek zorunda kalması\). Bunun gerçekleşmediği durumlarda klasik finans hizmeti verenlerin pastadan aldığı pay azalacak, yeni sistemler giderek insanlığın hayatına daha çok girmeye başlayacak.

Not: Teknik olarak çok detaya girmedik ancak DAI dışında MakerDAO’nun bir parası daha var o da MKR. DAI’yi sistemin parası, MKR’yi ise sistemin sermayesi \(equity\) olarak düşünebiliriz. Para alışverişleri DAI ile yapılırken ve DAI ABD Dolarına sabitlenmiş bir para iken, bu para üzerindeki faiz MKR üzerinden ödeniyor. MKR sahibi olanlar aynı zamanda sistemin yönetiminde söz sahibi oluyorlar - örneğin teminat oranlarının belirlenmesi ya da sistemdeki ani düşüşlerde çalıştırılacak mekanizmaların prensiplerinin belirlenmesi gibi. Bu arada olası bir kriz durumunda MKR bir nevi acil durumda kırılacak cam gibi de çalışıyor. Eğer teminat rakamları kredi rakamlarını karşılamaz ise o zaman açık MKR bozularak karşılanıyor - bu da MKR için olumsuz bir durum. Dolayısıyla MKR sahipleri ellerindeki değer azalmasın diye teminat oranı vb rakamlarda olabildiğince konservatif davranmak zorundalar. Bir nevi sistem bu alanda da bir otokontrol getiriyor.







Not: Basitçe MakerDAO olayını anlatmaya çalışırsak, olay şu: Sistemin özünde kullanıcıların ellerindeki ETH \(Ether\)’leri teminat olarak gösterip DAI yaratmaları \(borçlanmaları\) var. Yatırılan teminatın yaratılan paranın %150’si olması gerekiyor ki sistem işlesin. Neden bu teminat var?

Klasik bankacılıkta karşımıza çıkan karşı partinin borcunu ödememe riski \(counter-party risk\) burada ekstra teminatlandırma ile çözülüyor. Zira normal hayatta yani klasik bankacılıkta bu riski bertaraf etmek için bankanın kredi derecelendirme uzmanları, kredinin ödenmemesi durumunda tahsilat için avukatları ve tahsilat elemanları var. Dijital dünyada bunların hiçbiri olmadığı için karşı parti riskini önlemenin tek yolu teminat miktarını olabildiğince fazla tutmak. İleride dijital kimliklerin daha da geliştiği ve bu kimlikler üzerinden karşı parti riskinin daha yönetilebilir hâle geldiği noktada bu yüksek teminat miktarları da azalacak muhtemelen.

Ancak 12 Mart günü ETH fiyatının %53 düşmesi nedeniyle neredeyse bütün kredilerin karşılığı olan teminatlar pula döndü. Diyelim 100 ETH’ye denk gelecek bir kredi almak istiyorsunuz. Alacağınız kredi DAI cinsinden, DAI ise dolara sabitlenmiş bir para. Bunun için minimum 150 ETH teminat koymanız lazım. Ama siz ihtiyatlı davranıp 200 ETH koydunuz. ETH bir günde %53 değer kaybedince dolar cinsinden 200 ETH teminatınız, bırakın aldığınız kredinin 150%’sini karşılamayı, bir anda %94’ünü karşılar hale geliyor \(200x\(1-0.53\)=94\). Bu durumda da sistem teminatınızı bozuyor ve paranız yanıyor.

Böyle bir durumda makul olanı, ya ekstradan ETH koyarak ya da yarattığınız DAI’lerin bir kısmını yok ederek teminatı yeniden %150’nin üzerine çıkararak kredinizin yanmasını önlemek. Ancak tam o sırada benzer şekilde işlem yapmak isteyenlerden dolayı ETH işlemleri için kullanılan gas ücretlerinin zıplaması ve sistemsel sorunlar nedeniyle pek çok kişi teminatlarını tamamlayamadı. Açıkta kalan krediler açık artırma sistemi ile satılırken, sistemsel bir hatadan dolayı pek çok kontrat sıfır değer ile satıldı. Böyle yaklaşık 5 milyon ABD doları kadar büyüklükte bir kontrat bu durumdan etkilendi.

MakerDAO yöneticileri, sistemin güvenliğini sağlayan MKR token sahiplerine dönerek zarar görenleri zor durumdan kurtaracak bir plan önerdiler. Bu sayede kontratı yananların durumları düzeltildi.







\_\_

