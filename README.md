# JavaScript çalışma notları

Türkçe açıklamalı **1.000 metot ve fonksiyon**, 10 bölüm.

## Çalışmaya başla

- [Başlıklara göre düzenlenmiş çalışma notları](notes/javascript.md)
- [1.000 maddelik JSON dosyası](data/javascript.json)
- [10 sayfalık yazdırılabilir PDF](pdf/javascript-1000.pdf)

Metot adları `.startsWith()` gibi kısa tutulmuştur. `String`, `Array`, `Map` ve diğer grup başlıkları bağlamı gösterir. Aynı isim farklı nesnelerde farklı davranabilir.

## Bölümler

1. Metinler, diziler ve türlenmiş diziler
2. Nesneler, koleksiyonlar ve matematik
3. Tarih, uluslararasılaştırma ve düzenli ifadeler
4. Genel işlevler, ikili bellek ve konsol
5. Promise, ağ istekleri ve akışlar
6. DOM ve HTML öğeleri
7. Canvas ve çizim
8. Depolama, performans ve iletişim
9. Node.js dosyaları, yolları ve işletim sistemi
10. Node.js Buffer, kriptografi ve olaylar

## Kullanım

Her bölüm 100 madde içerir. Günde 10 madde okuyup her biri için küçük bir örnek yazabilirsin.

- `[statik]` işaretli çağrılar sınıf üzerinden kullanılır.
- Diğer örnek metotları ilgili nesne üzerinde çağır: `"hello".startsWith("he")`.
- `()` yalnızca çağrı adını gösterir; zorunlu argümanlar yazılmamıştır.
- Liste JavaScript çekirdeğinin yanı sıra tarayıcı ve Node.js API’lerini de içerir. Hepsi her ortamda çalışmaz.
- Yeni API’ler güncel çalışma zamanı gerektirebilir; Web API’lerinde izin veya güvenli bağlam gerekebilir.
- PDF için **A4, yatay, sayfaya sığdır** seç.

## JSON yapısı

`entries` dizisinde `id`, `section`, `section_title`, `group`, `name`, `api`, `description_tr`, `kind` ve `environment` alanları bulunur. `name` kısa gösterimdir; `api` tam API adını korur.

## Başvuru kaynakları

- [MDN JavaScript referansı](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)
- [MDN Web API referansı](https://developer.mozilla.org/en-US/docs/Web/API)
- [Node.js API referansı](https://nodejs.org/api/)
