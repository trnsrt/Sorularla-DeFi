# Yearn Finance: DeFi'de merkeziyetsiz portföy yönetimi:

Kripto paralar pek çok insan için oldukça teknik ve karışık. Sıradan bir kripto para borsasına girmeye çalışsanız bile bir sürü prosedürden geçmek zorundasınız. Merkeziyetsiz finans alanında durum daha da içler acısı. Neden? Sıralayalım…

* Bir kere klasik sistemlere göre temel farklar var. Anlamak için çaba sarfetmek, çok okumak ve kendini eğitmek gerekiyor.
* Denetim yok. Yatırım yaptığınız bir üründe sıkıntı yaşarsanız kendiniz ile baş başasınız.
* Mevcut ürünleri açıklayıcı çok kaynak yok. Özellikle Türkçe olanlar çok az.
* Her geçen gün yeni bir ürün ekleniyor. Daha birini anlamadan bir yenisi çıkıyor ortaya.
* Üstelik de işlem maliyetleri çok yüksek. İşlem yapmaya kalktığınıza onlarca dolar komisyon ödemek zorunda kalıyorsunuz.

Şöyle bir hizmet olsa yatırımcının parasını alıp değerlendiren? O yere parasını koyup sonrasında gönül rahatlığı içinde işine dönse? Var mı böyle bir yer?

