# DeFi'nin temel özellikleri neler?

Bir önceki bölümde bahsettiğimiz yönetim tokenları DeFi'nin patlamasına yardımcı oldu olmasına ama asıl DeFi'yi büyüten temel özelliklere de bakmak gerek:

### DeFi emanet tutmaz <a id="defi-emanet-tutmaz"></a>

DeFi için en önemli özelliklerden biri, borsaların aksine emanet tutmaması \(İngilizce'de non-custodial\). Bu ne demek? Gerek fiziksel gerekse dijital dünyada, maddi varlıklarımızın çalınmaması ya da kopyalanmaması için biz kullanıcılara banka ve finans kuruluşları yardımcı olur. Varlıklarımızı bankaya koyduğumuzda onu bankaya emanet ederiz. \(Bu emanet alma sorumluluğu nedeniyle, kanun koyucular haklı olarak finans kurumlarının tepesinde\) Ama bankacılık sistemi \(belki de kendilerince haklı olarak\) zaman geçtikte ve rekabet arttıkça, tüketicileri elinde tutabilmek için çeşitli zoraki yöntemler kullanmaya başladı. Geri kalmış sistemlerden dolayı müşterinin karşısına çıkarttıkları zoraki kısıtlardan, teknoloji artık daha kolayına imkan verse de, bir türlü vazgeçmemekte. Örneğin paranızı bir bankadan öbürüne taşımak hâlâ masraflı. Hadi para transferi nispeten daha kolay ama yatırımlarınızı bir kurumdan öbürüne taşımak oldukça sorunlu bir süreç. Her bir aracı kurum için aynı evraklar, süreçler her seferinde tekrar tekrar yaşanmak zorunda.

DeFi da ise, eğer bir elektronik  cüzdanınız varsa hükümdar sizsiniz. Zira DeFi ürünlerin çoğunluğu emanet sistemi ile çalışmıyor. Yani sizin paranıza dokunmuyorlar - size kelimenin tam anlamı ile aracılık ediyorlar, o kadar. Herhangi bir DeFi ürünün sitesine girdiğinizde genelde sağ üst köşede görünen ‘cüzdan bağla’ butonuna basarak cüzdanınızı saniyeler içinde bağlayabilirsiniz. Sitede işlem yapıp çıktığınızda da artık o siteye bir daha girmek zorunda değilsiniz \(pek çok ürün için bu böyle, tabii ki paranızı bağladığınız daha ileri seviye için değişiklik gösteriyor ama o bile yine klasik sistemlere göre çok daha rahat\)..

### Kullanıcı istediği platformu özgürce kullanabilir <a id="kullan&#x131;c&#x131;-istedi&#x11F;i-platformu-&#xF6;zg&#xFC;rce-kullanabilir"></a>

Pazarın hızlı büyümesinin temel nedenlerinden biri kullanıcıya verdiği özgürlük. Nasıl bir özgürlük? İstediği zaman bir platformdan diğerine geçebilmek. Bu da DeFi’in temel ilkelerinden birinden geliyor - uyumluluk. Bu platformlar kendi aralarında kabul görmüş standartlar ile çalışıyor. Öncelikle altyapı olarak Ethereum kullanıyor. Token çıkarıyorlar ise ERC20 protokolü ile ETC türevi paralar şeklinde oluyor. Hemen hemen hepsi bütün bilinen kripto cüzdanlar ile bağlantı kurabiliyorlar.

### Farklı platformları bir arada kullanabilir <a id="farkl&#x131;-platformlar&#x131;-bir-arada-kullanabilir"></a>

Peki nasıl hergün yeni bir ürün çıkabiliyor? Farklı ürünler sunan platformların birbirlerinin ürünlerini kullandığını ya da karma ürünler çıkardığını görebiliyorsunuz. Karmaşık bir örnek olacak ama örneğin [yearn.finance](https://yearn.finance/) adlı portföy yöneticisi sisteme para koyduğunuzda, sistem paranızı alıp [MakerDAO](https://makerdao.com/en/) sistemine teminat göstererek [DAI](https://oasis.app/) kredi alıyor, aldığı DAI’yı stabil paraların alım satımında çok kullanılan [Curve](https://www.curve.fi/) isimli borsaya likidite olarak koyup yapılan işlemlerden komisyon kazanıyor. Gördüğünüz gibi, bu işlemde birbirinden farklı üç adet sistem uyum içinde çalışıyor.

İşte bu uyumluluk da başlangıçta hayal edemeyeceğiniz kadar farklı ürünlerin çıkmasına ve pazarda arbitraj imkanları doğmasına yol açıyor. Bu arbitrajları değerlendiren kimi ürünlerde de uçuk kazanç rakamları görebiliyorsunuz.

### Açık kaynak hızlı geliştirme demek <a id="a&#xE7;&#x131;k-kaynak-h&#x131;zl&#x131;-geli&#x15F;tirme-demek"></a>

DeFi platformların bu kadar uyumlu olabilmesinin bir başka nedeni, yine başlangıç felsefesi olan açık kaynağa dayanmaları. Bu ne demek? Sonuçta birer yazılım olan bu sistemlerin bütün kodlarının apaçık ortada olması demek. Bu aynı zamanda herhangi birinin bu kodu alıp o platformun aynısını saatler içinde yaratabilmesi de demek.

Çok tehlikeli değil mi bu? İşte değiştirmeniz gereken kafa yapılarından biri ile karşı karşıyasınız: Eskinin “lisanslı ürün satayım, telif alayım” günleri geride kaldı. Öyle olduğunuzda rekabette geri kalıyor, hantal yapılar haline geliyorsunuz. DeFi dünyasında artık açık kaynak ile başkalarının yaptığından faydalanıyor ama kendi yaptığınızı da başkalarına sunuyorsunuz. Bu nedenle hep uyanık kalmalı ve hep yenilikler yapmalısınız. 

Konuyu toplayacak olursak, bu platformlar açık kaynaklı olunca tabii klonları da hemen çıkıyor. Ve bu klonlar orijinallerinin üzerine birkaç farklı özellik daha ekleyerek çok cazip ürünler sunabiliyor. Buna en güzel örneğin 2020 yılının Ağustos ayının sonlarında yaşadık. Piyasanın en büyük merkeziyetsiz borsası olan [Uniswap](https://uniswap.org/) klonlandı. Buraya kadar bir sorun yok. Uniswap, basit bir algoritma üzerine çalışan, yıllardır bu alanda faaliyet gösteren ama likiditenin artması ile birlikte patlama yapan bir merkeziyetsiz kripto para borsası. Yapılan al-sat işlemlerinden kazandığı komisyonun \(şimdilik\) tamamını kendisine likidite koyan bireysel kullanıcılara ödül olarak veriyor. 27 Ağustos’ta çıkan [SushiSwap](https://sushiswap.org/), UniSwap’ı birebir klonladı. Bununla da yetinmedi; sisteminin kullananlara Uniswap gibi yapılan işlemlerden aldığı komisyonlar dışında kendi yönetim tokenini de verdi. Sonuç: SushiSwap’a kilitlenen para [üç günde 1.5 milyar doları buldu](https://www.coindesk.com/sushiswap-uniswap-launch).

