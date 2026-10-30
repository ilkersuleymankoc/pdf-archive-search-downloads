# PDF Archive Search — Kurulum dosyaları

Test edilmiş Windows kurucuları ve kurulum rehberi.

| Paket | İndir |
| --- | --- |
| Sunucuya HTTP/Web 0.1.0 ve gömülü iş akışı 0.1.6.2 | [Archiv-HTTP-Web-Setup-0.1.0.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-http-web-0.1.0/Archiv-HTTP-Web-Setup-0.1.0.exe) |
| Windows istemcisi 0.1.6 | [Archiv-Client-Setup-0.1.6.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-client-0.1.6/Archiv-Client-Setup-0.1.6.exe) |
| Önkoşul: sunucu güncellemesi 0.1.6.1 R6 | [Archiv-Server-Update-0.1.6.1.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.1/Archiv-Server-Update-0.1.6.1.exe) |
| Yalnız yeni sunucu için temel kurulum 0.1.6 | [Archiv-Server-Setup-0.1.6.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-0.1.6/Archiv-Server-Setup-0.1.6.exe) |

[Türkçe kurulum ve kullanım rehberi](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-http-web-0.1.0/Archiv-Kurulum-HTTP-Web-0.1.0-Client-0.1.6.txt)

Çalışan sunucuyu kaldırmayın. Önce SQL veritabanını, kalıcı yapılandırmayı ve orijinal PDF'leri/Inbox'ı yedekleyin. **R6 henüz uygulanmadıysa R6 → HTTP/Web 0.1.0 → Client 0.1.6** sırasını izleyin. R6 zaten başarıyla uygulandıysa doğrudan HTTP/Web kurucusuyla devam edin. HTTP/Web, gereken 0.1.6.2 iş akışı güncellemesini içerir; SQL/Windows parolalarını yeniden istemez. **0.1.6.2 veya HTTP/Web kurulduktan sonra R6'yı tekrar çalıştırmayın.** Yeni sunucuda önce tam 0.1.6 temel kurulum gerekir.

Windows istemcisi ve tarayıcı aynı kök adresi kullanır: `http://SUNUCUNUN-OZEL-IP-ADRESI:8080` (örneğin `http://192.168.1.10:8080`). Sonuna `/api` eklenmez. HTTP şifrelenmez; yalnız güvenilir şirket ağı/VPN için kullanın, internete açmayın. iPhone için Safari web yolu bulunur; yerel iOS dağıtım paketi yoktur. Gerçek iPhone/Safari cihaz doğrulaması yapılmadı.

Fatura ekranında Belegdatum/Übertrag alanları, sabit EUR, yönetici tarafından düzenlenen alan etiketleri ve insan kontrolü/onayı bulunur. Orijinal PDF indirme ile ayrı **İçeri aktar** ekranı birbirinden ayrıdır. Ortak gelen kutusuna yüklemek için kaynakta **Read + Manage** gerekir; yalnız Read verilen kullanıcı görüntüleyip izinli orijinali indirebilir. PDF başına sınır 50 MiB'dir. Almanca/İngilizce/Türkçe OCR ve alan düzeltmeleri orijinal dosyayı değiştirmez.

Doğrulama: son UTF-8 Client 0.1.6 paketiyle gerçek 0.1.4 → 0.1.6 kurulum, yükseltme ve kaldırma kabulü **64/64**, temizlik **1/1** geçti; profil metadatası korundu. **51 Flutter testi**, analiz, Windows ve Web derlemeleri geçti. Sunucu birleşik özellik/yaşam döngüsü kabulü: **85/85 kurulum/servis, 69/69 fatura/OCR ve ilk/yeniden kurulumda 28/28 HTTP kontrolü geçti; hizmet 6,07 saniyede otomatik toparlandı. Test kaynaklarının ve geçici SQL hesabının temizliği doğrulandı**. Native istemci GUI'si, gerçek tarayıcı etkileşimleri ve iPhone/Safari cihaz incelemesi doğrulanmadı; kurulum kabulü bu testlerin yerine geçmez.

| Dosya | Bayt | SHA256 |
| --- | ---: | --- |
| HTTP/Web 0.1.0 | 42988406 | `DC838E720744BF22B05C963E0DCED80B26EFA89E4A0F2FCD3AC84CEBFCDF1A86` |
| Client 0.1.6 | 36887581 | `FBADDCCA6AD0AA19F37952DF87FBADD5E6B7A740C205DAE3C9B40F88F57316E7` |

[HTTP/Web SHA256 dosyası](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-http-web-0.1.0/Archiv-HTTP-Web-Setup-0.1.0.exe.sha256) · [Client SHA256 dosyası](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-client-0.1.6/Archiv-Client-Setup-0.1.6.exe.sha256)

Bu herkese açık depo yalnız kurulum dosyaları, sağlama toplamları ve kullanım rehberi içindir. Kurucular Releases varlıkları olarak paylaşılır; özel projenin kaynak kodu burada yayımlanmaz. Bu paketler yerelde derlendi; bu çalışma için GitHub Actions başlatılmadı.
