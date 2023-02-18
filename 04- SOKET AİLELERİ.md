# Socket Address Family (Socket Adres Ailesi)

Bir socket() API üzerindeki adres ailesi parametresi (socket_family), soket API'lerinde kullanılacak adres yapısının formatını belirler.

Adres ailesi protokolleri, uygulama verilerinin bir uygulamadan diğerine (veya aynı sistem içinde bir işlemden diğerine) ağ aktarımını sağlar. Uygulama, ağ taşıma sağlayıcısını soketin protokol parametresinde belirtir.

- **AF_INET adres ailesi:** Bu adres ailesi, aynı sistem üzerinde veya farklı sistemler üzerinde çalışan işlemler arasında işlemler arası iletişimi sağlar.
- **AF_INET6 adres ailesi:** Bu adres ailesi, İnternet Protokolü sürüm 6 (IPv6) için destek sağlar. AF_INET6 adres ailesi, 128 bitlik (16 bayt) bir adres kullanır.
- **AF_UNIX adres ailesi:** Bu adres ailesi, soket API'lerini kullanan aynı sistemde süreçler arası iletişim sağlar. Adres aslında dosya sistemindeki bir girdiye giden yol adıdır.
- **AF_UNIX_CCSID adres ailesi:** AF_UNIX adres ailesiyle uyumludur ve aynı sınırlamalara sahiptir.
