# DeFi dünyasında neler var?

DeFi yani merkeziyetsiz finans henüz yeni bir oluşum. 2017 yılında gerçekleşen IPO'lar sırasında ortaya atılan fikirlerin sonraki iki yıl boyunca deneme-yanılma yöntemiyle denenmesi sonucu 2020 yılının yaz aylarından itibaren çıkışa geçmiş bir hareket. 

DeFi alanında kullacılara sunulan ilk ürünlere baktığımızda bunların pek çoğunun aslında şu anda klasik finans dediğimiz mevcut finans piyasası aktörlerinin sunduğu ürünlere benzerlik gösterdiğini görüyoruz. Bunun temel nedeninin, öncelikle kullanıcının aşina olduğu ürünlere yakınlık göstermesi olarak düşünebiliriz. 

Ancak bir önceki kısımda bahsettiğimiz birlikte çalışılabilirlik, açık kaynak kullanımı gibi temel özelikleri nedeniyle DeFi'nin klasik finansın sunduğu hizmetlerin çok daha ötesini sunabileceğini söylemek çok da kehanet sayılmaz. 

### Klasik finans ile DeFi'nin temel farkı

Yukarıda bahsettiğimiz özellikler nedeniyle DeFi'nin çalışma prensiplerinin klasik finanstan temelde farklılık gösterdiğini söyleyebiliriz. Neler bunlar, kısaca değinelim: 

Klasik finans dünyasının aktörleri geçmişten gelen 'korumacı' zihniyetin devamı olarak 'silo' halinde çalışırlar.  Kullanıcı, varlığını bir finans kurumuna emanet eder ve sadece o finans kurumunun sunduğu ürünleri kullanabilir. Başka kurumlar ait ürünleri kullanmak isterse, o başka kurumda hesap açması ve oraya da ayrıca varlığını yatırması gerekir. 

Finans kurumu, aylarca yıllarca çalışarak, müşterileri için ürünler hazırlar ve onlara sunar. Bu ürünlerin gelişmesine ait telif haklarını sıkı sıkıya kayıt ettirir ve başkalarının kullanımı halinde mahkemelerde hakkını arar.  

DeFi'de ise bu durum kökten değişiyor. Öncelikle kullanıcı varlığını hizmet sağlayıcıya emanet etmez. Varlık kullanıcının elektronik cüzdanında durur \(Son bölümümüzde bu konuya detaylıca bakacağız\). Kullanıcı hizmet sağlayıcı ile çalışmak istediği anda cüzdanını bağlar, hizmeti kullanır sonra ilişkiyi keser. Üstelik, DeFi ürünleri birlikte çalışabildiği için, aldığı bir DeFi ürününü götürüp başka bir protokolde de kullanabilir. 

Bunun yanında açık kaynak sayesinde ürün geliştirme süreçleri DeFi için oldukça kısa. Bu dünyada, telif hakları gibi konular yok denecek kadar az. Zira, bırakın ürünlerin nasıl dizayn edildiğini, ürünün kaynak kodları yani onu oluşturan her parça isteyen herkesin görebileceği şekilde açık. 

### Dikey yapılanma yerine yatay yapılanma

Dolayısıyla, klasik finansın dikey yapılanma da diyebileceğimiz sistemine karşılık DeFi yatay bir yapılanma sağlar. Yani, sunulan hizmetler katman katman ayrılabilir. Her katmanda da birbiri ile yarışan servis sağlayıcılar bulunur. Servis sağlayıcılar diğer katmanlardaki ürünler ile birlikte çalışabildikleri için, kullanıcı her katmandan istediğini seçerek kendi risk/getiri profiline uygun kişiselleştirilmiş ürünler çıkarabilir. Bu alandaki yatırımcılardan Multicoin Capital, DeFi destesi olarak adlandırdığı aşağıdaki şemada DeFi ekosistemini gayet güzel bir şekilde anlatıyor:  

![DeFi Destesi \(DeFi Stack\) Kaynak: Multicoin Capital](../.gitbook/assets/defi_stack.jpg)

DeFi destesindeki altı parçayı en alt yani temel altyapıdan, en üst yani kullanıcıya dokunan şekilde sıralayıp, her bir katmandan birer cümle ile bahsetmekte fayda var: 

Bu arada hemen belirtelim, bu destedeki en alt üç parçaya, yani 'Para Birimleri', 'İşlem Katmanı' ve 'Bilgi Sağlayıcılar' parçalarına, bir sonraki kısım olan 'DeFi'nin Altyapı Taşları' kısmında, 'Temel DeFi Ürünleri' olarak adlandırabileceğimiz, kullanıcıların daha aşina olduğu DeFi protokollerine bu kısımda, en üstte bulunan 'Kaynak Sağlayıcılar' ve ' Cüzdanlar/Önyüzler' parçalarına ise en son bölüm olan 'DeFi Dünyasına Adım Atacaklar İçin Pratik Bilgiler' kısmında değiniyor olacağız. 

#### Para birimleri \(Unit of Value\):

İşin en temelinde para birimleri var. Neden? Ortada bir para birimi yani değer olmalı ki, kullanıcı varlığını saklayabilsin ve o varlık ile finansal işlem yapabilsin. DeFi'de kullanılan para birimleri, BTC, ETH gibi kıymeti kendinden menkul kriptoparalar olabildiği gibi, değeri ABD Doları gibi itibari paralara dayanan stabil para dediğimiz kripto paralar da olabiliyor. 

#### İşlem katmanı \(Transaction layer\): 

Kullanıcı kendine ait bir değeri olduktan sonra bu değeri saklayabileceği ve finansal işlemlerini gerçekleştirebileceği bir alan arar. İşte temel olarak blokzincirler burada DeFi'nin ihtiyacı olan altyapı hizmetini verirler. 

Bu kitapta genelde blokzincir olarak Ethereum'dan bahsedildiğini göreceksiniz.  Bunun temel nedenleri arasında, Ethereum'un Bitcoin sonra çıkmış en popüler blokzincir olması, kendisini bir akıllı kontrat platformu olarak sunması ve DeFi protokollerinin ağırlıklı bir çoğunluğuna ev sahipliği yapması geliyor. 

Teknolojinin her alanında olduğu gibi burada da Ethereum'un rakipleri var, ancak şu anda hemen hemen hepsi emekleme aşamasında. Gelecekte, bu rakiplerden bir ya da birkaçının Ethereum'a ciddi rakip olabileceğini de görebiliriz. 

Ethereum'un rakiplerinin ataklarına karşılık verdiği cevaplardan bir tanesi 2022 yılında görücüye çıkaracağı yeni versiyonu olacak. Ancak DeFi'nin patlaması ile birlikte Ethereum blokzincirine yoğun bir talep olduğu ve bunun işlem ücretlerinde ciddi bir yükselişe neden olduğu da bir gerçek. Bu nedenle özellikle Ethereum üzerine kurulu ikinci seviye çözümler, ağın üzerindeki yükü alması, belli hizmetlerin hem ucuz hem de hızlı bir şekilde gerçekleşebilmesi için kritik. 

#### Bilgi Sağlayıcılar 



#### Temel DeFi ürünleri



#### Kaynak Sağlayıcılar



#### Cüzdanlar/Önyüzler



