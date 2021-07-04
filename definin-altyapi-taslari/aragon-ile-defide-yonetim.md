# Aragon ile DeFi'de yönetim

Bu bölümde gelin hep birlikte, merkeziyetsiz yönetim konusunda enteresan bir deneysel fikir olan [Aragon](https://aragon.org/)‘a göz atalım.

Şu aralar ağırlıklı token değeri bazlı spekülatif yanı konuşulsa da, DeFi projelerinin devrim olarak nitelendirilebilecek en heyecan verici taraflarından biri; merkeziyetsiz bir şekilde yönetiliyor olmaları. Aslına bakarsanız, merkeziyetsiz yönetim o kadar da kolay değil. Hatta nasıl yapılır, nasıl yönetilir tam bir fikir birliği de yok.

Aragon öncesinde, DeFi projelerinin pek çoğunun kendine model aldığı [DAO \(Decentralized Autonomous Organization\)](https://en.wikipedia.org/wiki/Decentralized_autonomous_organization) yani Merkeziyetsiz Otonom Organizasyon yapısı ne demek ona bakalım:

### DAO ne demek?

DAO; dijital dünyada kurulu, işleyiş ve kanunları kod olarak yazılı, otonom ve şeffaf olarak çalışan yapılara verilen ad. Yaptıkları işlemlerin güvenilir olması için elbette blokzincir altyapılarını kullanıyorlar. Sistem yalnızca hissedarları tarafından kontrol edilebiliyor. Fiziki dünyada bir aktiviteleri \(ya da ofisleri\) olmadığı için herhangi bir devletin denetimi altında sayılmıyorlar. Hukuki yapıları da o anlamda çok net olarak belirlenmiş değil.

DAO’ların ilk duyulması aslında o kadar da pozitif olmadı. Zira, Ethereum üzerine kurulu ilk yapı olan [The DAO](https://en.wikipedia.org/wiki/The_DAO_%28organization%29), 2016 yılında 150 milyon ABD Doları para topladıktan kısa bir süre sonra hacklendi ve emanetinde duran 50 milyon ABD Doları karşılığı ETH çalındı. Ethereum içinde çıkan derin tartışmalar sonucu, bir çatallama \(hard fork\) yapılarak bu rakam blokzincir içinde geri çevrildi. Parasını geri alanlar için güzel; ancak blokzincirin güvenirliği \(geri çevrilemez\) özelliğini yerle bir etmesi bakımından Ethereum için kara bir leke olarak tarih sayfalarına yazıldı.

O zamandan sonra bir süre pek sesi çıkmayan DAO’lar, yeni DeFi projelerle birlikte tekrar spot ışıkları altında boy göstermeye başladılar.

### Nedir Aragon?

Efendim, Aragon özünde merkeziyetsiz olarak yönetilmek isteyen kişilere, bu tip bir yönetim için gerekli olan DAO yapısını sağlayan Ethereum üzerine kurulu bir platform. Tabii ki dijital dünyada. Fiziksel dünyadan bir örnek olarak kooperatifleri düşünebilirsiniz. Kişilerin bir proje amaçlı olarak bir araya geldikleri ve proje bitiminde lağvettikleri birlikler gibi.

![](../.gitbook/assets/030605-aragon_ile_defide_yonetim-aragon-defi.jpg)

_Photo by_ [_Sam Beasley_](https://unsplash.com/@sam_beasley) _on Unsplash_

“Ne gerek var?” diye sorabilirsiniz. Gereği şu: Dijital dünyada da olsanız, kişilerin oluşturduğu toplulukları yönetmek için kurallara ihtiyacınız var. Benzer şekilde sorunlar çıktığında bunları çözmek için de belli mekanizmalara ihtiyaç duyuyorsunuz. Ancak katılımcıların hepsinin bu kuralları, artılarını eksilerini bilme imkanı yok, hatta buna gerek de yok.

İşte Aragon, bu anlamda bir araya gelen gruplara kendi sistemlerini yönetmek için daha önce denenmiş hazır ve esnek şablonlar sunuyor. Kullanıcı dostu, Akıllı Kontratlar ile çalışan ve kişilerin ihtiyaçlarına göre şekillendirebildikleri platformlar.

Malum, dijital dünyanın fiziksel dünyaya göre avantajı işlerinizi daha hızlı, basit, zahmetsiz ve ucuza çözmeniz. Aragon da bu DAO’ları aylık 10-20 ABD Doları’na kullanabileceğiniz bir hizmet sunuyor. Bir nevi, zamanında her tür web projesi için bir yazılımcı ile çalışılmak zorunda iken sonrasında Wordpress’in ortaya çıkışıyla blog yazma ya da web sitesi kurmanın çocuk oyuncağı haline gelmesi gibi.

### Nasıl çalışıyor?

Aragon üzerine kurulu olan DAO’larda olması gereken üç temel özellik var; üyelik ve oylama hakkı için bir '**token'**, grubun sahip olduğu varlıkları korumak için bir '**cüzdan'** ve her tür oylama sonucu oluşan kararı ve işlemleri takip etmek için bir '**blokzincir'**.

İşte bu üç temel özelliği ihtiyacınıza göre şekillendirerek gruplar kurabilir, projeler ortaya çıkarabilirsiniz. Haziran 2021’e kadar bu şekilde [Aragon üzerinde kurulmuş 1,700’ün üzerinde DAO](https://poweredby.aragon.org/) var ve bu yapılar yaklaşık 900 Milyon ABD Dolarından fazla bir dijital varlığı ellerinde tutuyorlar.

Tabii projeleri kurmak nispeten kolay. Asıl büyük sorun genelde üyeler arasında anlaşmazlıklar çıktığında oluyor. Fiziksel dünyada sorunlar çözülmez ise mahkemeye gidiyorsunuz. Burada? Aragon’un bu tip sorunlar için de ilginç bir çözümü var:

Başta söyledik, blokzincirlerde kanunlar yazılımcılar tarafından kod yazılarak sisteme konuyor. Ancak her tür senaryoyu koda çevirmek mümkün olmayabiliyor. İşte o zaman Aragon, katılımcılara opsiyonel bir Subjektif Akıllı Kontrat sunuyor. Baştan böyle bir kontratı kabul etmeleri durumunda katılımcılar bir miktar kriptoparayı sisteme teminat olarak kilitliyorlar. Sonrasında, bir anlaşmazlık olduğunda ya konuyu kendi aralarında hallediyor ya da “sanal mahkeme”ye gidebiliyorlar .\(Yalnız sanal mahkemeye gider ve kaybederler ise teminatları yanıyor. Bunu; sorunları, mahkemeye gitmeden kendi aralarında çözsünler diye yapmışlar\).

Peki sanal mahkeme nasıl çalışıyor? Yargıyı kimler sağlıyor? Sisteme özgü Aragon Network Juror \(ANJ\) tokene sahip olan üyeler arasından sanal mahkemeye rastgele bir seçim yapılıyor. Seçilen üyeler önlerine gelen vakayı inceliyor ve oyluyorlar. Çoğunluğun verdiği karar kazanıyor. \(Yalnız burada da ilginç bir durum var; eğer çoğunluk tarafında değilseniz teminat olarak verdiğiniz para yanıyor\).

Sistemin nasıl çalıştığı Aragon yatırımcılarından Joel Monegro’nun [şu yazısından](https://www.placeholder.vc/blog/2020/5/7/aragon-daos) ya da yargı sisteminin detaylarını [Aragon blog sayfasından](https://blog.aragon.one/aragon-agreements/) inceleyebilirsiniz.

### Aragon üzerine son birkaç söz

Decentralized Autonomus Organization yani DAO’lar DeFi alanına ilgi duyanların yakından anlamaları gereken yapılar. Zira fiziki dünyada hepimizin alıştığı anonim şirket, limited şirket gibi oluşumlar devletin koyduğu kanunlara tabi, otoriteler tarafından kontrol edilen ve hissedar ya da çalışan haklarının bir nevi korunduğu yerler. Dijital dünyada ise devlet kontrolünün olmadığı bir ortamda, bu tip yapılar katılımcılar için pratiklik yanında sorumluluk da getiriyor. Aragon benzeri projeler bu anlamda bize bu tip yapıların nasıl işleyebileceği konusunda farklı alternatifler sunuyor, bir nevi yol gösteriyor.

Hep söylediğimiz gibi son on yıldır dijital dünyada hepimizin gözleri önünde bir devrim yaşanıyor, DAO’lar da bu devrimin önemli yapı taşlarından biri. Gelecek bu anlamda çok heyecanlı olacak, hep birlikte yaşayarak göreceğiz.

