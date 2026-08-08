# READMEMarketOOP

Bu dosya, depodaki `JS-OOP-E-Ticaret Ve Market Örneği.js` dosyası için hazırlanmış kısa bir açıklama ve kullanım rehberidir.

## Özet

Bu örnek, JavaScript ile Nesne Yönelimli Programlama (OOP) kullanarak basit bir e-ticaret / market senaryosu uygular. Ürünler (genel), Elektronik ve Gıda ürünlerini temsil eden sınıflar tanımlanır; ayrıca bir `Sepet` sınıfı ile ürünleri sepete ekleyip toplam tutarı hesaplama gösterilmiştir.

## Dosya

- `JS-OOP-E-Ticaret Ve Market Örneği.js` — Örnek uygulama dosyası (sınıf tanımları, örnek ürünler ve sepet işlemleri).

## İçindekiler (kısa açıklama)

- sınıf ürün
  - Genel ürün özellikleri: isim, birim_fiyat, stok, gelir hesaplaması
  - Erişim metodları: `getİsim`, `getBirimFiyat`, `getStok`, `getGelir`

- sınıf Elektronik (ürün'den extends)
  - Ek özellikler: hafıza, marka, garanti_süresi
  - Erişim metodları: `getHafiza`, `getMarka`, `getGarantiSüresi`

- sınıf Gida (ürün'den extends)
  - Ek özellikler: gramaj, son_kullanma_tarihi
  - Erişim metodları: `getGramaj`, `getSonTüketimTarihi`

- sınıf Sepet
  - Sepete ürün ekleme (`sepeteEkle`) ve sepeti yazdırma (`sepeti_yazdir`) metodları
  - Stok kontrolü, toplam tutar güncelleme ve stoktan düşme işlemleri içerir

## Nasıl çalıştırılır

1. Node.js yüklü olduğundan emin olun (recommended: Node 14+).
2. Depoyu klonladıysanız veya dosya yerelinizdeyse, terminalde dosyanın bulunduğu dizine gidin.
3. Aşağıdaki komutla dosyayı çalıştırın:

```bash
node "JS-OOP-E-Ticaret Ve Market Örneği.js"
```

Çıktıda sepete ekleme bilgileri ve sepet özeti gözükecektir.

## Nasıl genişletilir / özelleştirilir

- Yeni ürünler ekleyebilir veya mevcut örnekleri değiştirebilirsiniz.
- Sepete ürün çıkarma, adet güncelleme, indirim/kupon mekanizması, sipariş özeti (fatura) gibi özellikler eklenebilir.
- Modüler kullanım için sınıfları modül haline getirip `export`/`import` ile ayrıştırabilirsiniz.

## Dikkat Edilmesi Gerekenler

- Dosya ve sınıf isimlerinde Türkçe karakterler (örn. `ürün`, `Gida`) kullanılmış; bazı araçlar veya ortamlar bu karakterleri farklı yorumlayabilir.
- Tarih formatları (`son_kullanma_tarihi`) örnek amaçlıdır; gerçek uygulamalarda Date objesi veya ISO formatı kullanılması önerilir.

## Lisans ve Yazar

Bu örnek küçük eğitim amaçlı bir koddur. Yazar: calti23 (GitHub).

