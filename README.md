# FgAutoBanner-Tr-

CS 1.6 sunucuları için Türk hilecilerin nicklerini listeleyen ve sunucuya o nickle girenleri otomatik tespit edip banlayan AMX Mod X eklentisi.

> Sadece göz atmak isterseniz: **[Herkese açık liste sayfası](https://github.com/Gokalpgokcee/Cs1.6-Tr-Hacker-List)**

## Nasıl çalışır?

1. Python scripti Fungun'daki "Cheats detected" kayıtlarından Türk oyuncuların nicklerini çeker.
2. İkinci script nickleri temizler: tekrarları siler, bozuk karakterleri düzeltir.
3. Eklenti bu listeyi okur. Listedeki bir nickle sunucuya giren oyuncuya `amx_addban` ile ban uygular.

## Kurulum

1. Eklentiyi (`.amxx`) `addons/amxmodx/plugins/` klasörüne koyun.
2. `addons/amxmodx/configs/plugins.ini` dosyasına eklentinin adını yazın.
3. Nick listesini eklentinin okuduğu konuma koyun (`DOSYA_YOLU_BURAYA`).
4. Sunucuyu yeniden başlatın veya haritayı değiştirin.

## Listeyi güncelleme

```
python SCRIPT_1.py   # nickleri çeker
python SCRIPT_2.py   # nickleri temizler
```

Scriptlerin gerçek adlarını ve gerekli Python sürümünü buraya yazın.

## Önemli uyarı

**Nick eşleşmesi kimlik kanıtı değildir.** Aynı nicki kullanan masum bir oyuncu, ya da bir nicki taklit eden biri yanlışlıkla banlanabilir. Özellikle kısa ve yaygın nickler (`ez`, `Alfa34` gibi) risklidir.

Bu yüzden önerilenler:

- Kalıcı ban yerine **kısa süreli ban** veya sadece **yöneticilere uyarı** kullanın.
- Çok kısa nickleri otomatik ban dışında tutun.
- Bir oyuncu itiraz ederse banı kaldırın.

Eklentiyi kullanmak kendi sorumluluğunuzdadır.

## Veri ve gizlilik

- Liste yalnızca oyun içi nickleri içerir. IP adresleri yayınlanmaz.
- Kayıtlar otomatik tespite dayanır ve hatalı olabilir.
- Listeden çıkarılmak veya hatalı kaydı bildirmek için: **4mp21diz5@mozmail.com**

## Katkı

Hata bildirimi ve öneriler için [Issues](../../issues) bölümünü kullanabilirsiniz.

## Lisans

[MIT](LICENSE)
