# Compound: Klasik bankacılığın rakibi

Kripto dünyasında ise DeFi hareketi benzer şekilde bize yeni alternatifler sunuyor. Henüz çok küçük ve deneyseller. Ama belli bir potansiyel sağlayacakları kesin. Gelin bu bölümde bu alandaki ilginç yapılardan [Compound](https://compound.finance/)‘a bakalım:

Günümüzde klasik bankacılığın karşısına pek çok rakip çıkıyor. Özellikle Avrupa ve Amerika’da adına [Neobank](https://en.wikipedia.org/wiki/Neobank) denen yeni oluşumlara her geçen gün yenileri ekleniyor. Bunlar mevcut bankacılık hizmetlerini çok daha ucuza sağlıyorlar. Neden? Temelde klasik bankaların geçmişten gelen artık kemikleşmiş maliyetlerinin hiçbirine sahip değiller.

### Nedir bu Compound?

[Compound](https://compound.finance/) klasik bankacılık sisteminin bir alternatifi.

Klasik bankacılık en basit tarifi ile aslında mevduat sahiplerinin yatırdığı paraların ihtiyaç sahiplerine kredi olarak verilmesi. Mevduata verilen ile kredilere uygulanan faizler arasındaki fark da esas olarak bir bankanın kâr marjı \(spread\).

Compound da benzer şekilde mevduat sahipleri ile kredi verenler arasında banka benzeri çalışan Ethereum üzerine kurulu bir sistem.

![Image by Gerhard B&#xF6;gner from Pixabay](../.gitbook/assets/02031-compound-money-3405700_1920.jpg)

### Nasıl çalışıyor sistem?

Compound sisteminde bireyler ellerindeki kripto paraları mevduat olarak yatırıp faiz kazanıyorlar. İhtiyacı olan bireyler ise bu faizin bir miktar fazlasına bu kripto paraları kredi olarak kullanıyorlar. Bu “bir miktar fazla” Compound’un bu işten aldığı komisyon. Bankalara göre çok daha az.

#### Faiz nasıl belirleniyor?

Sistemin faiz belirleme yöntemi aslında bankalara benziyor: Kredi isteyen ve mevduat yatıranların sayısına ve oluşturduğu havuza, yani arz ve talebe göre bir algoritma tarafından hesaplanıyor faiz.

Ne sıklıkla? Çok! Ethereum üzerine kurulu bir sistem olarak Ethereum blok zincirine paralel şekilde borç verenlere ya da alanlara uygulanacak faiz her 15 saniyede bir belirleniyor.

Basitçe denge sistemi ile çalışıyor sistem: Örneğin, faizlerin düşmesi durumunda mevduat sahiplerinin paralarını çekeceği, bunun da faizleri artırarak yeni bir denge oluşturacağı şeklinde özetlenebilecek temel ekonomik prensiplere dayanıyor.

#### Faiz çok oynak görünüyor, ya sisteme giriş-çıkış nasıl oluyor?

Şunu da hemen belirtelim. neredeyse anlık değişen faize paralel olarak sisteme giriş çıkış da istenildiği zaman yapılabiliyor. Yani kredi aldığınızda istediğiniz zaman geri ödeyebiliyorsunuz. Aynı şekilde mevduat yaptığınızda da istediğiniz zaman paranızı çekebiliyorsunuz.

#### Tahsilat riski nasıl aşılıyor?

Peki bankacılığın meşhur olayı “alacak riski \(counter-party risk\)” nasıl bertaraf ediliyor? Diğer DeFi projelerine \(örneğin MakerDAO\) benzer şekilde kredi alanın belli bir kripto parayı teminat olarak yatırması gerekiyor Compound sisteminde. Her kripto paranın teminat oranı farklı. En likit olan örneğin ETH en düşük teminat oranına sahip.

#### Hangi paralarda işlem yapılabiliyor?

Şu aşamada ETH, WBTC \(Bitcoin’in değerine eşit ETH bazlı bir sentetik para\), Augur gibi Ethereum bazlı kripto paralar ile USDC, Tether, DAI gibi sabit paralar ile [mevduat yapabilir ya da kredi alabilirsiniz sistemden](https://compound.finance/markets).

#### Kimler kullanıyor?

Neden bir kişi sistemden borç almak ister? Teminat verecek kadar “param” varsa neden borç almak isteyeyim? Temel nedeni spekülatif hareketler. Örneğin bir nedenle sabit bir paraya sıkıştınız ancak elinizdeki ETH’i satmak istemiyorsunuz çünkü artacağını düşünüyorsunuz. Böyle bir durumda bu ETH’i teminat gösterip karşılığında ETH kredi alabilirsiniz.

Neden borç verirsiniz peki? Yatırım amaçlı. Bir süreliğine kenarda tutmak istediğiniz bir paraya faiz kazanmak isterseniz bu sistem tam size göre.

### Kim kurmuş bu Compound’u? Güvenilir mi peki?

Compound’u kuran ekip tecrübeli, ayrıca arkalarında teknoloji dünyasının en prestijli girişim sermayeleri var. Daha önce pek çok büyük kripto projesine yatırım yapmış [a16z](https://a16z.com/crypto/) ve [polychain capital](https://polychain.capital/) ve ABD’nin en büyük borsası [Coinbase](https://www.coinbase.com/)‘in yatırım [fonu](https://ventures.coinbase.com/) bunlardan en belirgin ikisi. Bir DeFi hareketinin temel özelliği olarak tamamen şeffaf yürütülen sistem hem yatırımcılara hem de kullanıcılara bir nebze iç rahatlığı verebilir. Görebildiğim kadarıyla sistemdeki tek kapalı noktaya gelelim şimdi.

#### Tamamen merkeziyetsiz mi?

Hayır. Merkeziyetsizlik “[uzun ince bir yol](https://www.youtube.com/watch?v=PXw3f9YTqV0)” ise Compound bu yolun ilerisinde ama sonunda değil. Olacak mı, o da belli değil açıkçası.

Merkezilik nerede var? Öncelikle, geliştiren ekip merkezi ama bu o kadar da kritik değil.

Asıl kritik olan, kredi alanlara hangi faiz oranı uygulayacağına bir “robot” karar veriyor. Peki bu robot nasıl karar veriyor? Compound’un içindeki \(içeriği çok da bilinmeyen\) bir algoritma sistemdeki arz ve talebe göre faizi belirliyor. Yani arz ve talep toplanıp bir havuz şeklinde düşünülüyor.

Eğer tam merkeziyetsiz bir yapı düşünüyor olsaydık, o zaman direkt alıcı ile verici pazaryeri misali birbirleri ile direkt biraraya gelebilirdi. O zaman da böyle bir karar kutuya ihtiyaç olmazdı. Birkaç yıl önce Dharma protokolü böyle bir niyetle ortaya çıktı ancak o projenin çok başarılı olduğu söylenemez.

### MakerDAO’dan farkı ne?

Compound, MakerDAO’ya göre bir parça daha basit. Bir analoji vermek gerekirse, Compound bir banka, MakerDAO ise merkez bankası.

Belki de bu nedenle MakerDAO kendi sistemini sürdürmek için bir sabit para \([Dai](https://community-development.makerdao.com/makerdao-mcd-faqs/faqs/dai)\) yaratmışken, Compound’da benzer bir stabil para yok - onlar Dai de dahil başka paraları kullanıyorlar, aynı bir banka gibi. \(Sistemden Compound'un yönetim tokeni olan COMP ile kredi ya da mevduat işlemi yapabilirsiniz ancak COMP stabil bir para değil\). 

Compound’un nihai hedefi, faizi belirlemede bir gösterge olacak, üzerine pek çok başka uygulamanın yazıldığı, kurucularının hakimiyetinden uzaklaşmış merkeziyetsiz bir protokol olmak.

Öte yandan Compound’un MakerDAO’dan bir diğer farkı da yönetim kısmında. Her iki sistemde de yönetim hakları için bir token çıkarılmış durumda: MakerDAO için [MKR](https://community-development.makerdao.com/makerdao-mcd-faqs/faqs/mkr-token), Compound için ise 2020 Haziran ayında çıkan COMP. Gelin şimdi de COMP yönetim tokenına yakından bakalım. 

### Nedir COMP token?

Compound  ilk kurulduğunda girişim sermayesi alıp, ürün olarak merkeziyetsiz ama yönetim olarak merkezi, sonrasında yavaş yavaş yönetimi de merkeziyetsiz hale getirmek olarak özetlenebilecek bir yol haritası çizdi kendine. Pek çok prestijli girişim sermayesinden yatırım aldı. İlk olarak ürünlerini kullanıcıların beğenisine sunup, sorunlarını çözdü.

Sıradaki hamle benzer şekilde yönetimi de merkeziyetsiz hale getirmek idi. Bunu da demokratik bir şekilde geniş bir kitle tarafından yönetilebilmek için COMP adı verilen bir token çıkarıp kullanıcılarına dağıtmaya başlayarak yaptılar.

Bu yolu seçmelerindeki en önemli neden, kullanıcıların tokenlara sahip olmaları durumunda gelecekte sistemin güvenliği ve doğru bir yolda ilerlemesi konusunda ellerinden geleni yapacağını düşünmeleri idi.

### Nasıl işledi COMP hamlesi?

Compound, COMP tokenları dağıtırken kullanıcıları tamamen serbest bıraktı. Bu ne demek? Genelde, örneğin bir şirket çalışanlarına hisse dağıtırken, çalışanlar hisseyi alıp satıp kaçmasınlar diye onlara bu hisseleri zamana yayarak verir. DeFi platformların kimileri de yönetim tokeni dağıtırken bu yolu izledi. Örneğin [Futureswap](https://www.futureswap.com/) kendi kullanıcılarına verdiği yönetim tokenlarını bu şekilde “başkasına devredemezsiniz” [şartıyla dağıtmaya başladı](https://defirate.com/futureswap-launches/) \(ve kısa bir süre sonra da satışı durdurdu\).

Herhangi bir kısıtlama getirilmediği için kullanıcılara verilen bu COMP tokenlar anında çeşitli borsalarda işlem görmeye başladı. 

Kısıtlı sayıda \(10 milyon adet\) olarak basılan olan COMP tokenlar başlangıçta 20 ABD Doları gibi bir değerden işlem görürken sonrasında yaklaşık 910 ABD Dolarına kadar [çıktı](https://www.coingecko.com/en/coins/compound).

Tabii, bu hemen akıllara 2017 yılının meşhur ICO’larını getirdi. Zira, hatırlarsanız o zamanlar binbir proje binbir vizyon ile piyasadan hatırı sayılır bir parayı “kaldırmıştı”. COMP da acaba öyle mi?

Cevap sanırım hem evet hem de hayır. Önce neden değil ona bakalım sonra neden benzediğini tartışırız.

Öncelikle, 2017 yılının ICO projeleri tamamen kağıda yazılı bir hayal satıyorlardı. Compound’un durumu öyle değil - zira sahip oldukları ve gayet iyi işleyen bir sistemleri var halihazırda.

İkincisi, ICO’larda girişimlerin çıkardığı tokenlar tamamen kâr amacı güden yatırımcılara para karşılığı satılmıştı \(her ne kadar bu tokenların bir gün sistemi kullanmakta da işe yarayacağı söylense de\). Şimdi ise sistem üzerinden alım satım yapan kullanıcılara yaptıkları işlem karşılığı token verilmesi var. Dolayısıyla sistemi büyütmeye yarayan bir token dağıtımı söz konusu.

Neden 2017’in token projelerini andırıyor? En önemli nedeni kullanıcılarda “aman kârlı bir projeyi kaçırıyorum” şeklinde bir panik \(FOMO\) yaratmış olması. Halbuki, Compound’un CEO’su bile bu tokenların bir kâr amacı gütmeyeceğini söylüyor.

### Niye bu kadar talep gördü COMP?

En önemli nedeni, aslında yavaş yavaş artan token değerinin kendi kendine bir sarmala dönüşmüş olması. Ne demek bu?

Compound’un kredi vermek ya da almak işine yaradığına geçen kısımda değinmiştik. Sisteme kredi verdiğinizde karşılığında bir faiz alıyorsunuz. Ancak bunun yanında, şu anda bir de COMP token kazanıyorsunuz. Ve bu tokenı aldığınız gibi piyasada satabiliyorsunuz. Böyle olunca aslında kazandığınız para kat be kat artıyor.

COMP bunu kendi sistemini geniş kitlelere kullandırabilmek için yaptı. Zira bu tip DeFi platformların en büyük sorunu likidite sıkıntısı. Bu da bir tür sarmal. Kullanıcı olmayınca likidite olmuyor, likidite olmayınca da yeni kullanıcı gelmiyor. Bu sarmalı kırmak gerek. Sanırım Compound, COMP token ile bu sarmalı kırmayı başardı. İki hafta içinde Compound sisteminine bağlanan kripto para değeri beş kat artarak DeFi piyasasının en büyüğü olan MakerDAO sistemini geçti.

Böyle bir sıçramanın ne kadar sağlıklı ya da gerçekçi olduğu ise tartışmaya açık. Zira sistemde hem kredi veren hem kredi alan COMP kazandığı için, türev enstrümanlar aracılığıyla çoklu miktarda işlem yapıp kat kat COMP kazanma imkanları da hemen kullanılmaya başlandı.

### COMP tokenların değeri nereden geliyor?

Bu arada şunu da belirtelim. Compound, ellerinde COMP tutanlara herhangi bir ekonomik menfaat vaat etmiyor. Şu an için sadece sistemin hangi yöne gideceği konusunda oy verecek ellerinde COMP tutanlar.

Peki ileride bu değişebilir mi? Örneğin sistem kâr dağıtmaya başlayabilir mi? Kim bilir? COMP tokenlar bu hızla giderse 4 yıl sonra tamamen dağıtılmış olacak. Yönetim de tamamen merkeziyetsiz bir hale gelecek. O zaman COMP sahipleri oturup demokratik olarak kâr dağıtmaya karar verebilirler mi? Verebilirler tabii, neden olmasın?

İşte bu ileride kâr dağıtma ihtimalini sevdi sanki kimi uzun vadeli ve sadece ekonomik getiriye bakan yatırımcılar.

Ancak unutmamak lazım: bu aslında iki ucu keskin bir kılıç. COMP sayesinde yönetimi eline geçiren istediğini yapabilir. Kâr dağıtma kararı verebileceği gibi, yeni token dağıtma yolunu da seçebilir. Hepimizin aklı Bitcoin’in 21 milyon ile sınırlı olmasına gidiyor ama orada kanunu kod yazıyor ve bozulması merkeziyetsiz yapının iyice oturmuş olması nedeniyle neredeyse imkansız. Ama COMP için bu kadar kesin konuşmamak gerekiyor.

### Peki kim alıyor bu COMP tokenları?

Şu anda hızlı yükseliş ile gözleri kamaşan spekülatörler - ki bunlar kısa vadeli kazanç peşindeler. Bu spekülatörlerin Compound sisteminin yönetimine katılmak konusunda çok büyük bir arzusu olduğu pek düşünülemez.

Ama sadece onlar değil. Compound’un gelecekte hangi yöne gitmesi konusunda hassas olan kesimler de var. Kim bunlar? Öncelikle, şimdiye kadar Compound’a yatırım yapmış olan fonlar - zira yaptıkları yatırımın ne yöne gideceği konusunda kontrolü ellerinden kaçırmak istemiyorlar.

Compound’un mevcut yatırımcıları ile sınırlı değil COMP’a ilgi duyanlar. İlginç ama Compound sistemi üzerine kurulu girişimlere yatırım yapan girişim sermayeleri de bu COMP’lara sahip olmak istiyor. Zira, yatırım yaptıkları girişimlerin üzerine kurulu olduğu Compound altyapısının istemedikleri şekilde değiştirilip kendi yatırımlarına sorun çıkarması ihtimalinden kaçınmak arzusundalar.

Bunun dışında, ilginç bir başka görüş daha var: Biliyorsunuz, dünyanın hemen hemen yerinde, kripto paraların para mı yoksa hisse mi olduğu tartışılıyor. Neden? Vergi yüzünden. Para olarak değerlendirilmeleri durumunda pek çok ülke \(örneğin BTC için ABD\) vergi uygulamıyor - ancak hisse senedi olursa işler değişiyor - o zaman vergi var. Hisse senedinin teoride en önemli özelliği ne? Sahiplerine temettü yani kâr payı dağıtması. Compound en azından şimdilik böyle olmayacağını söylüyor - ama ileride bu değişebilir.

Neden şimdi değil de ileride? Birkaç nedeni olabilir. Birincisi, kripto paralar ile ilgili kural ve yorumları değişme ihtimaline karşı şimdiden kendilerine “hisse” damgasının vurulmasını istemiyor olabilirler. İkincisi, Compound sistemi şu anda yönetim ve işletim olarak ABD’de kurulu bir şirket. İleride bir altyapı haline geçer ve tamamen merkeziyetsiz olarak kripto âleminde yaşar ise Compound’a nasıl ve hangi ülkede vergi uygulayacaksınız?

### COMP token üzerine son birkaç söz

İşte gelecekte karşımıza çok çıkacak olan kripto para sanal dünyası ile fiziki dünya arasında yaşanacak zihin açıcı sorulardan bir tanesi size: Bir gün Facebook, Google gibi büyük devlerin fiziki ülkelerden daha güçlü olacağını düşünenler var. Peki bu bir şekilde gerçek olursa, BTC, ETH gibi platformların da kendi içlerinde bağımsız adacıklar olarak bu merkezi yapıların yanında kendilerine yer bulmaları mümkün olabilir mi?

