# Socket Methodları

Soket kullanımı için işe yarar methodlar:

## Sunucu Soketi Methodları (Server Socket Methods)
| Method     | Açıklama                                                                                                           |
|------------|--------------------------------------------------------------------------------------------------------------------|
| s.bind()   | Bu method, adresi (ana bilgisayar adı, bağlantı noktası numarası çiftini) sokete bağlar.                           |
| s.listen() | Bu method, TCP dinleyicisini kurar ve başlatır.                                                                    |
| s.accept() | Bu method, pasif olarak TCP istemci bağlantısını kabul eder ve bağlantı gelene kadar bekler (engelleme işlemidir). |

## İstemci Soketi Methodları (Client Socket Methods)
| Method      | Açıklama                                                                                                           |
|-------------|--------------------------------------------------------------------------------------------------------------------|
| s.connect() | Bu method, TCP sunucusu bağlantısını etkin olarak başlatır.                                                        |

## Genel Soket Methodları (General Socket Methods)
| Method               | Açıklama                          |
|----------------------|-----------------------------------|
| s.recv()             | Bu method, TCP mesajını alır.     |
| s.send()             | Bu method, TCP mesajını iletilir. |
| s.recvfrom()         | Bu method, UDP mesajını alır.     |
| s.sendto()           | Bu method, UDP mesajını iletir.   |
| s.close()            | Bu method, soketi kapatır.        |
| socket.gethostname() | Ana bilgisayar adını döndürür.    |
