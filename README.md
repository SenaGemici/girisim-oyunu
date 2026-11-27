# 10 Saniyede Startup

**Bir problem, 10 saniye, bir girişim fikri!**

[birseyleryapiyoruz](https://www.instagram.com/birseyler_yapiyoruz/) Instagram hesabı için hazırlanmış interaktif bir mini oyun. Öğrencilere günlük hayattan rastgele bir problem gösterilir ve bu probleme 10 saniyede yaratıcı bir girişim fikri bulmaları istenir. Kabataş Erkek Lisesi'ndeki girişimcilik etkinliğinde Reels çekimi için tasarlandı.

## Nasıl oynanır

1. **Rastgele konu seç**: Slot makinesi animasyonuyla bir problem seçilir.
2. Konu ekranda büyük harflerle görünür. Öğrenci hemen düşünmeye başlar.
3. Öğrenci hazır olunca **Süreyi başlat**: önce *HAZIR → BAŞLA!*, ardından 10 saniyelik geri sayım.
4. Süre bitince: **"Süre doldu! Girişim fikrin ne?"**
5. Sıradaki öğrenci için **Yeni konu**, aynı konuyu yeniden denemek için **Tekrar**.

## Özellikler

- 50 konuluk havuz. Tüm konular gösterilmeden aynı konu tekrar gelmez. Kalınan yer sayfa yenilense de hatırlanır.
- Daralan dairesel geri sayım. Son 3 saniyede kırmızıya döner ve titrer.
- Açılıp kapatılabilen ses efektleri. Sesler tarayıcıda üretilir, ses dosyası yoktur.
- Tam ekran modu. Oyun sırasında ekran kararmaz (destekleyen tarayıcılarda).
- Geri sayımın yanlışlıkla iki kez başlatılmasına karşı koruma.
- 9:16 dikey telefon ekranı öncelikli, masaüstünde de çalışır.
- **Tek dosya, internetsiz çalışır:** backend, kurulum veya harici kaynak gerekmez.

## Klavye kısayolları

Laptoptan yönetirken:

| Tuş | İşlev |
|-----|-------|
| `Space` / `Enter` | Sıradaki adım (konu seç / süreyi başlat) |
| `N` | Yeni konu |
| `R` | Tekrar başlat |
| `M` | Sesi aç/kapat |
| `F` | Tam ekran |
| `Esc` | Geri sayımı iptal et |

## Çalıştırma

`index.html` dosyasını herhangi bir tarayıcıda açmak yeterli.

Telefonda kullanmak için dosyayı bir statik hosting'e (GitHub Pages, Netlify vb.) yükleyip adresi telefonda açın, ardından ana ekrana ekleyin:

- **iPhone (Safari):** Paylaş → Ana Ekrana Ekle
- **Android (Chrome):** ⋮ menüsü → Ana ekrana ekle

Ana ekrandan açıldığında oyun adres çubuğu olmadan, tam ekran çalışır.

> **Etkinlik ipucu:** Sayfa bir kez yüklendikten sonra internet olmadan da çalışır, yeter ki yenilenmesin. Çekimden önce ekran parlaklığını artırın. iPhone'da sessiz mod açıkken sesler çıkmayabilir.

## Konuları değiştirme

`index.html` içindeki `TOPICS` listesini düzenleyin. Her satır bir konu.

```js
const TOPICS = [
  'Okul kantinindeki uzun sıralar',
  'Sınav stresi',
  // ...
];
```

Geri sayım süresi `DURATION` sabitinden (milisaniye) değiştirilebilir. Süreyi değiştirirseniz başlıktaki ve metinlerdeki "10" ifadelerini de güncellemeyi unutmayın.