|  |
| :--- |
| _Image by_ [_Gerd Altmann_](https://pixabay.com/users/geralt-9301/) _from_ [_Pixabay_](https://pixabay.com/) |

Öncelikle söyleyelim, yukarıda bahsettiğimiz tüm dertlere çare olacak bir çözüm henüz yok. Daha doğrusu böyle çözümler mevcut ancak bunların çoğu merkezi yapılar. Paranızı alıp değerlendiren fonlar ya da aracılar var ama bu merkeziyetsizlik ruhuna çok da uygun değil. Peki ya merkeziyetsiz çözümler?

Gelin bu bölümde, 2020 yazında DeFi’nin parlayan yıldızlarından biri haline gelen, ‘merkeziyetsiz portföy yönetimi’ girişimi [Yearn](https://yearn.finance/) platformuna bakalım.

### Ne yapar Yearn protokolü?

Yearn protokolü çok basit olarak, bir kaç belirlenmiş strateji doğrultusunda paranızı otomatik şekilde değerlendirmeye yarıyor. Çıkış amacı, riski az stabil paraları farklı platformlarda değerlendirerek ekstra getiri yaratmak. Bir başka deyişle, **geliri maksimize etmek yerine riski minimize etmek yoluya kullanıcısına makul bir getiri sağlama** hedefindeler.

Yearn protokolünün sloganı “basitleştirilmiş merkeziyetsiz finans”\(“DeFi simplified”\). Ancak Yearn burada ölçüyü bir parça kaçırmış sanki. Sistemin kullanıcı arayüzleri gayet basit. Örneğin diğer tüm DeFi protokollerinde olduğu gibi kullanıcı web sitesine girdiğinde saniyeler içinde kripto cüzdanınızı bağlayıp kullanmaya başlayabiliyor. Ancak giriş ekranı o kadar basit ki, kullanıcının ne yapması gerektiğini anlaması gerçekten zaman alabiliyor, çünkü herhangi bir açıklama yok. Bunun temel nedeni, sistemin kurucusu [Andre Cronje](https://twitter.com/AndreCronjeTech)‘nin bir programcı olarak ürüne odaklı olması ve birinci önceliği hızlı ürün çıkarmaya vermesi. Adeta “bu işi bilmiyorsan hiç buralarda vakit geçirme” dercesine hafif bir üstten bakış havası seziyor insan. İşte tipik bir DeFi sıkıntısı: Kullanıcı dostu, net, açıklayıcı arayüz eksikliği.

Neyse ki topluluğun katkıları ile neyin ne olduğu ve nasıl yapılacağını anlatan [sayfalar](https://docs.yearn.finance/) websitesine sonradan eklenmiş. Ancak bu sayfaları bulmak bile kullanıcı için kolay değil. Neyse, konudan fazla sapmadan gelin ne tip ürünler var Yearn içinde, ona bakalım.

### Ne tip ürünler var?

Yearn sitesine girince onlarca ürün görebilirsiniz, ancak temel olarak iki ana grup olduğunu söyleyebiliriz. Bunlardan birincisi, ilk çıkan ürünleri olan Earn. Bu ürünün başarısı sonrası, daha riskli bir alana girip ikinci ürünleri yVault’u çıkarıyorlar. Bunun yanında tamamen pazarlama ağırlıklı bir sigorta ürünü ve deneme aşamasında olan pek çok farklı projeyi de sitede görmek mümkün.

#### Earn

Kullanıcının parasını alıp, çeşitli borç verme protokolleri arasında gezdirerek en yüksek getiriyi otomatik olarak sağlayan [Earn](https://yearn.finance/earn) Yearn platformundan çıkan ilk ürün.

İki önceki bölümde detaylı olarak baktığımız borç verme platformu Compound ve rakipleri Aave ve dYdX, Earn ürününün elindeki parayı dolaştırdığı birbirine rakip üç temel DeFi projesi. **Kullanıcıların ağırlıklı olarak ABD Doları’na bağlı stabil paralarını değerlendirdiği bu ürün, hem getirisi hem de riski düşük bir yatırım alternatifi olarak öne çıkıyor. Özet olarak DeFi dünyasındaki birbirinden inişli çıkışlı kripto paralarının riskini almak istemeyen yatırımcılar için makul getiriler sunan bir araç.**

Neden kullanıcılar Earn kullansın? Bir kaç temel nedeni var.

Öncelikle kullanıcının farklı borç verme protokollerini sürekli olarak kontrol etmek için zamanı yok, bunun yerine elinde olan bir stabil parayı Yearn protokolüne koyup kendi işine dönebilir - üstelik herhangi bir komisyon ödemeden.

İkincisi, Earn para transferi sırasında çıkabilecek yüksek işlem ücretlerinden kullanıcıyı kurtarıyor - sonuçta işlem yaptığınızda ödenecek ücreti işlemin tutarı değil, yapılacak işlemin ne kadar karmaşık olduğu ve ne kadar hızlı yapmak istediğiniz belirliyor. Kullanıcının 100 ABD Doları’nı platformlar arası değiştirirken ödeyeceği ücret ile Earn’in 10 milyon ABD Doları için aynı işlemi yapmasında ödeyeceği ücret arasında öyle ahım şahım bir fark yok.

Üçüncü önemli neden ise, Earn içinde yatırımcıların para yatırabildiği dört farklı stabil para var. Bunlar DAI, USDC, USDT, TUSD. Bütün bu paralar bir başka protokol olan Curve içinde özel bir havuzda tutuluyor. Curve, Uniswap benzeri ancak stabil paralar üzerine uzmanlaşmış merkeziyetsiz bir borsa. Curve kullanıcıları, bu dört stabil paraları alıp sattıkça bu havuza komisyon veriyorlar. Bu komisyonlar da Earn’e para koymuş yatırımcılara gidiyor. Dolayısıyla, bireysel olarak elde edemeyeceği ekstra bir gelir kapısına sahip oluyor kullanıcılar.

#### yVaults

Yearn ekibinin çıkardığı ikinci ürün ise, DeFi piyasasının 2020 yazında yaşadığı hızlı yükselişin temel nedenlerinden olan getiri çiftçiliği \(yield farming\) furyasından yararlanmayı hedefleyen [yVaults](https://yearn.finance/vaults) oldu.

Hatırlatmak gerekirse, getiri çiftçiliği temel olarak, herhangi bir platforma likidite sağlama karşılığında komisyon geliri ile birlikte o platformun yönetim tokenlarını da kazanmak demek. DeFi platformlarının yönetimini merkeziyetsizleştirmek için kullanıcılara dağıtılan bu tokenlar, [Uniswap](https://app.uniswap.org/) gibi merkezi olmayan borsalarda hızlıca işleme sokularak yatırımcılar ciddi kazanç sağladılar. **yVault, bir yandan Earn gibi kullanıcının parasını stabil paralara koyuyor bir yandan da getiri çiftçiliğinden para kazanmaya çalışıyor**.

yVault’un Earn’e göre farklarına bakalım isterseniz hızlıca:

Earn, strateji olarak en iyi borç verme oranına bakıp ona göre kullanıcının parasını uygun platforma yönlendiriyor. yVault ise bu getirinin yanında ilgili protokolün verdiği yönetim tokenlarının piyasa değerlerini de dikkate alıyor. Kullanıcının parasını da her iki getirinin toplamının en yüksek olduğu yere yatırıyor.

Dolayısıyla yVault Earn’e göre daha riskli bir strateji güdüyor. Neden? Zira, burada Earn gibi borç verme protokollerinde otomatik para dolaştırmanın ötesinde, getiri çiftçiliği işini mekanik olarak yapan bir kontrolör var. Bu merkeziyetsizlik ruhuna bir parça aykırı, ancak stratejiyi belirlemek ve uygulamak için böyle bir “aracı” gerekli gibi görünüyor.

Öte yandan, yVault ürünleri “al ve tut” stratejisi izledikleri için hangi üründen para kazandılar ise, kazandıklarını gidip yine aynı ürüne yatırıyorlar. Dolayısıyla bu getiri çiftçiliğinin prim yaptığı dönemlerde toplam getiri oranını daha da artırabiliyor.

Bu arada, kontrolör olması manuel işlem anlamına geliyor. Bu nedenle yVault, ürünlerinde getiri çiftçiliğinden kazanılan kârın %5’ini komisyon olarak alıyor. Bir de kullanıcı parasını çekmek istediğinde eğer o ürünün boşta parası varsa kullanıcıya ücretsiz geri ödeme yapıyor, ama tüm para yatırım olarak değerlendirilmişse o zaman yatırımı bozma ücreti olarak %0.5 oranında bir komisyon kesiyor.

Başta da bahsettiğimiz gibi Earn ve yVault, stabil paralar üzerinden yatırımcıya riski az getiri stratejisine odaklanmışlar. Bunlara ek olarak kullanıcının stabil olmayan volatil paraları değerlendirebileceği bir başka ürün daha yaratmış Yearn. Aslında yapılan iş aynı, stabil parayı değerlendirmek.

Peki ya kullanıcı elinde tuttuğu volatil kripto paradan vazgeçmek istemiyor ise ne yapacak?

O zaman kullanıcıya stabil para bulalım ve onu değerlendirelim. Nasıl? Hatırlarsanız, bundan üç bölüm önce DeFi’nin ilk büyük platformlarından MakerDAO’dan bahsetmiştik. Kullanıcıların Ether teminat gösterip, DAI kredi kullanabildiği bir merkeziyetsiz sistem. İşte Yearn burada benzer bir sistemi kullanıyor.

Delegated Vaults denen bu üründe kullanıcılar [Aave](https://www.coingecko.com/en/coins/aave) ya da [Link](https://www.coingecko.com/en/coins/chainlink) kripto parası koyup, sonrasında borç verme ve getiri çiftçiliğinden para kazanabiliyor. Nasıl oluyor bu? Sistem, kullanıcının koyduğu parayı teminat göstererek stabil para borç alıyor. Sonra bu stabil parayı yukarıdaki bahsettiğimiz yVault ürünlerine koyarak ekstra stabil para gelir kazanıyor. Kazandığı bu stabil para ile gidip orijinal para ne ise ondan satın alıp tekrar ürünün içine koyuyor. Böylece kullanıcı, sahip olduğu Aave ya da Link’in getirisinden \(ve riskinden\) feragat etmeden, ekstra getiri kazanma imkanına sahip oluyor.

Yalnız bu ürün diğer yVault ürünlerine göre daha riskli. Neden? Mevcut yVault risklerinin üzerinde bir de Delegated Vault ürününün getirisi eğer alınan borç için ödenen faizden az olursa, kullanıcının koyduğu paranın sistemde kilitli kalma riski var. Bu para ancak sistemdeki getiri ödenen faizden fazla olursa tekrar kullanıma açılıyor.

#### Diğer ürünler

Bunun yannda deneme anlamında pek çok yeni ürün çıkarma çabaları da sürüyor Yearn’da.. Malum, açık kaynaklı “lego” gibi bir sistem DeFi.. Bu dünyadaki ürünler aynı dili konuştukları için yeni ürün çıkarmak yıllar, aylar değil, haftalar alıyor.

Alın örneğin [yInsure](https://yinsure.finance/) ürününü.  Bu kısmın en son bölümünde detaylı olarak bahsedeceğimiz DeFi’nin en büyük sigortacısı olan [Nexus Mutual](https://nexusmutual.io/) üzerinden aparılan bir sigortacılık ürünü. Bir diğer adı da [Cover](https://yinsure.finance/). Nexus Mutual, üyelerinden KYC \(Know-Your-Customer yani Müşterini Tanı\) prosedürü isterken, yinsure, benzer sistemi DeFi’nin KYC’den uzak kendi dünyası içinde kullanıcılarına sunuyor.

Bunun dışında henüz ArGe aşamasında olan, şu anki mevcut DeFi sistemi içinde yaşanan aksaklıkların önüne geçip kullanıcıya daha sorunsuz bir deney sunmaya çalışan birçok ürüne sahip Yearn. Bunların ne zaman ve ne kadar yaygınlaşacağını hep birlikte göreceğiz.

Kullanımda olan tüm Yearn ürünleri ile ilgili yatırılmış ya da yatırıma yönlendirilmiş para, günlük/haftalık/aylık kazançları topluca görebileceğiniz [bir bilgi sayfası da mevcut](https://stats.finance/yearn).

Şimdi de gelin Yearn protokolünün tokeni YFI ile birlikte platformun risklerini değerlendirelim.

### Ve YFI

Daha önce de birkaç kez yazdığımız gibi, merkeziyetsizlik uzun ince bir yol. Bu alanda kurulmuş pek çok girişim gibi Yearn protokolü de merkezilikten merkeziyetsizliğe benzer bir yol izledi. Başlangıçta yazılımcı [Andre Cronje](https://twitter.com/AndreCronjeTech)‘den oluşan “tek kişilik bir ordu” tarafından kurulan Yearn zamanla daha geniş bir topluluk haline geldi.

|  |
| :--- |
| _Image by_ [_Sarah Labbat_](https://pixabay.com/users/xoco-89138/) _from_ [_Pixabay_](https://pixabay.com/) |

Merkeziyetsizleştirme vizyonundaki adımlara baktığımızda, yol genelde gücün kullanıcılara verilmesi ve kodların açık hale getirilmesi şeklinde başlıyor. Bunun hemen arkasından sıra yazılım/geliştirme faaliyetlerini topluluğa bırakmaya geliyor. Son olarak platformun yönetiminin de merkeziyetsizleştirilmesi ile vizyon tamamlanıyor.

Bu süreci planlamak kolay ancak gerçekleştirmek zor ve meşakkatli. Özellikle son adım. DeFi alanında bu son adımı gerçekleştirmeye yönelik keskin hamle 2020 yazında yönetimi tokenlaştırma oldu. 

Yearn ekibi de, kendi merkeziyetsizleştirme sürecinde benzer bir süreç yaşadı. Ekip, yeni ürünleri tabiri caiz ise ‘çılgınlar gibi’ ardı ardına piyasaya sürerken, Temmuz ayı ortasında bir gün ansızın [YFI token](https://www.coingecko.com/en/coins/yearn-finance) adında bir yönetim tokeni çıkarttı. Bu tokenin özelliği kurucu ortaklara herhangi bir pay verilmeden, tamamının kullanıcılara dağıtılmış olması. Bu arada sadece 30.000 adet var bu tokenlardan \(Ocak 2021’de mevcut YFI sahiplerinin oylaması sonucu 6,666 adet token daha basmaya [karar verdiler](https://cryptobriefing.com/yearn-mints-yfi-worth-200-million/). Basılan bu tokenların üçte biri geliştiricilere ödül olarak verilecek, kalanı ise Yearn hazinesinde tutulacak\). 

Temel olarak Yearn protokolünün yönetimini merkeziyetsiz hale getirmek için tasarlanmış olan YFI tokenları sahiplerine para da kazandırıyor. [Bir önceki yazımızda](https://turansert.com/genel/2020/11/10/Defida-merkeziyetsiz-yonetim-platform-yearn-finance.html) bahsettiğimiz yVault ürünlerinden alınan toplam komisyonların \(kârdan %5 ve kullanıcının parasını geri çekmek istemesi durumda uygulanan %0.5 cezanın toplamı bunlar\) onda biri ürünü yaratan ve yöneten ekibe giderken, kalanı Yearn hazinesine kalıyor. Hazinede kalan bu para daha sonra oy kullanma yoluyla yönetime katılan YFI token sahiplerine dağıtılıyor.

Gerek kurucu ortaklara herhangi bir pay verilmemesi, gerekse yVault ürünlerinden alınan komisyonların geliştirici ekip ve kullanıcılara dağıtılması merkeziyetsizlik açısından önemli noktalar. Neden?

Öncelikle diğer DeFi projelerinde gördüğümüz kurucu ekibe %20-30 oranında pay verilmesi, kalan tokenları satın alan kişilerde tüm işi bu kurucu ekip yapacakmış gibi bir izlenim yaratıyor. Yearn platformunda ise, kurucu ekip baştan herhangi bir pay almadığı için sistemi yürütmek ve büyütmekte YIF token sahiplerine de sorumluluk düşüyor. Onların da böyle bir sorumluluk almak için teşvik edilmeleri gerek. İşte bu nedenlerle, yeni çıkan ürünlerde geliştiricilerin yaratılan komisyonların onda birini alması, kalan komisyonun ise oylamalara katılma karşılığı YIF sahiplerine verilmesi sistemin gelecekte de düzgün bir şekilde işlemesi için kritik.

YFI token sahiplerinin oylamaları sonucu çıkan kararları 9 kişinin sahip olduğu bir çoklu-imza cüzdanı hayata geçiriyor. Kripto dünyasında bilinen 9 oyuncunun her birinin bir imza yetkisine sahip olduğu bu cüzdanda işlem yapmak için 6 üyenin oyu gerekiyor. Merkeziyetsiz mi? Tam olarak değil, ama hiç yoktan iyidir.

Özet olarak, **YIF tokeni, hem token sahiplerine oylamalara katılma karşılığı gelir sağlıyor, hem de yazılımcılara geliştirdikleri ürünlerin yarattığı komisyonlardan pay veriyor. Bu da bireylerden bağımsız uzun vadeli sürdürülebilir bir platform yaratılmasında kritik bir önem taşıyor.**

#### Riskler neler?

_**Platform, platform üzerine olunca Akıllı Kontrat riski artıyor…**_

Öncelikle, Yearn ürünlerinin her birinin birer akıllı kontrat olduğunu belirtelim. Ve her bir ürünün başka başka DeFi platformları üzerinden getiri sağlamaya çalıştığını da ekleyelim. Dolayısıyla, kullanıcı yalnızca bu ürünlerin değil aynı zamanda bu ürünlerin üzerinde çalıştığı DeFi platformlarının riskini almak zorunda.

Üstelik bir değil birden fazla platform riski var. Örneğin, [Delegated yVault](https://yearn.finance/vaults) ürününde, i\) kullanıcı elinde tuttuğu kripto para \(örneğin [Link](https://www.coingecko.com/en/coins/chainlink)\), ii\) o paranın emanet verildiği platform \(örneğin [Aave](https://app.aave.com/home)\), iii\) karşılığında borç alınan para \(mesela [USDC](https://www.coingecko.com/en/coins/usd-coin)\), iv\) bu paranın değerlendirildiği platform \(örneğin [Curve](https://www.curve.fi/)\) ve son olarak da tüm bu sistemi yöneten Yearn akıllı kontratının riskini almak zorunda. Üzerine bir de tüm sistemi yöneten Controller denen strateji yürütücünün manuel işlem yapma riskini.

|  |
| :--- |
| _Image by_ [_Gerd Altmann_](https://pixabay.com/users/geralt-9301/) _from_ [_Pixabay_](https://pixabay.com/) |

Açıkcası bu alanda kullanıcıyı ferahlatacak mekanizmalar çok az ve yavaş gelişiyorlar. Bunlardan bir tanesi, kod anlamında yapılan denetimler. Pek çok proje çok hızlı ilerlediği için bu denetimleri yaptırmaz iken, kendisi eski bir denetim görevlisi olduğu için Andre’nin bu konuda hassasiyet gösterdiğini görüyoruz. [Yeterli mi](https://github.com/iearn-finance/yearn-audits)? Hayır.

Andre, hemen hemen her ortamda ürünlerinin yüksek risk içerdiğini söylüyor. Twitter profilinde “I test in prod” yazıyor, Türkçe meali “Ben ürünü çıkartırken test ederim, hatalar çıkabilir, dikkat edin”. Dolayısıyla konu hakkında tecrübesi az olanların, en azından başlangıç aşamasında Yearn ürünlerinden uzak durmasında fayda olabilir.

_**Platform ne kadar Andre’ye bağlı?**_

Andre çok sıkı bir programcı. Üniversite eğitimi hukuk, ancak Yearn öncesinde [CryptoBriefing](https://cryptobriefing.com/) sitesi için değişik blokzincirleri analiz ediyor \(bu arada kripto alanının en önde gelen şahsiyetlerinden Akıllı Kontratların mucidi [Nick Szabo](https://twitter.com/NickSzabo4)‘nun da [hukuk eğitimi almış olması](https://en.wikipedia.org/wiki/Nick_Szabo) ilginç bir detay\). Oldukça zeki ve kuvvetli bir programcı olmasının yanında gelgitleri olan biri: Kurduğu programı bir süreliğine bıraktı, hem de [bir](https://cointelegraph.com/news/one-man-defi-developer-quits-citing-hostile-community) değil [iki](https://www.coindesk.com/yearn-finances-creator-says-hes-quit-defi-but-project-has-bench-strength) kez. Verdiği kimi sözleri tutmadığı iddia edildi. Hatta bununla ilgili [Güney Afrika’da açılmış davalar olduğu söyleniyor](https://unchainedpodcast.com/why-bitcoin-now-meltem-demirors-and-lyn-alden-on-the-perfect-conditions-for-bitcoin/).

Andre hakkında çıkan söylentileri “meyveli ağacı taşlarlar” olarak mı “ateş olmayan yerden duman çıkmaz” olarak mı değerlendirmeli o kullanıcıya kalmış.

Zira, asıl önemli olan projenin nasıl bir topluluğa sahip olduğu. Kişisel olarak çok sevdiğim Naval Ravikant’ın geçtiğimiz günlerde yazdığı şu tweeti hatırlatayım size: “[Bir ürünün sürdürülebilmesi için bir şirket gerektiği gibi, bir protokolün devam etmesi için de bir topluluk gerekir](https://twitter.com/naval/status/1325531942431813632?s=20) "

Sonuçta Yearn tarafından ortaya çıkarılan bütün ürünler açık kod. İsteyen istediği gibi içine girip bakabilir. Klasik dünyada ise o koca koca şirketlerin içinde de kim bilir neler dönüyor? “Kol kırılır yen içinde kalır” hesabı bu olaylar dış dünyaya yansıtılmıyor. Hangisi daha şeffaf ve güvenilir?

Bir sistemin sürdürülebilirliğine bakarken belli sorular var cevaplanması gereken: Topluluk ne kadar geniş, ne kadar aktif, kurucunun topluluk içindeki payı ne? Her ne kadar Andre, Yearn protokolü içinde lider ve kritik bir role sahip olsa da, ekip onunla sınırlı değil. Örneğin DeFi dünyasının en eski ve büyük oyuncularından [MakerDAO](https://makerdao.com/en/)‘nun ileri gelen yazılımcılarından [Mariano Conti](https://twitter.com/nanexcool) geçtiğimiz aylarda Yearn ekibine katıldı. Bunun yanında topluluğun Discord kanalının 8,200, Telegram kanalının ise 13,200 üyesi var.

Keza bir önceki bölümde bahsettiğimiz YIF tokeninin ana amacı, protokolü kişilerden bağımsız topluluk tarafından sürdürülebilir hale getirmek.

Dolayısıyla kurucusu Andre’nin gelgitlerinden bağımsız olarak Yearn protokolü, takipçi sayısı ve kullanıcısı geniş bir topluluk olarak gelecekte de DeFi’nin önemli platformlarından biri olmaya aday.

#### Neden popüler oldu Yearn ürünleri?

Öncelikle yukarıda da belirttiğimiz gibi bu tip ürünlere piyasada gerçekten ihtiyaç var. Yearn sloganını “DeFi, simplified” \(Basitleştirilmiş Merkeziyetsiz Finans\) olarak belirlemiş.

DeFi platformlarını kullanmak, ileri seviyede teknik ve finans bilmek gerektirebiliyor. Geniş kitlelerden böyle bir bilgi birikimi beklemek haksızlık. Yapılması gereken ürünleri anlaşılır hale getirmek. Yearn platformu, daha kırk fırın ekmek yemesi gerekse de, bu yönde atılmış olumlu bir adım.

Bunun ötesinde piyasaya her gün yeni bir ürün çıkıyor. Yearn platformu, kullanıcıları farklı ürünlerin nasıl çalıştığını anlama zahmetinden kurtarıyor.

Peki Yearn protokol en kârlı stratejileri mi uyguluyor? Hayır. Daha önce de belirttiğimiz gibi, **Yearn’ın amacı riski minimize etmek**. Tek tek yeni girişimleri incelemeyi ve daha fazla risk almayı göze alan kullanıcılar kendi başlarına daha kârlı stratejiler çizebilirler.

Bunun yanında, özellikle yVault gibi ürünlerde, kripto para teminat göstererek kredi alıp, sonra bu krediyi farklı stabil paralarda değerlendirme stratejisi sürekli takip istiyor. Zira teminat değeri belli ürünün altına düşerse teminat yanabiliyor. yVault bu anlamda kullanıcıyı böyle bir dertten kurtarıyor.

Yukarıda bahsettiğimiz özellikler kullanıcıların ilgisini çekti. Ancak bu, tek başına Yearn üzerinde bir milyar ABD Doları para toplanmasına yeterli değil. Baksanıza bu yaz yaşadıklarına:

|  |
| :--- |
| _2020 yılı içinde Yearn platformuna kilitlenen para miktarı. Kaynak:_ [_DeFi Pulse_](https://defipulse.com/yearn.finance) |

Yearn asıl büyümesini, DeFi alanında yeni ortaya çıkan yönetim tokenlarının ilk başta çok hızlı değer kazanmaları sayesinde yaşadı. Bu gelişme, Yearn ürünlerinin de benzer şekilde çok iyi getiriler sağlıyor gibi görünmesine neden oldu. ABD Doları bazında üç haneli rakamlara varan getiriler, insanların gözlerini kamaştırdı. Büyük miktarlarda “balina” olarak adlandırılan yatırımcı paraları bu alana ve Yearn platformuna yığıldı.

#### Sonra?

Sonra “deniz tükendi”. Yönetim tokenlarındaki artışların getirdiği üç haneli rakamlar tek haneli rakamlara doğru inmeye başladı. Aslında üç haneli rakamlar yanıltıcı idi. Neden?

Çünkü gösterilen getiri, aylık getirinin bileşik hesaba göre yıllığa çevrilmesi idi. Açıkcası bu da tek gösterim yolu, zira geçmişe ait veri yok elde. Ama bu yine de yanıltıcı olduğu gerçeğini değiştirmiyor. Örneğin, aylık %5.94 getirili bir ürün her ay aynı şekilde kazandırmaya devam ederse yılda %100 getirir. Soru tabii ki her ay aynı getiriyi getirebilir mi?

Şunu söyleyelim: Yearn ürünleri hâlâ ortada ve getirileri eskisi kadar yüksek olmasa da hâlâ makul rakamlarda. Risk yönetimi açısından yukarıdaki gibi onlarca risk saysak da bu riskler genelde teknik alanda \(kod hatası benzeri\). Finansal olarak ise gerek Earn gerekse yVault prensip olarak kullanıcıya ellerinde tuttukları kripto paranın üzerine “risksiz getiri” sağlama mantığına göre çalışıyor. Nasıl yapıyorlar bunu? Kullanıcının kripto parasını teminat verdiklerinde, borç olarak stabil para alıp bu stabil parayı yatırım araçlarında değerlendirdikleri için. Yani, **teminat volatil \(iniş-çıkışlı\), ama hem yatırım yapılan hem de bu yatırım için kullanılan kredi tam tersi olarak sıfıra yakın volatileye sahip.**

Öte yandan, sistemin kurucusu Andre Cronje ile ilgili çıkan haberler de kimi kullanıcıları sistemden soğutmuş olabilir. Örneğin, Andre’nin attığı birkaç esrarengiz tweet sonrası, kullanıcılar daha tanıtımı bile yapılmamış bir ürün için, “yüksek kazanç” hevesiyle bir ETH hesabına tam 15 milyon ABD Dolar’a yakın para yatırdılar. Sonrasında bir hacker çıkıp bu hesaptaki paralara el koydu. [Ortalık ayağa kalktı](https://www.coindesk.com/eminence-exploit-defi-compensated). Hacker insaflı çıkıp paranın 8 milyonluk kısmını geri gönderdi de insanlar yatırdıklarının yarısını geri aldılar. Şahsen, burada Andre’yi haklı bulduğumu söylemeliyim. Ne işe yaradığını ve hazır olup olmadığını bilmediğiniz bir ürüne, üstelik denetimden bile geçmemişken yatırım yapıyorsanız, paranızı kaybetme riskiniz olduğunu bilmeniz gerekir. Paranız yanınca Andre’den medet umuyorsanız, o zaman DeFi ile ilgili bildiklerinizi tekrar gözden geçirmenizi tavsiye ederim.

#### Gelecekte kullanıcıları neler bekliyor?

Yearn, ilk ürünlerinde zarar etme riskini minimize eden stratejiler üzerine yoğunlaşmış idi. Bunun yapmanın yolu olarak da stabil paraları seçmişti. Görünen bundan sonra daha volatil kripto paraları kullanarak daha kârlı stratejiler yürütmeye çalışacak. Örneğin, vadeli piyasaları kullanarak, ETH üzerindeki düşüş riskini yok edecek opsiyonlar satın alacak. Ancak bu opsiyonları satın almanın doğa olarak bir maliyeti var. Bu nedenle, bu stratejiyi uygularken hedefi, ETH’yi yatırarak kazanacağı getirinin opsiyon maliyetinden yüksek olmasını sağlamak olacak.

