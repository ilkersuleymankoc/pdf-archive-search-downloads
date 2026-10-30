# PDF Archive Search — Windows kurulumları

| Paket | İndir |
| --- | --- |
| Mevcut sunucuya güncelleme 0.1.6.1 | [Archiv-Server-Update-0.1.6.1.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.1/Archiv-Server-Update-0.1.6.1.exe) |
| Windows istemcisi 0.1.4 | [Archiv-Client-Setup-0.1.4.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-client-0.1.4/Archiv-Client-Setup-0.1.4.exe) |
| Yeni sunucu için temel kurulum 0.1.6 | [Archiv-Server-Setup-0.1.6.exe](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-0.1.6/Archiv-Server-Setup-0.1.6.exe) |

**Çalışan sunucuda önce 0.1.6.1 güncellemesini yönetici olarak çalıştırın; sonra istemciyi 0.1.4'e güncelleyin.** Önceki sürümü kaldırmayın; ProgramData, Config, SQL veritabanı ve PDF'leri silmeyin. Mevcut bağlantılar, hesaplar, kaynaklar, izinler ve indeksleyici Windows hesabı korunur. SQL/Windows parolası yeniden istenmez. Yeni sunucuda önce tam 0.1.6 kurulumu, ardından güncelleme gerekir.

[Kurulum ve kullanım adımları](https://github.com/ilkersuleymankoc/pdf-archive-search-downloads/releases/download/windows-server-update-0.1.6.1/Archiv-Guncelleme-0.1.6.1.txt)

Güncelleme API ve indeksleyicinin beklenmeyen işlem çıkışlarından toparlanmasını, yerel sabit disk klasörlerinin ek paylaşım/kök listesi olmadan okunmasını, kaynak silmeyi ve fatura inceleme ekranını ekler. Windows hesabının dosya okuma hakkı gerekir; UNAS/SMB izinleri geçerlidir. Fatura alanları yerel metin/OCR'den çıkarılır ve elle düzeltilebilir; özgün PDF'ler değişmez.

Son sunucu güncelleme EXE'siyle Windows 11 x64 / SQL Server 2022 Express üzerinde 70 kurulum/yaşam döngüsü, 37 kaynak/fatura ve 11 temel API/PDF/OCR kontrolü geçti. Zorla kapatma sonrasında API 8,84 saniyede, indeksleyici 6,97 saniyede elle müdahale olmadan geri geldi. Görev durdurma, güncellemeyi tekrar uygulama, kaldırma ve test temizliği geçti. İstemcide 56 gerçek kurulum/açılış/kaldırma kontrolü ve 32 Flutter testi geçti; analiz temiz.

Gerçek şirket Windows Server / SQL Server 2019 Standard / UNAS, 40.000 PDF kapasitesi, uzak HTTPS, işletim sistemi yeniden başlatması ve iOS bu yerel kabul kapsamında doğrulanmadı.

| Dosya | Bayt | SHA256 |
| --- | ---: | --- |
| Sunucu güncellemesi 0.1.6.1 | 275517 | `6B76B934DD3DD7F483B944286C15C370DBC61F639F04EA4A59649E204EECDEC0` |
| İstemci 0.1.4 | 36543446 | `F8ADD1483B69CEE45622914ECD9F8FF0B3A491848E87BBB42E2E140DD61DFC5F` |
| Tam sunucu kurulumu 0.1.6 | 112104280 | `CC656ECC39404C67629DE0547D4436BF7B0599FBC9BECF5D5116DC7250CD6201` |

Bu depo yalnız kurulum dosyaları ve kullanım bilgileri içindir. Dosyalar GitHub Releases'te tutulur; özel projenin kaynak kodu bu depoya konmaz. Bu sürümler yerelde derlendi, GitHub Actions çalıştırılmadı. 30.10.2026 kontrolünde her iki deponun Actions artifact ve cache kullanımı 0 bayttı.

