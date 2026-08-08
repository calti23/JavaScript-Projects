# Banka Hesabı OOP Örneği

Bu dosya, `JS-Banka Hesabı OOP Örneği.js` içindeki üç basit JavaScript sınıfı örneğini açıklar ve nasıl çalıştırılacağını gösterir.

## İçerik
- BankAccount: Kapanış (closure) kullanarak özel `budget` alanı sağlayan basit bir banka hesabı sınıfı. `deposit`, `withdraw` ve `getBudget` metotlarını içerir.
- Animal / Dog: Kalıtım (inheritance) örneği. `Animal` temel sınıfı ve ondan türeyen `Dog` sınıfı gösterilir (`bark` metodu ile).
- Person: Basit bir kişi sınıfı, `introduce` adlı metot ile kendini tanıtır.

## Çalıştırma
Node.js yüklü ise projeyi terminalden çalıştırmak için:

```bash
node "JS-Banka Hesabı OOP Örneği.js"
```

Beklenen çıktı (örneğe bağlı olarak):
- BankAccount örneği için güncellenmiş bakiye (deposit sonrası)
- Dog örneğinin havlama çıktısı ve tür/isim
- Person örneğinin tanıtım satırı

## Önemli Notlar ve Düzeltme Önerisi
Orijinal dosyada `withdraw` metodunda bir hata bulunuyor:

- `withdraw` içinde kullanılan `_budget` isimli değişken tanımlı değil; bu durumda çalışma zamanında ReferenceError oluşur veya şart yanlış değerlendirilir.

Düzeltme önerisi: `withdraw` koşulunu `if (amount <= newbudget) { ... }` şeklinde güncelleyin. Örnek:

```javascript
this.withdraw = function (amount) {
  if (amount <= newbudget) {
    newbudget -= amount;
  } else {
    console.log("NOT SUIT TO WITHDRAW!!!");
  }
}
```

Bu değişiklik, sınıfın kapalı (private) `newbudget` değişkenini doğru şekilde kontrol eder.

## Dosya
Kaynak dosya: `JS-Banka Hesabı OOP Örneği.js`

---

Bu README, dosyayı daha hızlı anlamanız ve örnekleri çalıştırmanız için hazırlandı. İsterseniz README'yi genişletip her sınıf için test örnekleri ve beklenen çıktıları ekleyebilirim.