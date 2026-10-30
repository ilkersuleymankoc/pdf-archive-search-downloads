# PDF Archive Search — Kurulum dosyaları

Güncel sunucu güncellemesi ve Windows istemcisi. Gerçek kurucu kabulü tamamlandı; herkese açık doğrudan indirme bağlantıları aşağıdadır.

| Güncel paket | İndir |
| --- | --- |
| Sunucu güncellemesi 0.1.6.3 | [Archiv-Server-Update-0.1.6.3.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.3/Archiv-Server-Update-0.1.6.3.exe) |
| Windows istemcisi 0.1.7 | [Archiv-Client-Setup-0.1.7.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-client-0.1.7/Archiv-Client-Setup-0.1.7.exe) |
| Türkçe kurulum ve kullanım rehberi | [Archiv-Kurulum-0.1.6.3-Client-0.1.7.txt](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.3/Archiv-Kurulum-0.1.6.3-Client-0.1.7.txt) |

Mevcut HTTP/Web 0.1.0 veya fatura iş akışı 0.1.6.2 kurulumu için önce **sunucuda 0.1.6.3**, ardından **kullanıcı bilgisayarlarında Client 0.1.7** kurun. Çalışan uygulamayı kapatıp aynı kurulu klasöre yükseltin; önceki sürümü kaldırmayın. Önce SQL veritabanını, kalıcı yapılandırmayı ve orijinal PDF/Inbox dosyalarını yedekleyin. SQL/Windows parolaları yeniden istenmez; hesaplar, kaynaklar, izinler ve elle kaydedilmiş fatura alanları korunur.

Sunucu güncellemesi mevcut HTTP/Web arayüzünü de 0.1.7'ye yükseltir; HTTP bileşeninin kayıtlı sürümü 0.1.1 olur. Tarayıcı sayfasını yenileyin. HTTP/Web kurulu değilse bu paket yeni bir HTTP hizmeti oluşturmaz. **0.1.6.3 sonrasında eski R6, HTTP/Web 0.1.0 veya iş akışı kurucularını tekrar çalıştırmayın.**

Bu sürümde ayrı sütundaki **Belegdatum** tarihinin tanınması düzeltildi. Eski otomatik öneriler yeniden değerlendirilir; elle kaydedilmiş alanlar değiştirilmez. Fatura araması indekslenmiş PDF içeriğinde de arar; birden çok kelime aynı sayfada bulunmalıdır. Tablo satırları ve form alanları küçültüldü, PDF'ye daha fazla alan ayrıldı. Küçültme/geri açmada sayfa ve yakınlaştırma korunur; oturuma özel sınırlı RAM önbelleği tekrar aktarımı azaltır. Yetki denetimleri sürer; ilk açılışın süresi ağ ve belgeye bağlıdır.

Windows ve tarayıcı adresi aynıdır: `http://SUNUCUNUN-OZEL-IP-ADRESI:8080`; sonuna `/api` eklemeyin. HTTP şifrelenmez; yalnız güvenilir şirket ağı/VPN için kullanın. iPhone için Safari web yolu vardır; gerçek iPhone/Safari doğrulaması ve yerel iOS dağıtım paketi bu sürümde yoktur.

Yalnız eski sürümden veya sıfırdan kurulum için önkoşullar:

| Önceki paket | İndir |
| --- | --- |
| Yalnız yeni sunucu: temel kurulum 0.1.6 | [Archiv-Server-Setup-0.1.6.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-0.1.6/Archiv-Server-Setup-0.1.6.exe) |
| R6 henüz kurulmadıysa: 0.1.6.1 | [Archiv-Server-Update-0.1.6.1.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.1/Archiv-Server-Update-0.1.6.1.exe) |
| İş akışı 0.1.6.2 ve HTTP/Web erişimi | [Archiv-HTTP-Web-Setup-0.1.0.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-http-web-0.1.0/Archiv-HTTP-Web-Setup-0.1.0.exe) |

Sıfırdan sıra: **Server 0.1.6 → R6 → HTTP/Web 0.1.0 → Server Update 0.1.6.3 → Client 0.1.7**. Kurulu önkoşulları yeniden çalıştırmayın.

Doğrulama: **69 Flutter testi**, analiz, Windows/Web derlemeleri ve gerçek Windows PDF motoruyla yaşam döngüsü testi geçti. Son sunucu EXE kabulü: **110/110 ana kontrol, 69/69 fatura/OCR, 28/28 HTTP, 2/2 temizlik**; Client 0.1.6 → 0.1.7 yükseltme/kaldırma: **71/71 ve 1/1 temizlik**. Yerel küçük sentetik PDF aktarımı ilk istekte **930,862 ms**, bağlayıcı durmuşken önbellekten **4,434 ms**; hizmet otomatik toparlanması **6,02 saniye**. Şirket ağı/büyük belge süresi garantisi değildir. Genel istemci GUI'si, gerçek tarayıcı etkileşimleri ve iPhone/Safari incelemesi doğrulanmadı.

| Dosya | Bayt | SHA256 |
| --- | ---: | --- |
| Server Update 0.1.6.3 | 1145861 | `4E040DCB861D4A2ACB5B4D1E99C9E42D0CD02C2CB0C3C572AC2E13E25631A22D` |
| Client 0.1.7 | 36898723 | `26817A308FC2D4E39B5E702223E0B2C090DD0341146F4C06C40CE4E0F60DC7F7` |

[Sunucu SHA256 dosyası](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.3/Archiv-Server-Update-0.1.6.3.exe.sha256) · [Client SHA256 dosyası](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-client-0.1.7/Archiv-Client-Setup-0.1.7.exe.sha256)

Bu herkese açık depo yalnız kurucular, sağlama toplamları ve kullanım rehberi içindir. Kaynak proje özeldir. Paketler yerelde derlendi; bu çalışma için GitHub Actions başlatılmadı.
