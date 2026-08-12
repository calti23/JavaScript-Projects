# READMEGitHubAnalyzer

JS GitHub Analyzer, GitHub depolarını hızlıca incelemek için tasarlanmış hafif bir JavaScript aracıdır. Bu araç; dil dağılımı, dosya sayıları, önemli dosyaların varlığı (README, LICENSE, package.json) ve package.json varsa bağımlılık listesini çıkararak JSON ve insan okunur özet halinde çıktı üretir.

Bu depo, bir dizi bağımsız JavaScript örnek projesi içerir. "JS-GitHub Analyzer" aracı bir zip dosyası olarak repoda bulunur; içeriğini açarak tarayıcıda veya yerel sunucuda çalıştırabilirsiniz.

Özellikler

- Depo dil dağılımı ve yaklaşık satır sayısını raporlar
- Dosya sayıları ve dikkat çeken dosyaları listeler (README, LICENSE, package.json vb.)
- package.json içindeki bağımlılıkları çıkarır
- Çıktıyı JSON olarak kaydeder ve kısa bir özet yazdırır

Dosya düzeni (kök dizin)

- JS-GitHub Analyzer.zip — Analiz aracının sıkıştırılmış dağıtımı (index.html, project.js, assetler)
- JS-Banka Hesabı OOP Örneği.js — Banka hesabı, hayvan, kişi örnekleri
- JS-OOP Kütüphane Örneği.js — Kitap ve kütüphane OOP örneği
- JS-OOP-E-Ticaret Ve Market Örneği.js — Ürün, sepet ve türler içeren örnek
- JS-Weather Forecast Project.zip — Hava durumu tahmin örneği (statik site)
- README*.md — Her örnek için ayrı açıklayıcı dosyalar

Nasıl çalıştırılır

1. Depoyu klonlayın:

   git clone https://github.com/calti23/JavaScript-Projects.git
   cd JavaScript-Projects

2. JS-GitHub Analyzer'ı açma (hızlı yol - tarayıcı):
   - `JS-GitHub Analyzer.zip` dosyasını açın ve içindeki klasörü çıkarın.
   - `index.html` dosyasını bir tarayıcıda açın.

3. Veya yerel statik sunucu ile servis edin:

   npx serve "JS-GitHub Analyzer"
   # veya
   python -m http.server 8000 --directory "JS-GitHub Analyzer"

   Sonra tarayıcıda http://localhost:5000 (veya sunucunun raporladığı port) adresini açın.

4. Eğer proje `project.js` gibi bir Node betiği içeriyorsa CLI ile JSON çıktı almak için:

   node "JS-GitHub Analyzer/project.js" --path /path/to/repo --output result.json

Notlar

- Bu repoda kök düzeyinde package.json veya merkezi bir build sistemi gözükmüyor; her örnek bağımsız çalışır.
- ZIP içindeki dağıtımın nasıl çalıştığını görmek için önce klasörü açın ve `index.html` ile `project.js` dosyalarını inceleyin.

Katkıda bulunma

Katkılar için teşekkürler — issue açabilir veya pull request gönderebilirsiniz. Öneriler:

- `JS-GitHub Analyzer` klasörünü açıp `package.json` ekleyerek npm scriptleri (`start`, `build`) ekleyin
- CLI için daha sağlam argüman işleme ve testler ekleyin
- Tarayıcı arayüzüne GitHub repo URL'si ile analiz özelliği ekleyin (CORS/İzinler göz önüne alınarak)

Lisans

Bu projede lisans belirtilmemiştir. Açık kaynak lisansı eklemek isterseniz (ör. MIT) bir LICENSE dosyası ekleyin.

İletişim

Sorumlu: calti23
