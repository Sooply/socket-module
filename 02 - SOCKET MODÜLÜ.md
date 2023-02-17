# Socket Modülü

Soket oluşturmak için, genel sözdizimi (syntax) şöyle olan socket modülünde bulunan `socket.socket()` fonksiyonunu kullanmalısınız:

```s = socket.socket (socket_family, socket_type, protocol=0)```

Burada da parametlerin açıklamaları bulunuyor:
- **socket_family:** Soket aileleridir, önceki dosyada açıkladığımız gibi bu parametre ya `AF_UNIX` ya da `AF_INET`'tir.
- **socket_type:** Soket tipidir, önceki dosyada açıkladığımız gibi bu parametre ya `SOCK_STREAM` ya da `SOCK_DGRAM` olarak geçer.
- **protocol:** Bu parametre genellikle belirtilmez ve varsayılan olarak 0 olarak ayarlanır.

### Örnek kullanım

```python
s = socket.socket (socket.AF_INET, socket.SOCK_STREAM)```
