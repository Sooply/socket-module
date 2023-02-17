# Soket Temelleri

Ağ soketi, bir bilgisayar ağı boyunca gerçekleşen bir işlem-işlem iletişiminin uç noktasıdır. Soketler bir işlem içinde, aynı makinedeki farklı işlemler arasında veya farklı kıtalardaki işlemler arasında iletişim kurabilirler. Günümüzde bilgisayarlar arasındaki çoğu iletişim internet protokolüne dayandığından, çoğu ağ soketi internet soketleridir. Makineler arasında bir bağlantı kurmak için, Python programları socket modülünü içe aktarır, bir soket nesnesi oluşturur ve nesnenin yöntemlerini çağırarak bağlantıları kurar ve veri gönderip alır. Soketler, çift yönlü iletişim kanalının uç noktalarıdır.

# Python'da Soket

Python, ağ hizmetlerine iki seviyede erişim sağlar. _Düşük seviyede_, temel soket desteğine erişebilirsiniz. Bu, bağlantı odaklı ve bağlantısız protokoller için hem istemcileri hem de sunucuları uygulamanıza olanak tanır. Python ayrıca FTP, HTTP, SMTP gibi belirli uygulama düzeyi ağ protokollerine daha _yüksek seviyede_ erişim sağlayan kütüphanelere de sahiptir. Soketler, UNIX alan soketleri, TCP, UDP vb. gibi birçok farklı kanal türünde uygulanabilir. Soket kütüphanesi, ortak taşımacılık işlemleri için özel sınıflar sağlar ve geri kalan işlemler için genel bir arabirim sağlar.

## Socket için sözlük

| Terim         | Açıklama      |
| ------------- |:-------------:| 
| **domain**    | Taşıma mekanizması olarak kullanılacak protokol ailesi. Bu değerler, **AF_INET**, **PF_INET**, **PF_UNIX**, **PF_X25** vb. gibi sabitlerdir. | 
| **type**    | İki uç nokta arasındaki iletişim türü, genellikle bağlantı odaklı protokoller için `SOCK_STREAM` ve bağlantısız protokoller için `SOCK_DGRAM`'dir. | 
| **protocol**    | Genellikle değeri sıfırdır. Bu, bir etki alanı ve tür içindeki bir protokolün bir varyantını tanımlamak için kullanılabilir. | 
| **hostname**    | Bir ağ arabiriminin tanımlayıcısı: • Bir host adı, noktalı dörtlü bir adres veya iki noktalı (ve belki de bir noktalı) IPV6 adresi olabilen bir dizedir. • "**<broadcast>**" karakter dizisi, `INADDR_BROADCAST` adresini belirler. • Uzunluğu sıfır olan bir dize, `INADDR_ANY`'yi belirtir, veya ana bilgisayar bayt sırasında ikili adres olarak yorumlanan bir tamsayı olabilir. | 
| **port**    | Her sunucu, bir veya daha fazla bağlantı noktasını arayan istemcileri dinler. Bir bağlantı noktası, Fixnum bağlantı noktası numarası, bir bağlantı noktası numarası içeren bir dize veya bir hizmetin adı olabilir. | 
