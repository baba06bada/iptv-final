# BABA ÖZKAN PLAYER

LG WebOS 2.2.3 akıllı TV'ler için IPTV Smarters Pro tarzı medya oynatıcı.

## Özellikler

- **Canlı TV**, **VOD (Film)** ve **Diziler** desteği
- Xtream Codes API ile panel bağlantısı
- HLS.js ile .m3u8 akış oynatma
- Magic Remote (pointer + yön tuşları) desteği
- Netflix tarzı gradient OSD
- Otomatik sonraki bölüm (dizilerde)
- Devam izleme (resume)
- Son eklenenler
- Global arama
- Kanal logoları
- Sıralama seçenekleri (A-Z, Yıl, Puan)
- Reklam atlama (+60sn)
- Hız kontrolü (0.5x - 4x)
- En-boy oranı değiştirme
- Bağlantı hız testi
- PIN kilidi
- Pano özelleştirme
- Sanal kaydırma (1000+ içerik için performans)
- Otomatik yeniden bağlanma (canlı yayın kopmalarında)

## Kullanım

1. `cc.html` dosyasını bir web sunucusuna yükle (Apache, Nginx, veya Node.js)
2. LG TV'nin tarayıcısından dosyaya eriş
3. Ayarlar'dan Xtream Codes panel bilgilerini gir (URL, kullanıcı adı, şifre)
4. İzlemeye başla

### Node.js sunucu (isteğe bağlı)
```
node server.js
```
Ardından `http://SUNUCU_IP:8080/cc.html`

## LG TV'de Erişim

TV'de tarayıcı aç:
```
http://192.168.1.___:8080/cc.html
```

## Notlar

- WebOS 2.2.3 (Chrome 34) için optimize edilmiştir
- ES6+ sentaksı kullanılmaz
- Flex `gap`, `display: grid`, `backdrop-filter` kullanılmaz
- Tüm ekranlarda Magic Remote için tıklanabilir geri butonu bulunur

## Dosyalar

- `cc.html` - Ana oynatıcı
- `server.js` - Basit HTTP sunucu
- `LGTV.html` - Yedek oynatıcı
