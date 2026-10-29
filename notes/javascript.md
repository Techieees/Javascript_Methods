# JavaScript çalışma notları

Türkçe açıklamalı 1.000 metot ve fonksiyon · 10 bölüm

Başlık, metodu çağıracağın nesneyi veya modülü gösterir. `.startsWith()` gibi kısa adlar kullanılır. `()` içindeki gerekli argümanlar gösterilmez.

`[statik]` sınıf üzerinden çağrılan metodu belirtir. Tarayıcı ve Node.js başlıkları çalışma ortamını gösterir. Bazı yeni API’ler güncel sürüm gerektirir.

## Bölümler

- [Bölüm 01: JavaScript: metinler, diziler ve türlenmiş diziler](#bolum-01)
- [Bölüm 02: JavaScript: nesneler, koleksiyonlar ve matematik](#bolum-02)
- [Bölüm 03: JavaScript: tarih, uluslararasılaştırma ve desenler](#bolum-03)
- [Bölüm 04: JavaScript: genel işlevler, bellek ve günlükleme](#bolum-04)
- [Bölüm 05: Asenkron işlemler, ağ ve akış API'leri](#bolum-05)
- [Bölüm 06: Tarayıcı: DOM, belge ve HTML öğeleri](#bolum-06)
- [Bölüm 07: Tarayıcı: Canvas, çizim ve görseller](#bolum-07)
- [Bölüm 08: Tarayıcı: depolama, performans ve iletişim](#bolum-08)
- [Bölüm 09: Node.js: dosyalar, yollar ve işletim sistemi](#bolum-09)
- [Bölüm 10: Node.js: Buffer, kriptografi ve olaylar](#bolum-10)

<a id="bolum-01"></a>
## Bölüm 01: JavaScript: metinler, diziler ve türlenmiş diziler


### String

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 1 | `.fromCharCode() [statik]` | UTF-16 kod birimlerinden metin üretir. |
| 2 | `.fromCodePoint() [statik]` | Unicode kod noktalarından metin üretir. |
| 3 | `.raw() [statik]` | Şablonun ham metin parçalarını kullanır. |
| 4 | `.at()` | Konumdaki UTF-16 birimini getirir. |
| 5 | `.charAt()` | Konumdaki karakteri getirir. |
| 6 | `.charCodeAt()` | Konumdaki UTF-16 kodunu verir. |
| 7 | `.codePointAt()` | Konumdaki Unicode kod noktasını verir. |
| 8 | `.concat()` | Metinleri birleştirir. |
| 9 | `.endsWith()` | Belirtilen son ekle bitiyor mu? |
| 10 | `.includes()` | Alt metni içeriyor mu? |
| 11 | `.indexOf()` | İlk eşleşme konumunu verir. |
| 12 | `.lastIndexOf()` | Son eşleşme konumunu verir. |
| 13 | `.localeCompare()` | Yerel kurallarla karşılaştırır. |
| 14 | `.match()` | Düzenli ifadeyle eşleşmeleri alır. |
| 15 | `.matchAll()` | Eşleşmeleri yineleyici olarak verir. |
| 16 | `.normalize()` | Unicode normalleştirmesi yapar. |
| 17 | `.padEnd()` | Sonuna dolgu ekleyerek uzatır. |
| 18 | `.padStart()` | Başına dolgu ekleyerek uzatır. |
| 19 | `.repeat()` | Metni belirtilen sayıda tekrarlar. |
| 20 | `.replace()` | İlk veya desene bağlı eşleşmeleri değiştirir. |
| 21 | `.replaceAll()` | Bütün eşleşmeleri değiştirir. |
| 22 | `.search()` | Düzenli ifadenin ilk konumunu bulur. |
| 23 | `.slice()` | Metnin bir bölümünü kopyalar. |
| 24 | `.split()` | Ayırıcıya göre dizi oluşturur. |
| 25 | `.startsWith()` | Belirtilen başlangıçla başlıyor mu? |
| 26 | `.substring()` | İki indis arasındaki metni alır. |
| 27 | `.toLocaleLowerCase()` | Yerel kurallarla harfleri küçültür. |
| 28 | `.toLocaleUpperCase()` | Yerel kurallarla harfleri büyütür. |
| 29 | `.toLowerCase()` | Harfleri küçültür. |
| 30 | `.toUpperCase()` | Harfleri büyütür. |
| 31 | `.trim()` | İki uçtaki boşlukları kaldırır. |
| 32 | `.trimEnd()` | Sondaki boşlukları kaldırır. |
| 33 | `.trimStart()` | Baştaki boşlukları kaldırır. |
| 34 | `.toString()` | Metin değerini döndürür. |
| 35 | `.valueOf()` | İlkel metin değerini döndürür. |

### Array

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 36 | `.from() [statik]` | Yinelenebilir veya dizi benzerinden dizi kurar. |
| 37 | `.fromAsync() [statik]` | Asenkron kaynaktan Promise ile dizi üretir. |
| 38 | `.isArray() [statik]` | Değerin dizi olduğunu kontrol eder. |
| 39 | `.of() [statik]` | Argümanlardan dizi oluşturur. |
| 40 | `.at()` | Negatif indis de destekleyerek öğe alır. |
| 41 | `.concat()` | Dizileri yeni dizide birleştirir. |
| 42 | `.copyWithin()` | Öğeleri dizi içinde kopyalar. |
| 43 | `.entries()` | İndis ve değer çiftlerini yineler. |
| 44 | `.every()` | Bütün öğeler koşulu sağlıyor mu? |
| 45 | `.fill()` | Diziyi verilen değerle doldurur. |
| 46 | `.filter()` | Koşulu sağlayan öğeleri seçer. |
| 47 | `.find()` | Koşulu sağlayan ilk öğeyi bulur. |
| 48 | `.findIndex()` | Koşulu sağlayan ilk indisi bulur. |
| 49 | `.findLast()` | Koşulu sağlayan son öğeyi bulur. |
| 50 | `.findLastIndex()` | Koşulu sağlayan son indisi bulur. |
| 51 | `.flat()` | İç içe dizileri düzleştirir. |
| 52 | `.flatMap()` | Eşler ve bir düzey düzleştirir. |
| 53 | `.forEach()` | Her öğe için işlev çalıştırır. |
| 54 | `.includes()` | Öğenin varlığını kontrol eder. |
| 55 | `.indexOf()` | Öğenin ilk konumunu bulur. |
| 56 | `.join()` | Öğeleri ayırıcıyla metne çevirir. |
| 57 | `.keys()` | Dizi indislerini yineler. |
| 58 | `.lastIndexOf()` | Öğenin son konumunu bulur. |
| 59 | `.map()` | Öğeleri dönüştürüp yeni dizi üretir. |
| 60 | `.pop()` | Son öğeyi çıkarıp döndürür. |
| 61 | `.push()` | Sona öğe ekler; yeni uzunluğu verir. |
| 62 | `.reduce()` | Soldan birikimli sonuç hesaplar. |
| 63 | `.reduceRight()` | Sağdan birikimli sonuç hesaplar. |
| 64 | `.reverse()` | Öğe sırasını yerinde tersine çevirir. |
| 65 | `.shift()` | İlk öğeyi çıkarıp döndürür. |
| 66 | `.slice()` | Dizinin bölümünü kopyalar. |
| 67 | `.some()` | En az bir öğe koşulu sağlıyor mu? |
| 68 | `.sort()` | Diziyi yerinde sıralar. |
| 69 | `.splice()` | Aradan öğe siler, değiştirir veya ekler. |
| 70 | `.toLocaleString()` | Öğeleri yerel kurallarla metne çevirir. |
| 71 | `.toReversed()` | Ters sıralı yeni dizi üretir. |
| 72 | `.toSorted()` | Sıralanmış yeni dizi üretir. |
| 73 | `.toSpliced()` | Kesme ve eklemeyi yeni diziye uygular. |
| 74 | `.toString()` | Diziyi metne dönüştürür. |
| 75 | `.unshift()` | Başa öğe ekler; yeni uzunluğu verir. |
| 76 | `.values()` | Dizi değerlerini yineler. |
| 77 | `.with()` | Tek konumu değiştirilmiş kopya üretir. |

### Uint8Array

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 78 | `.from() [statik]` | Kaynaktan sekiz bitlik dizi oluşturur. |
| 79 | `.of() [statik]` | Argümanlardan sekiz bitlik dizi kurar. |
| 80 | `.set()` | Başka dizinin değerlerini kopyalar. |
| 81 | `.subarray()` | Aynı bellekte alt dizi görünümü verir. |
| 82 | `.slice()` | Dizi bölümünün kopyasını üretir. |
| 83 | `.at()` | Konumdaki sayısal öğeyi alır. |
| 84 | `.copyWithin()` | Değerleri aynı dizi içinde kopyalar. |
| 85 | `.entries()` | İndis ve değer çiftlerini yineler. |
| 86 | `.every()` | Bütün sayılar koşulu sağlıyor mu? |
| 87 | `.fill()` | Diziyi sayısal değerle doldurur. |
| 88 | `.filter()` | Koşulu sağlayan sayıları seçer. |
| 89 | `.find()` | Koşulu sağlayan ilk sayıyı bulur. |
| 90 | `.findIndex()` | Koşulu sağlayan ilk indisi bulur. |
| 91 | `.forEach()` | Her sayı için işlev çalıştırır. |
| 92 | `.includes()` | Sayının dizide varlığını sınar. |
| 93 | `.indexOf()` | Sayının ilk konumunu bulur. |
| 94 | `.join()` | Sayıları ayırıcıyla metne çevirir. |
| 95 | `.keys()` | Sayısal dizinin indislerini yineler. |
| 96 | `.lastIndexOf()` | Sayının son konumunu bulur. |
| 97 | `.map()` | Sayıları yeni türlenmiş diziye eşler. |
| 98 | `.reduce()` | Sayıları tek bir sonuçta biriktirir. |
| 99 | `.reduceRight()` | Sayıları sağdan biriktirir. |
| 100 | `.reverse()` | Sayısal diziyi yerinde ters çevirir. |

<a id="bolum-02"></a>
## Bölüm 02: JavaScript: nesneler, koleksiyonlar ve matematik


### Object

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 101 | `.assign() [statik]` | Kaynakların kendi sayılabilir alanlarını kopyalar. |
| 102 | `.create() [statik]` | Belirtilen prototiple nesne oluşturur. |
| 103 | `.defineProperty() [statik]` | Bir özelliğin tanımını ayarlar. |
| 104 | `.defineProperties() [statik]` | Birden fazla özelliğin tanımını ayarlar. |
| 105 | `.entries() [statik]` | Kendi sayılabilir anahtar-değer çiftlerini verir. |
| 106 | `.fromEntries() [statik]` | Anahtar-değer çiftlerinden nesne kurar. |
| 107 | `.freeze() [statik]` | Nesnenin doğrudan özelliklerini dondurur. |
| 108 | `.getOwnPropertyDescriptor() [statik]` | Bir özelliğin tanımını getirir. |
| 109 | `.getOwnPropertyDescriptors() [statik]` | Kendi özellik tanımlarını getirir. |
| 110 | `.getOwnPropertyNames() [statik]` | Kendi metin özellik adlarını getirir. |
| 111 | `.getOwnPropertySymbols() [statik]` | Kendi sembol anahtarlarını getirir. |
| 112 | `.getPrototypeOf() [statik]` | Nesnenin prototipini getirir. |
| 113 | `.hasOwn() [statik]` | Özellik doğrudan nesneye mi ait? |
| 114 | `.is() [statik]` | Aynı değer karşılaştırması yapar. |
| 115 | `.isExtensible() [statik]` | Yeni özellik eklenebilir mi? |
| 116 | `.isFrozen() [statik]` | Nesne dondurulmuş mu? |
| 117 | `.isSealed() [statik]` | Nesne mühürlenmiş mi? |
| 118 | `.keys() [statik]` | Kendi sayılabilir metin anahtarlarını verir. |
| 119 | `.preventExtensions() [statik]` | Yeni özellik eklenmesini engeller. |
| 120 | `.seal() [statik]` | Özellik ekleme ve silmeyi engeller. |
| 121 | `.setPrototypeOf() [statik]` | Nesnenin prototipini değiştirir. |
| 122 | `.values() [statik]` | Kendi sayılabilir özellik değerlerini verir. |

### Reflect

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 123 | `.apply()` | İşlevi this ve argüman listesiyle çağırır. |
| 124 | `.construct()` | Kurucuyu argüman listesiyle çağırır. |
| 125 | `.defineProperty()` | Özellik tanımlar; başarı bilgisi döndürür. |
| 126 | `.deleteProperty()` | Özelliği siler; başarı bilgisi döndürür. |
| 127 | `.get()` | Nesne özelliğini getirir. |
| 128 | `.getOwnPropertyDescriptor()` | Kendi özellik tanımını getirir. |
| 129 | `.getPrototypeOf()` | Prototipi getirir. |
| 130 | `.has()` | Prototip zinciri dahil özellik var mı? |
| 131 | `.isExtensible()` | Nesne genişletilebilir mi? |
| 132 | `.ownKeys()` | Bütün kendi anahtarlarını getirir. |
| 133 | `.preventExtensions()` | Genişletmeyi engeller; başarıyı bildirir. |
| 134 | `.set()` | Özelliğe değer atar. |
| 135 | `.setPrototypeOf()` | Prototipi atar; başarıyı bildirir. |

### Map

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 136 | `.clear()` | Bütün anahtar-değer çiftlerini kaldırır. |
| 137 | `.delete()` | Anahtarı ve değerini siler. |
| 138 | `.entries()` | Anahtar-değer çiftlerini yineler. |
| 139 | `.forEach()` | Her çift için işlev çalıştırır. |
| 140 | `.get()` | Anahtarın değerini getirir. |
| 141 | `.has()` | Anahtar mevcut mu? |
| 142 | `.keys()` | Anahtarları yineler. |
| 143 | `.set()` | Anahtara değer atar. |
| 144 | `.values()` | Değerleri yineler. |

### Set

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 145 | `.add()` | Kümeye değer ekler. |
| 146 | `.clear()` | Kümeyi boşaltır. |
| 147 | `.delete()` | Değeri kümeden siler. |
| 148 | `.entries()` | Değer-değer çiftlerini yineler. |
| 149 | `.forEach()` | Her değer için işlev çalıştırır. |
| 150 | `.has()` | Değer kümede mevcut mu? |
| 151 | `.keys()` | Kümenin değerlerini yineler. |
| 152 | `.values()` | Kümenin değerlerini yineler. |

### WeakMap

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 153 | `.delete()` | Zayıf anahtar eşlemesini siler. |
| 154 | `.get()` | Zayıf anahtarın değerini getirir. |
| 155 | `.has()` | Zayıf anahtar mevcut mu? |
| 156 | `.set()` | Zayıf anahtara değer atar. |

### WeakSet

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 157 | `.add()` | Zayıf kümeye değer ekler. |
| 158 | `.delete()` | Değeri zayıf kümeden siler. |
| 159 | `.has()` | Değer zayıf kümede mevcut mu? |

### Math

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 160 | `.abs()` | Mutlak değer hesaplar. |
| 161 | `.acos()` | Ters kosinüs hesaplar. |
| 162 | `.acosh()` | Ters hiperbolik kosinüs hesaplar. |
| 163 | `.asin()` | Ters sinüs hesaplar. |
| 164 | `.asinh()` | Ters hiperbolik sinüs hesaplar. |
| 165 | `.atan()` | Ters tanjant hesaplar. |
| 166 | `.atanh()` | Ters hiperbolik tanjant hesaplar. |
| 167 | `.atan2()` | Koordinatların yön açısını hesaplar. |
| 168 | `.cbrt()` | Küpkök hesaplar. |
| 169 | `.ceil()` | Yukarı tamsayıya yuvarlar. |
| 170 | `.clz32()` | Otuz iki bitte baştaki sıfırları sayar. |
| 171 | `.cos()` | Radyan cinsinden kosinüs hesaplar. |
| 172 | `.cosh()` | Hiperbolik kosinüs hesaplar. |
| 173 | `.exp()` | e üzeri x hesaplar. |
| 174 | `.expm1()` | e üzeri x eksi bir hesaplar. |
| 175 | `.floor()` | Aşağı tamsayıya yuvarlar. |
| 176 | `.fround()` | Otuz iki bit kayan sayıya yuvarlar. |
| 177 | `.hypot()` | Kareler toplamının karekökünü alır. |
| 178 | `.imul()` | Otuz iki bit tamsayı çarpımı yapar. |
| 179 | `.log()` | Doğal logaritma hesaplar. |
| 180 | `.log1p()` | Bir artı x'in logaritmasını hesaplar. |
| 181 | `.log10()` | On tabanında logaritma hesaplar. |
| 182 | `.log2()` | İki tabanında logaritma hesaplar. |
| 183 | `.max()` | En büyük sayıyı verir. |
| 184 | `.min()` | En küçük sayıyı verir. |
| 185 | `.pow()` | Üs alma işlemi yapar. |
| 186 | `.random()` | Sıfır dahil, bir hariç rastgele sayı verir. |
| 187 | `.round()` | En yakın tamsayıya yuvarlar. |
| 188 | `.sign()` | Sayının işaretini verir. |
| 189 | `.sin()` | Radyan cinsinden sinüs hesaplar. |
| 190 | `.sinh()` | Hiperbolik sinüs hesaplar. |
| 191 | `.sqrt()` | Karekök hesaplar. |
| 192 | `.tan()` | Radyan cinsinden tanjant hesaplar. |
| 193 | `.tanh()` | Hiperbolik tanjant hesaplar. |
| 194 | `.trunc()` | Kesirli kısmı atar. |

### Number

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 195 | `.isFinite() [statik]` | Değer sonlu number mı? |
| 196 | `.isInteger() [statik]` | Değer tamsayı mı? |
| 197 | `.isNaN() [statik]` | Değer NaN mı? |
| 198 | `.isSafeInteger() [statik]` | Güvenli tamsayı aralığında mı? |
| 199 | `.parseFloat() [statik]` | Metnin başından ondalıklı sayı okur. |
| 200 | `.parseInt() [statik]` | Metnin başından tamsayı okur. |

<a id="bolum-03"></a>
## Bölüm 03: JavaScript: tarih, uluslararasılaştırma ve desenler


### Date

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 201 | `.now() [statik]` | Geçerli zamanı milisaniye damgası verir. |
| 202 | `.parse() [statik]` | Tarih metnini zaman damgasına çevirir. |
| 203 | `.UTC() [statik]` | UTC bileşenlerinden zaman damgası üretir. |
| 204 | `.getDate()` | Yerel ayın gününü verir. |
| 205 | `.getDay()` | Yerel hafta gününü pazar sıfırla verir. |
| 206 | `.getFullYear()` | Yerel yılı verir. |
| 207 | `.getHours()` | Yerel saati verir. |
| 208 | `.getMilliseconds()` | Yerel milisaniye alanını verir. |
| 209 | `.getMinutes()` | Yerel dakika alanını verir. |
| 210 | `.getMonth()` | Yerel ayı sıfır tabanlı verir. |
| 211 | `.getSeconds()` | Yerel saniye alanını verir. |
| 212 | `.getTime()` | Milisaniye zaman damgasını verir. |
| 213 | `.getTimezoneOffset()` | UTC eksi yerel farkını dakika verir. |
| 214 | `.getUTCDate()` | UTC ayın gününü verir. |
| 215 | `.getUTCDay()` | UTC hafta gününü verir. |
| 216 | `.getUTCFullYear()` | UTC yılını verir. |
| 217 | `.getUTCHours()` | UTC saatini verir. |
| 218 | `.getUTCMilliseconds()` | UTC milisaniye alanını verir. |
| 219 | `.getUTCMinutes()` | UTC dakika alanını verir. |
| 220 | `.getUTCMonth()` | UTC ayını sıfır tabanlı verir. |
| 221 | `.getUTCSeconds()` | UTC saniye alanını verir. |
| 222 | `.setDate()` | Yerel ayın gününü değiştirir. |
| 223 | `.setFullYear()` | Yerel yılı değiştirir. |
| 224 | `.setHours()` | Yerel saat bileşenlerini değiştirir. |
| 225 | `.setMilliseconds()` | Yerel milisaniyeyi değiştirir. |
| 226 | `.setMinutes()` | Yerel dakikayı değiştirir. |
| 227 | `.setMonth()` | Yerel ayı değiştirir. |
| 228 | `.setSeconds()` | Yerel saniyeyi değiştirir. |
| 229 | `.setTime()` | Milisaniye damgasını değiştirir. |
| 230 | `.setUTCDate()` | UTC ayın gününü değiştirir. |
| 231 | `.setUTCFullYear()` | UTC yılını değiştirir. |
| 232 | `.setUTCHours()` | UTC saat bileşenlerini değiştirir. |
| 233 | `.setUTCMilliseconds()` | UTC milisaniyeyi değiştirir. |
| 234 | `.setUTCMinutes()` | UTC dakikayı değiştirir. |
| 235 | `.setUTCMonth()` | UTC ayı değiştirir. |
| 236 | `.setUTCSeconds()` | UTC saniyeyi değiştirir. |
| 237 | `.toDateString()` | Yerel tarih metni üretir. |
| 238 | `.toISOString()` | UTC ISO tarih ve saat metni üretir. |
| 239 | `.toJSON()` | JSON için tarih metni üretir. |
| 240 | `.toLocaleDateString()` | Yerel kurallarla tarihi biçimler. |
| 241 | `.toLocaleString()` | Yerel kurallarla tarih ve saati biçimler. |
| 242 | `.toLocaleTimeString()` | Yerel kurallarla saati biçimler. |
| 243 | `.toString()` | Yerel tarih ve saati metne çevirir. |
| 244 | `.toTimeString()` | Yerel saat metni üretir. |
| 245 | `.toUTCString()` | UTC tarih ve saat metni üretir. |
| 246 | `.valueOf()` | Milisaniye damgasını ilkel değer verir. |

### Intl

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 247 | `.getCanonicalLocales() [statik]` | Dil etiketlerini standartlaştırır. |
| 248 | `.supportedValuesOf() [statik]` | Desteklenen uluslararası değerleri listeler. |

### Intl · biçimleyici örnekleri / statik

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 249 | `.Collator.supportedLocalesOf() [statik]` | Desteklenen karşılaştırma dillerini bulur. |
| 250 | `.Collator.compare()` | Yerel kurallarla iki metni karşılaştırır. |
| 251 | `.Collator.resolvedOptions()` | Etkin karşılaştırma seçeneklerini verir. |
| 252 | `.DateTimeFormat.supportedLocalesOf() [statik]` | Desteklenen tarih biçim dillerini bulur. |
| 253 | `.DateTimeFormat.format()` | Tarih ve saati yerel biçimde yazar. |
| 254 | `.DateTimeFormat.formatToParts()` | Tarih çıktısını anlamlı parçalara böler. |
| 255 | `.DateTimeFormat.formatRange()` | Tarih aralığını yerel biçimde yazar. |
| 256 | `.DateTimeFormat.formatRangeToParts()` | Tarih aralığını parçalara ayırır. |
| 257 | `.DateTimeFormat.resolvedOptions()` | Etkin tarih biçim seçeneklerini verir. |
| 258 | `.NumberFormat.supportedLocalesOf() [statik]` | Desteklenen sayı biçim dillerini bulur. |
| 259 | `.NumberFormat.format()` | Sayıyı yerel kurallarla biçimler. |
| 260 | `.NumberFormat.formatToParts()` | Sayı çıktısını anlamlı parçalara ayırır. |
| 261 | `.NumberFormat.formatRange()` | Sayı aralığını yerel biçimde yazar. |
| 262 | `.NumberFormat.formatRangeToParts()` | Sayı aralığını parçalara ayırır. |
| 263 | `.NumberFormat.resolvedOptions()` | Etkin sayı biçim seçeneklerini verir. |
| 264 | `.PluralRules.supportedLocalesOf() [statik]` | Desteklenen çoğul kuralı dillerini bulur. |
| 265 | `.PluralRules.select()` | Sayının çoğul kategorisini seçer. |
| 266 | `.PluralRules.selectRange()` | Sayı aralığının çoğul kategorisini seçer. |
| 267 | `.PluralRules.resolvedOptions()` | Etkin çoğul seçeneklerini verir. |
| 268 | `.RelativeTimeFormat.supportedLocalesOf() [statik]` | Desteklenen göreli zaman dillerini bulur. |
| 269 | `.RelativeTimeFormat.format()` | Göreli zaman ifadesi üretir. |
| 270 | `.RelativeTimeFormat.formatToParts()` | Göreli zaman çıktısını parçalara böler. |
| 271 | `.RelativeTimeFormat.resolvedOptions()` | Etkin göreli zaman seçeneklerini verir. |
| 272 | `.ListFormat.supportedLocalesOf() [statik]` | Desteklenen liste biçim dillerini bulur. |
| 273 | `.ListFormat.format()` | Metin listesini yerel kurallarla birleştirir. |
| 274 | `.ListFormat.formatToParts()` | Biçimli listeyi parçalara ayırır. |
| 275 | `.ListFormat.resolvedOptions()` | Etkin liste biçim seçeneklerini verir. |
| 276 | `.Segmenter.supportedLocalesOf() [statik]` | Desteklenen metin bölme dillerini bulur. |
| 277 | `.Segmenter.segment()` | Metni harf, sözcük veya cümleye böler. |
| 278 | `.Segmenter.resolvedOptions()` | Etkin bölümleme seçeneklerini verir. |
| 279 | `.DisplayNames.supportedLocalesOf() [statik]` | Desteklenen adlandırma dillerini bulur. |
| 280 | `.DisplayNames.of()` | Dil, bölge veya para biriminin adını verir. |
| 281 | `.DisplayNames.resolvedOptions()` | Etkin adlandırma seçeneklerini verir. |

### RegExp

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 282 | `.exec()` | Eşleşme ayrıntılarını veya null verir. |
| 283 | `.test()` | Desenin eşleşip eşleşmediğini sınar. |
| 284 | `.toString()` | Deseni ve bayraklarını metne çevirir. |

### JSON

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 285 | `.parse()` | JSON metnini JavaScript değerine çevirir. |
| 286 | `.stringify()` | Değeri JSON metnine dönüştürür. |

### BigInt

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 287 | `.asIntN() [statik]` | BigInt değerini işaretli bit genişliğine sarar. |
| 288 | `.asUintN() [statik]` | BigInt değerini işaretsiz bit genişliğine sarar. |
| 289 | `.toString()` | Tamsayıyı seçilen tabanda metne çevirir. |
| 290 | `.toLocaleString()` | Büyük tamsayıyı yerel kurallarla biçimler. |
| 291 | `.valueOf()` | İlkel BigInt değerini verir. |

### Boolean

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 292 | `.toString()` | Mantıksal değeri metne çevirir. |
| 293 | `.valueOf()` | İlkel mantıksal değeri verir. |

### Symbol

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 294 | `.for() [statik]` | Genel sembol kaydından sembol alır. |
| 295 | `.keyFor() [statik]` | Genel sembolün kayıt anahtarını bulur. |
| 296 | `.toString()` | Sembolün okunabilir gösterimini verir. |
| 297 | `.valueOf()` | İlkel sembol değerini verir. |

### Function

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 298 | `.apply()` | İşlevi this ve argüman dizisiyle çağırır. |
| 299 | `.bind()` | this ve bazı argümanları bağlar. |
| 300 | `.call()` | İşlevi açık this değeriyle çağırır. |

<a id="bolum-04"></a>
## Bölüm 04: JavaScript: genel işlevler, bellek ve günlükleme


### Genel işlevler

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 301 | `parseInt()` | Metnin başından belirtilen tabanda tamsayı okur. |
| 302 | `parseFloat()` | Metnin başından ondalıklı sayı okur. |
| 303 | `isFinite()` | Sayıya çevirerek sonluluğu sınar. |
| 304 | `isNaN()` | Sayıya çevirerek NaN olmasını sınar. |
| 305 | `encodeURI()` | Tam URI içindeki uygun karakterleri kodlar. |
| 306 | `decodeURI()` | Kodlanmış tam URI metnini çözer. |
| 307 | `encodeURIComponent()` | Tek URI bileşenini kodlar. |
| 308 | `decodeURIComponent()` | Kodlanmış URI bileşenini çözer. |
| 309 | `atob()` | Base64 metnini ikili metne çözer. |
| 310 | `btoa()` | İkili metni Base64 olarak kodlar. |

### ArrayBuffer

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 311 | `.isView() [statik]` | Değer türlenmiş dizi veya DataView mı? |
| 312 | `.slice()` | Bellek aralığının kopyasını oluşturur. |
| 313 | `.resize()` | Yeniden boyutlanabilir tamponu boyutlandırır. |
| 314 | `.transfer()` | Belleği yeni tampona aktarır; eskisini ayırır. |
| 315 | `.transferToFixedLength()` | Belleği sabit uzunluklu tampona aktarır. |

### DataView

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 316 | `.getInt8()` | İşaretli sekiz bit tamsayı okur. |
| 317 | `.getUint8()` | İşaretsiz sekiz bit tamsayı okur. |
| 318 | `.getInt16()` | İşaretli 16 bit tamsayı okur. |
| 319 | `.getUint16()` | İşaretsiz 16 bit tamsayı okur. |
| 320 | `.getInt32()` | İşaretli 32 bit tamsayı okur. |
| 321 | `.getUint32()` | İşaretsiz 32 bit tamsayı okur. |
| 322 | `.getFloat32()` | 32 bit kayan noktalı sayı okur. |
| 323 | `.getFloat64()` | 64 bit kayan noktalı sayı okur. |
| 324 | `.getBigInt64()` | İşaretli 64 bit BigInt okur. |
| 325 | `.getBigUint64()` | İşaretsiz 64 bit BigInt okur. |
| 326 | `.setInt8()` | İşaretli sekiz bit tamsayı yazar. |
| 327 | `.setUint8()` | İşaretsiz sekiz bit tamsayı yazar. |
| 328 | `.setInt16()` | İşaretli 16 bit tamsayı yazar. |
| 329 | `.setUint16()` | İşaretsiz 16 bit tamsayı yazar. |
| 330 | `.setInt32()` | İşaretli 32 bit tamsayı yazar. |
| 331 | `.setUint32()` | İşaretsiz 32 bit tamsayı yazar. |
| 332 | `.setFloat32()` | 32 bit kayan noktalı sayı yazar. |
| 333 | `.setFloat64()` | 64 bit kayan noktalı sayı yazar. |
| 334 | `.setBigInt64()` | İşaretli 64 bit BigInt yazar. |
| 335 | `.setBigUint64()` | İşaretsiz 64 bit BigInt yazar. |
| 336 | `.getFloat16()` | 16 bit kayan noktalı sayı okur. |
| 337 | `.setFloat16()` | 16 bit kayan noktalı sayı yazar. |

### Atomics

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 338 | `.add()` | Atomik toplar; önceki değeri verir. |
| 339 | `.and()` | Atomik bitsel VE uygular. |
| 340 | `.compareExchange()` | Beklenen eşitse atomik değer değiştirir. |
| 341 | `.exchange()` | Atomik değiştirir; önceki değeri verir. |
| 342 | `.isLockFree()` | Belirtilen bayt işlemi kilitsiz mi? |
| 343 | `.load()` | Elemanı atomik olarak okur. |
| 344 | `.notify()` | Bekleyen yürütmeleri uyandırır. |
| 345 | `.or()` | Atomik bitsel VEYA uygular. |
| 346 | `.store()` | Elemanı atomik olarak yazar. |
| 347 | `.sub()` | Atomik çıkarma yapar. |
| 348 | `.wait()` | Değer değişimini engelleyerek bekler. |
| 349 | `.waitAsync()` | Atomik beklemeyi asenkron hazırlar. |
| 350 | `.xor()` | Atomik özel VEYA uygular. |

### console

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 351 | `.assert()` | Koşul yanlışsa tanılama mesajı yazar. |
| 352 | `.clear()` | Desteklenen ortamda konsolu temizler. |
| 353 | `.count()` | Etikete ait çağrı sayısını artırır. |
| 354 | `.countReset()` | Etiketin çağrı sayacını sıfırlar. |
| 355 | `.debug()` | Hata ayıklama düzeyinde mesaj yazar. |
| 356 | `.dir()` | Nesneyi incelenebilir biçimde gösterir. |
| 357 | `.dirxml()` | Nesneyi ortama göre ağaç biçiminde gösterir. |
| 358 | `.error()` | Hata düzeyinde mesaj yazar. |
| 359 | `.group()` | Girintili konsol grubu başlatır. |
| 360 | `.groupCollapsed()` | Daraltılmış konsol grubu başlatır. |
| 361 | `.groupEnd()` | Geçerli konsol grubunu kapatır. |
| 362 | `.info()` | Bilgi düzeyinde mesaj yazar. |
| 363 | `.log()` | Konsola mesaj yazar. |
| 364 | `.table()` | Veriyi tablo biçiminde gösterir. |
| 365 | `.time()` | Etiketli süre ölçümü başlatır. |
| 366 | `.timeEnd()` | Süre ölçümünü bitirip sonucu yazar. |
| 367 | `.timeLog()` | Ölçüm sürerken geçen süreyi yazar. |
| 368 | `.trace()` | Çağrı yığınını gösterir. |
| 369 | `.warn()` | Uyarı düzeyinde mesaj yazar. |

### Set

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 370 | `.union()` | İki kümenin birleşimini yeni küme yapar. |
| 371 | `.intersection()` | Kümelerin ortak değerlerini verir. |
| 372 | `.difference()` | İlk kümede olup diğerinde olmayanları verir. |
| 373 | `.symmetricDifference()` | Yalnızca bir kümede bulunanları verir. |
| 374 | `.isSubsetOf()` | Küme diğerinin alt kümesi mi? |
| 375 | `.isSupersetOf()` | Küme diğerinin üst kümesi mi? |
| 376 | `.isDisjointFrom()` | Kümelerin ortak değeri yok mu? |

### Sayı, işlev ve hata nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 377 | `.Number.toLocaleString()` | Sayıyı yerel kurallarla metne çevirir. |
| 378 | `.Number.toString()` | Sayıyı seçilen tabanda metne çevirir. |
| 379 | `.Number.valueOf()` | İlkel sayı değerini verir. |
| 380 | `.Function.toString()` | İşlevin metin gösterimini verir. |
| 381 | `.Error.toString()` | Hata adı ve mesajını birleştirir. |

### Uint8Array

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 382 | `.toLocaleString()` | Sayıları yerel kurallarla metne çevirir. |
| 383 | `.some()` | En az bir sayı koşulu sağlıyor mu? |
| 384 | `.sort()` | Türlenmiş diziyi sayısal sıralar. |
| 385 | `.values()` | Sayısal öğeleri yineler. |
| 386 | `.findLast()` | Koşulu sağlayan son sayıyı bulur. |
| 387 | `.findLastIndex()` | Koşulu sağlayan son konumu bulur. |
| 388 | `.toReversed()` | Ters sıralı yeni türlenmiş dizi üretir. |
| 389 | `.toSorted()` | Sıralanmış yeni türlenmiş dizi üretir. |
| 390 | `.with()` | Tek değeri değiştirilmiş kopya üretir. |

### SharedArrayBuffer

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 391 | `.slice()` | Paylaşılan belleğin bölümünü kopyalar. |
| 392 | `.grow()` | Büyüyebilir paylaşılan belleği genişletir. |

### Iterator

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 393 | `.from() [statik]` | Yineleyiciyi yardımcı metotlarla sarar. |
| 394 | `.map()` | Öğeleri tembel olarak dönüştürür. |
| 395 | `.filter()` | Koşulu sağlayan öğeleri tembel seçer. |
| 396 | `.take()` | İlk n öğeyi tembel olarak alır. |
| 397 | `.drop()` | İlk n öğeyi atlar. |
| 398 | `.flatMap()` | Dönüştürür ve bir düzey açar. |
| 399 | `.reduce()` | Yineleyiciden birikimli sonuç hesaplar. |
| 400 | `.toArray()` | Kalan öğeleri diziye toplar. |

<a id="bolum-05"></a>
## Bölüm 05: Asenkron işlemler, ağ ve akış API'leri


### Promise

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 401 | `.all() [statik]` | Bütün sonuçları bekler; ilk hatada reddeder. |
| 402 | `.allSettled() [statik]` | Başarı ve hata sonuçlarının hepsini bekler. |
| 403 | `.any() [statik]` | İlk başarılı sonucu bekler. |
| 404 | `.race() [statik]` | İlk sonuçlanan Promise'i izler. |
| 405 | `.resolve() [statik]` | Değeri çözümlenen Promise'e dönüştürür. |
| 406 | `.reject() [statik]` | Reddedilmiş Promise oluşturur. |
| 407 | `.withResolvers() [statik]` | Promise ve çözümleme işlevlerini verir. |
| 408 | `.then()` | Başarı veya hata işleyicisi ekler. |
| 409 | `.catch()` | Reddedilme işleyicisi ekler. |
| 410 | `.finally()` | Sonuçtan bağımsız son işlem ekler. |

### Genel işlevler

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 411 | `fetch()` | HTTP isteği gönderip Response bekler. |
| 412 | `queueMicrotask()` | Mikro görev kuyruğuna iş ekler. |
| 413 | `setTimeout()` | Gecikmeden sonra görev planlar. |
| 414 | `clearTimeout()` | Zaman aşımı görevini iptal eder. |
| 415 | `setInterval()` | Tekrarlanan görev planlar. |
| 416 | `clearInterval()` | Tekrarlanan görevi iptal eder. |
| 417 | `structuredClone()` | Desteklenen değerlerin derin kopyasını alır. |

### AbortController

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 418 | `.abort()` | Bağlı işlemlere iptal sinyali gönderir. |

### AbortSignal

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 419 | `.abort() [statik]` | Zaten iptal edilmiş sinyal oluşturur. |
| 420 | `.timeout() [statik]` | Süre sonunda iptal olan sinyal oluşturur. |
| 421 | `.any() [statik]` | İlk iptali izleyen birleşik sinyal üretir. |
| 422 | `.throwIfAborted()` | Sinyal iptalse nedenini fırlatır. |

### Fetch · Request / Response / Headers

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 423 | `.Request.arrayBuffer()` | İstek gövdesini ArrayBuffer olarak okur. |
| 424 | `.Request.blob()` | İstek gövdesini Blob olarak okur. |
| 425 | `.Request.clone()` | İstek nesnesini kopyalar. |
| 426 | `.Request.formData()` | İstek gövdesini form verisi olarak okur. |
| 427 | `.Request.json()` | İstek gövdesini JSON olarak çözer. |
| 428 | `.Request.text()` | İstek gövdesini metin olarak okur. |
| 429 | `.Response.error() [statik]` | Ağ hatasını temsil eden yanıt üretir. |
| 430 | `.Response.json() [statik]` | JSON gövdeli yanıt üretir. |
| 431 | `.Response.redirect() [statik]` | Yönlendirme yanıtı üretir. |
| 432 | `.Response.arrayBuffer()` | Yanıt gövdesini ArrayBuffer olarak okur. |
| 433 | `.Response.blob()` | Yanıt gövdesini Blob olarak okur. |
| 434 | `.Response.clone()` | Yanıt nesnesini kopyalar. |
| 435 | `.Response.formData()` | Yanıt gövdesini form verisi olarak okur. |
| 436 | `.Response.json()` | Yanıt gövdesini JSON olarak çözer. |
| 437 | `.Response.text()` | Yanıt gövdesini metin olarak okur. |
| 438 | `.Headers.append()` | Üstbilgiye ek değer ekler. |
| 439 | `.Headers.delete()` | Üstbilgiyi kaldırır. |
| 440 | `.Headers.entries()` | Üstbilgi çiftlerini yineler. |
| 441 | `.Headers.forEach()` | Her üstbilgi için işlev çalıştırır. |
| 442 | `.Headers.get()` | Üstbilgi değerini getirir. |
| 443 | `.Headers.has()` | Üstbilgi mevcut mu? |
| 444 | `.Headers.keys()` | Üstbilgi adlarını yineler. |
| 445 | `.Headers.set()` | Üstbilgi değerini değiştirir. |
| 446 | `.Headers.values()` | Üstbilgi değerlerini yineler. |

### FormData

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 447 | `.append()` | Forma alan veya dosya ekler. |
| 448 | `.delete()` | Adı verilen alanları kaldırır. |
| 449 | `.entries()` | Form alanı çiftlerini yineler. |
| 450 | `.forEach()` | Her form alanı için işlev çalıştırır. |
| 451 | `.get()` | Adın ilk değerini getirir. |
| 452 | `.getAll()` | Adın bütün değerlerini getirir. |
| 453 | `.has()` | Adı verilen alan mevcut mu? |
| 454 | `.keys()` | Alan adlarını yineler. |
| 455 | `.set()` | Alan değerlerini tek değerle değiştirir. |
| 456 | `.values()` | Alan değerlerini yineler. |

### URL

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 457 | `.canParse() [statik]` | Metin verilen tabanla URL olabilir mi? |
| 458 | `.createObjectURL() [statik]` | Blob için geçici nesne URL'si üretir. |
| 459 | `.revokeObjectURL() [statik]` | Nesne URL'sini serbest bırakır. |
| 460 | `.toJSON()` | URL'yi JSON için metne çevirir. |
| 461 | `.toString()` | URL'nin tam metnini verir. |

### URLSearchParams

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 462 | `.append()` | Sorguya anahtar-değer çifti ekler. |
| 463 | `.delete()` | Eşleşen sorgu parametresini siler. |
| 464 | `.entries()` | Parametre çiftlerini yineler. |
| 465 | `.forEach()` | Her parametre için işlev çalıştırır. |
| 466 | `.get()` | Parametrenin ilk değerini getirir. |
| 467 | `.getAll()` | Parametrenin bütün değerlerini getirir. |
| 468 | `.has()` | Parametrenin varlığını denetler. |
| 469 | `.keys()` | Parametre anahtarlarını yineler. |
| 470 | `.set()` | Parametrenin değerini ayarlar. |
| 471 | `.sort()` | Parametreleri anahtara göre sıralar. |
| 472 | `.toString()` | Kodlanmış sorgu metni üretir. |
| 473 | `.values()` | Parametre değerlerini yineler. |

### Blob

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 474 | `.arrayBuffer()` | Blob içeriğini ArrayBuffer olarak okur. |
| 475 | `.slice()` | Blob'un bir bölümünü alır. |
| 476 | `.stream()` | İçeriği okunabilir akış olarak verir. |
| 477 | `.text()` | İçeriği metin olarak okur. |

### Metin kodlama · TextEncoder / TextDecoder

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 478 | `.TextEncoder.encode()` | Metni UTF-8 baytlarına çevirir. |
| 479 | `.TextEncoder.encodeInto()` | UTF-8 baytlarını hedef diziye yazar. |
| 480 | `.TextDecoder.decode()` | Baytları metne dönüştürür. |

### Streams · akış nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 481 | `.ReadableStream.cancel()` | Okunabilir akışı iptal eder. |
| 482 | `.ReadableStream.getReader()` | Akışa özel okuyucu alır. |
| 483 | `.ReadableStream.pipeThrough()` | Akışı dönüşüm üzerinden geçirir. |
| 484 | `.ReadableStream.pipeTo()` | Akışı yazılabilir hedefe aktarır. |
| 485 | `.ReadableStream.tee()` | Okunabilir akışı iki kola ayırır. |
| 486 | `.ReadReader.cancel()` | Okunan akışı iptal eder. |
| 487 | `.ReadReader.read()` | Sonraki veri parçasını bekler. |
| 488 | `.ReadReader.releaseLock()` | Okuyucunun akış kilidini bırakır. |
| 489 | `.WritableStream.abort()` | Yazılabilir akışı hatayla durdurur. |
| 490 | `.WritableStream.close()` | Yazılabilir akışı kapatır. |
| 491 | `.WritableStream.getWriter()` | Akışa özel yazıcı alır. |
| 492 | `.WriteWriter.abort()` | Yazılan akışı hatayla durdurur. |
| 493 | `.WriteWriter.close()` | Yazma işlemlerinden sonra kapatır. |
| 494 | `.WriteWriter.releaseLock()` | Yazıcının akış kilidini bırakır. |
| 495 | `.WriteWriter.write()` | Akışa veri parçası yazar. |
| 496 | `.TransformController.enqueue()` | Dönüşüm çıktısına parça ekler. |
| 497 | `.TransformController.error()` | Dönüşüm akışını hataya geçirir. |
| 498 | `.TransformController.terminate()` | Dönüşümü sonlandırır. |
| 499 | `.ReadController.close()` | Okunabilir akışı kapatır. |
| 500 | `.ReadController.enqueue()` | Okuma kuyruğuna veri ekler. |

<a id="bolum-06"></a>
## Bölüm 06: Tarayıcı: DOM, belge ve HTML öğeleri


### Document

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 501 | `.getElementById()` | Kimliği verilen öğeyi bulur. |
| 502 | `.getElementsByClassName()` | Sınıfa uyan canlı öğe koleksiyonu verir. |
| 503 | `.getElementsByTagName()` | Etiket adına göre canlı koleksiyon verir. |
| 504 | `.getElementsByName()` | name alanına göre canlı koleksiyon verir. |
| 505 | `.querySelector()` | CSS seçicisine uyan ilk öğeyi verir. |
| 506 | `.querySelectorAll()` | CSS seçicisine uyan sabit liste verir. |
| 507 | `.createElement()` | HTML öğesi oluşturur. |
| 508 | `.createElementNS()` | Ad alanıyla öğe oluşturur. |
| 509 | `.createTextNode()` | Metin düğümü oluşturur. |
| 510 | `.createComment()` | Yorum düğümü oluşturur. |
| 511 | `.createDocumentFragment()` | Geçici belge parçası oluşturur. |
| 512 | `.createAttribute()` | Öznitelik düğümü oluşturur. |
| 513 | `.createRange()` | Belge aralığı oluşturur. |
| 514 | `.createTreeWalker()` | Filtreli ağaç gezgini oluşturur. |
| 515 | `.createNodeIterator()` | Düğüm yineleyicisi oluşturur. |
| 516 | `.importNode()` | Başka belgedeki düğümü kopyalar. |
| 517 | `.adoptNode()` | Düğümü başka belgeden devralır. |
| 518 | `.elementFromPoint()` | Koordinattaki en üst öğeyi bulur. |
| 519 | `.elementsFromPoint()` | Koordinattaki öğeleri sırayla verir. |
| 520 | `.getSelection()` | Belgedeki metin seçimini getirir. |
| 521 | `.hasFocus()` | Belgenin odağı var mı? |
| 522 | `.exitFullscreen()` | Tam ekran modundan çıkar. |

### Node

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 523 | `.appendChild()` | Alt düğümü sona ekler veya taşır. |
| 524 | `.cloneNode()` | Düğümün kopyasını oluşturur. |
| 525 | `.compareDocumentPosition()` | Düğümlerin belge sırasını karşılaştırır. |
| 526 | `.contains()` | Düğümün alt ağacında bulunuyor mu? |
| 527 | `.getRootNode()` | Düğümün kökünü bulur. |
| 528 | `.hasChildNodes()` | Alt düğüm var mı? |
| 529 | `.insertBefore()` | Düğümü başka alt düğümün önüne ekler. |
| 530 | `.isEqualNode()` | Yapısal düğüm eşitliğini kontrol eder. |
| 531 | `.isSameNode()` | Aynı düğüm nesnesi mi? |
| 532 | `.normalize()` | Bitişik metin düğümlerini birleştirir. |
| 533 | `.removeChild()` | Alt düğümü çıkarır. |
| 534 | `.replaceChild()` | Alt düğümü başka düğümle değiştirir. |
| 535 | `.lookupNamespaceURI()` | Önekin ad alanı URI'sini bulur. |
| 536 | `.lookupPrefix()` | Ad alanının önekini bulur. |
| 537 | `.isDefaultNamespace()` | URI varsayılan ad alanı mı? |

### Element

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 538 | `.after()` | Öğenin arkasına içerik ekler. |
| 539 | `.before()` | Öğenin önüne içerik ekler. |
| 540 | `.append()` | İçeriği alt öğelerin sonuna ekler. |
| 541 | `.prepend()` | İçeriği alt öğelerin başına ekler. |
| 542 | `.remove()` | Öğeyi belgeden kaldırır. |
| 543 | `.replaceWith()` | Öğeyi verilen içerikle değiştirir. |
| 544 | `.replaceChildren()` | Bütün alt düğümleri değiştirir. |
| 545 | `.closest()` | Kendisi dahil en yakın eşleşeni bulur. |
| 546 | `.matches()` | CSS seçicisiyle eşleşiyor mu? |
| 547 | `.querySelector()` | Alt ağaçta ilk CSS eşleşmesini bulur. |
| 548 | `.querySelectorAll()` | Alt ağaçta CSS eşleşmelerini listeler. |
| 549 | `.getAttribute()` | Özniteliğin metin değerini getirir. |
| 550 | `.getAttributeNames()` | Öznitelik adlarını listeler. |
| 551 | `.getAttributeNS()` | Ad alanıyla öznitelik getirir. |
| 552 | `.hasAttribute()` | Belirtilen öznitelik mevcut mu? |
| 553 | `.hasAttributes()` | Herhangi bir öznitelik var mı? |
| 554 | `.hasAttributeNS()` | Ad alanındaki öznitelik mevcut mu? |
| 555 | `.setAttribute()` | Öznitelik değerini ayarlar. |
| 556 | `.setAttributeNS()` | Ad alanıyla öznitelik ayarlar. |
| 557 | `.removeAttribute()` | Özniteliği kaldırır. |
| 558 | `.removeAttributeNS()` | Ad alanındaki özniteliği kaldırır. |
| 559 | `.toggleAttribute()` | Mantıksal özniteliğin varlığını değiştirir. |
| 560 | `.getBoundingClientRect()` | Görünüm alanına göre sınırları verir. |
| 561 | `.getClientRects()` | Düzen kutularının sınırlarını verir. |
| 562 | `.insertAdjacentElement()` | Belirtilen komşu konuma öğe ekler. |
| 563 | `.insertAdjacentHTML()` | Komşu konuma HTML ayrıştırarak ekler. |
| 564 | `.insertAdjacentText()` | Komşu konuma metin ekler. |
| 565 | `.scroll()` | Kaydırma konumunu ayarlar. |
| 566 | `.scrollBy()` | Belirtilen miktarda kaydırır. |
| 567 | `.scrollTo()` | Belirtilen konuma kaydırır. |
| 568 | `.scrollIntoView()` | Öğeyi görünür alana kaydırır. |
| 569 | `.attachShadow()` | Öğeye gölge DOM kökü bağlar. |
| 570 | `.requestFullscreen()` | Öğeyi tam ekrana geçirmeyi ister. |
| 571 | `.setPointerCapture()` | İşaretçi olaylarını öğeye yakalar. |
| 572 | `.releasePointerCapture()` | İşaretçi yakalamayı bırakır. |
| 573 | `.hasPointerCapture()` | İşaretçi bu öğe tarafından yakalanmış mı? |
| 574 | `.animate()` | Anahtar karelerle animasyon başlatır. |
| 575 | `.getAnimations()` | Öğeye ait animasyonları getirir. |

### HTMLElement

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 576 | `.click()` | Öğede tıklama davranışını tetikler. |
| 577 | `.focus()` | Öğeye klavye odağı verir. |
| 578 | `.blur()` | Öğenin odağını kaldırır. |

### DOMTokenList

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 579 | `.add()` | Sınıf benzeri belirteçler ekler. |
| 580 | `.remove()` | Belirteçleri kaldırır. |
| 581 | `.contains()` | Belirteç mevcut mu? |
| 582 | `.toggle()` | Belirteci ekler veya kaldırır. |
| 583 | `.replace()` | Belirteci başka belirteçle değiştirir. |
| 584 | `.item()` | Konumdaki belirteci alır. |
| 585 | `.entries()` | İndis ve belirteç çiftlerini yineler. |
| 586 | `.forEach()` | Her belirteç için işlev çalıştırır. |
| 587 | `.keys()` | Belirteç indislerini yineler. |
| 588 | `.values()` | Belirteç değerlerini yineler. |

### EventTarget

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 589 | `.addEventListener()` | Olay dinleyicisi ekler. |
| 590 | `.removeEventListener()` | Olay dinleyicisini kaldırır. |
| 591 | `.dispatchEvent()` | Nesne üzerinde olay gönderir. |

### Event

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 592 | `.preventDefault()` | İptal edilebilen varsayılanı engeller. |
| 593 | `.stopPropagation()` | Olayın diğer düğümlere yayılmasını keser. |
| 594 | `.stopImmediatePropagation()` | Sonraki dinleyicileri ve yayılmayı keser. |
| 595 | `.composedPath()` | Olayın geçtiği hedef yolunu verir. |

### HTMLFormElement

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 596 | `.checkValidity()` | Form alanlarının geçerliliğini sınar. |
| 597 | `.reportValidity()` | Geçersiz alanları kullanıcıya bildirir. |
| 598 | `.requestSubmit()` | Doğrulamalı form gönderimi ister. |
| 599 | `.reset()` | Formu başlangıç değerlerine döndürür. |
| 600 | `.submit()` | Doğrulamayı atlayarak formu gönderir. |

<a id="bolum-07"></a>
## Bölüm 07: Tarayıcı: Canvas, çizim ve görseller


### CanvasRenderingContext2D

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 601 | `.save()` | Çizim durumunu yığına kaydeder. |
| 602 | `.restore()` | Kaydedilmiş çizim durumunu geri alır. |
| 603 | `.reset()` | Bağlamı varsayılan durumuna sıfırlar. |
| 604 | `.scale()` | Koordinat sistemini ölçekler. |
| 605 | `.rotate()` | Koordinat sistemini döndürür. |
| 606 | `.translate()` | Koordinat başlangıcını taşır. |
| 607 | `.transform()` | Geçerli dönüşümle matrisi çarpar. |
| 608 | `.setTransform()` | Dönüşüm matrisini değiştirir. |
| 609 | `.resetTransform()` | Dönüşümü birim matrise çevirir. |
| 610 | `.getTransform()` | Geçerli dönüşüm matrisini getirir. |
| 611 | `.createLinearGradient()` | Doğrusal renk geçişi oluşturur. |
| 612 | `.createRadialGradient()` | Radyal renk geçişi oluşturur. |
| 613 | `.createConicGradient()` | Konik renk geçişi oluşturur. |
| 614 | `.createPattern()` | Görselden tekrarlı desen oluşturur. |
| 615 | `.clearRect()` | Dikdörtgen alanı saydamlaştırır. |
| 616 | `.fillRect()` | Dolu dikdörtgen çizer. |
| 617 | `.strokeRect()` | Dikdörtgen kenarlığı çizer. |
| 618 | `.beginPath()` | Yeni çizim yolu başlatır. |
| 619 | `.closePath()` | Geçerli alt yolu kapatır. |
| 620 | `.moveTo()` | Yolun kalem konumunu taşır. |
| 621 | `.lineTo()` | Konuma düz çizgi ekler. |
| 622 | `.bezierCurveTo()` | Kübik Bézier eğrisi ekler. |
| 623 | `.quadraticCurveTo()` | İkinci dereceden Bézier eğrisi ekler. |
| 624 | `.arc()` | Dairesel yay ekler. |
| 625 | `.arcTo()` | Teğetli dairesel yay ekler. |
| 626 | `.ellipse()` | Eliptik yay ekler. |
| 627 | `.rect()` | Dikdörtgen yol ekler. |
| 628 | `.roundRect()` | Yuvarlatılmış dikdörtgen yol ekler. |
| 629 | `.fill()` | Yolun içini doldurur. |
| 630 | `.stroke()` | Yolun kenarını çizer. |
| 631 | `.clip()` | Çizim alanını yolla sınırlar. |
| 632 | `.isPointInPath()` | Nokta yolun içinde mi? |
| 633 | `.isPointInStroke()` | Nokta çizgi alanında mı? |
| 634 | `.fillText()` | Dolu metin çizer. |
| 635 | `.strokeText()` | Metnin dış çizgilerini çizer. |
| 636 | `.measureText()` | Metnin ölçülerini hesaplar. |
| 637 | `.drawImage()` | Görseli veya video karesini çizer. |
| 638 | `.createImageData()` | Boş piksel verisi oluşturur. |
| 639 | `.getImageData()` | Tuvalden piksel verisi okur. |
| 640 | `.putImageData()` | Tuvale doğrudan piksel verisi yazar. |
| 641 | `.setLineDash()` | Kesikli çizgi desenini ayarlar. |
| 642 | `.getLineDash()` | Kesikli çizgi desenini getirir. |

### Canvas · renk ve desen

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 643 | `.CanvasGradient.addColorStop()` | Renk geçişine renk durağı ekler. |
| 644 | `.CanvasPattern.setTransform()` | Desenin dönüşüm matrisini ayarlar. |

### Canvas ve bitmap nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 645 | `.HTMLCanvasElement.getContext()` | İstenen çizim bağlamını getirir. |
| 646 | `.HTMLCanvasElement.toDataURL()` | Tuvali veri URL'sine dönüştürür. |
| 647 | `.HTMLCanvasElement.toBlob()` | Tuvali Blob olarak kodlar. |
| 648 | `.HTMLCanvasElement.captureStream()` | Tuvalden canlı medya akışı üretir. |
| 649 | `.HTMLCanvasElement.transferControlToOffscreen()` | Tuval denetimini OffscreenCanvas'a taşır. |
| 650 | `.OffscreenCanvas.getContext()` | Ekran dışı çizim bağlamı alır. |
| 651 | `.OffscreenCanvas.convertToBlob()` | Ekran dışı tuvali Blob'a çevirir. |
| 652 | `.OffscreenCanvas.transferToImageBitmap()` | Son çizimi ImageBitmap olarak aktarır. |
| 653 | `.ImageBitmap.close()` | Görselin kaynaklarını serbest bırakır. |

### Genel işlevler

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 654 | `createImageBitmap()` | Kaynak görselden bitmap oluşturur. |

### Path2D

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 655 | `.addPath()` | Başka yolu mevcut yola ekler. |
| 656 | `.closePath()` | Geçerli alt yolu kapatır. |
| 657 | `.moveTo()` | Yolun kalem konumunu taşır. |
| 658 | `.lineTo()` | Yola düz çizgi ekler. |
| 659 | `.bezierCurveTo()` | Yola kübik eğri ekler. |
| 660 | `.quadraticCurveTo()` | Yola ikinci dereceden eğri ekler. |
| 661 | `.arc()` | Yola dairesel yay ekler. |
| 662 | `.arcTo()` | Yola teğetli yay ekler. |
| 663 | `.ellipse()` | Yola eliptik yay ekler. |
| 664 | `.rect()` | Yola dikdörtgen ekler. |
| 665 | `.roundRect()` | Yola yuvarlatılmış dikdörtgen ekler. |

### DOMMatrix · matris işlemleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 666 | `.multiplySelf()` | Matrisi yerinde sağdan çarpar. |
| 667 | `.preMultiplySelf()` | Matrisi yerinde soldan çarpar. |
| 668 | `.translateSelf()` | Matrise yerinde öteleme ekler. |
| 669 | `.scaleSelf()` | Matrise yerinde ölçekleme ekler. |
| 670 | `.scale3dSelf()` | Üç boyutta ortak ölçek uygular. |
| 671 | `.rotateSelf()` | Matrise yerinde dönme ekler. |
| 672 | `.rotateFromVectorSelf()` | Vektör açısına göre yerinde döndürür. |
| 673 | `.rotateAxisAngleSelf()` | Eksen ve açıyla yerinde döndürür. |
| 674 | `.skewXSelf()` | X yönünde yerinde eğme uygular. |
| 675 | `.skewYSelf()` | Y yönünde yerinde eğme uygular. |
| 676 | `.invertSelf()` | Matrisin tersini yerinde alır. |
| 677 | `.setMatrixValue()` | CSS dönüşüm metninden matrisi ayarlar. |
| 678 | `.translate()` | Ötelenmiş yeni matris üretir. |
| 679 | `.scale()` | Ölçeklenmiş yeni matris üretir. |
| 680 | `.scale3d()` | Üç boyutta ölçeklenmiş matris üretir. |
| 681 | `.rotate()` | Döndürülmüş yeni matris üretir. |
| 682 | `.rotateFromVector()` | Vektör açısıyla döndürülmüş matris üretir. |
| 683 | `.rotateAxisAngle()` | Eksen ve açıyla döndürülmüş matris üretir. |
| 684 | `.skewX()` | X yönünde eğilmiş matris üretir. |
| 685 | `.skewY()` | Y yönünde eğilmiş matris üretir. |
| 686 | `.multiply()` | Matris çarpımından yeni matris üretir. |
| 687 | `.flipX()` | X yönünü yansıtan matris üretir. |
| 688 | `.flipY()` | Y yönünü yansıtan matris üretir. |
| 689 | `.inverse()` | Ters matris üretir. |
| 690 | `.transformPoint()` | Noktaya matris dönüşümü uygular. |
| 691 | `.toFloat32Array()` | Matrisi 32 bit kayan diziye çevirir. |
| 692 | `.toFloat64Array()` | Matrisi 64 bit kayan diziye çevirir. |
| 693 | `.toString()` | Matrisi CSS dönüşüm metnine çevirir. |
| 694 | `.toJSON()` | Matris bileşenlerini nesne olarak verir. |

### Nokta ve dikdörtgen nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 695 | `.DOMPointReadOnly.matrixTransform()` | Noktayı matrisle dönüştürür. |
| 696 | `.DOMPointReadOnly.toJSON()` | Nokta bileşenlerini nesne olarak verir. |
| 697 | `.DOMRectReadOnly.toJSON()` | Dikdörtgen alanlarını nesne olarak verir. |

### HTMLImageElement

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 698 | `.decode()` | Görselin çözümlenmesini bekler. |

### window

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 699 | `.requestAnimationFrame()` | Sonraki çizim öncesine görev planlar. |
| 700 | `.cancelAnimationFrame()` | Planlanan çizim görevini iptal eder. |

<a id="bolum-08"></a>
## Bölüm 08: Tarayıcı: depolama, performans ve iletişim


### Storage

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 701 | `.getItem()` | Depodan anahtarın değerini okur. |
| 702 | `.setItem()` | Depoya anahtar-değer çifti yazar. |
| 703 | `.removeItem()` | Anahtarı depodan kaldırır. |
| 704 | `.clear()` | Depoyu tamamen boşaltır. |
| 705 | `.key()` | Konumdaki anahtarı getirir. |

### CacheStorage

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 706 | `.open()` | Adlandırılmış önbelleği açar veya oluşturur. |
| 707 | `.has()` | Adlandırılmış önbellek var mı? |
| 708 | `.delete()` | Adlandırılmış önbelleği kaldırır. |
| 709 | `.keys()` | Önbellek adlarını listeler. |
| 710 | `.match()` | Önbelleklerde isteğe uygun yanıt arar. |

### Cache

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 711 | `.add()` | İstek sonucunu indirip önbelleğe ekler. |
| 712 | `.addAll()` | İstek sonuçlarını topluca önbelleğe ekler. |
| 713 | `.put()` | İstek ve yanıtı önbelleğe yazar. |
| 714 | `.match()` | Önbellekte ilk uygun yanıtı bulur. |
| 715 | `.matchAll()` | Önbellekte uygun bütün yanıtları bulur. |
| 716 | `.delete()` | Eşleşen önbellek kaydını siler. |
| 717 | `.keys()` | Önbellekteki istekleri listeler. |

### IndexedDB · veritabanı nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 718 | `.Factory.open()` | IndexedDB veritabanını açar. |
| 719 | `.Factory.deleteDatabase()` | IndexedDB veritabanını siler. |
| 720 | `.Factory.cmp()` | İki IndexedDB anahtarını karşılaştırır. |
| 721 | `.Database.createObjectStore()` | Sürüm yükseltmede nesne deposu oluşturur. |
| 722 | `.Database.deleteObjectStore()` | Sürüm yükseltmede nesne deposunu siler. |
| 723 | `.Database.transaction()` | Veritabanı işlemi başlatır. |
| 724 | `.Database.close()` | Veritabanı bağlantısını kapatır. |
| 725 | `.Transaction.objectStore()` | İşlemdeki nesne deposunu getirir. |
| 726 | `.Transaction.abort()` | Veritabanı işlemini geri alır. |
| 727 | `.Transaction.commit()` | İşlemin tamamlanmasını başlatır. |
| 728 | `.ObjectStore.add()` | Yeni kayıt ekler; mevcut anahtarda hata verir. |
| 729 | `.ObjectStore.put()` | Kayıt ekler veya günceller. |
| 730 | `.ObjectStore.get()` | Anahtarla ilk kaydı getirir. |
| 731 | `.ObjectStore.getAll()` | Eşleşen kayıtları getirir. |
| 732 | `.ObjectStore.getKey()` | Eşleşen ilk anahtarı getirir. |
| 733 | `.ObjectStore.getAllKeys()` | Eşleşen anahtarları getirir. |
| 734 | `.ObjectStore.delete()` | Anahtar veya aralıktaki kayıtları siler. |
| 735 | `.ObjectStore.clear()` | Depodaki bütün kayıtları siler. |
| 736 | `.ObjectStore.count()` | Eşleşen kayıt sayısını verir. |
| 737 | `.ObjectStore.createIndex()` | Sürüm yükseltmede indeks oluşturur. |
| 738 | `.ObjectStore.deleteIndex()` | Sürüm yükseltmede indeksi siler. |
| 739 | `.ObjectStore.index()` | Adlandırılmış indeksi getirir. |
| 740 | `.ObjectStore.openCursor()` | Kayıt gezgini açar. |
| 741 | `.ObjectStore.openKeyCursor()` | Anahtar gezgini açar. |
| 742 | `.Index.get()` | İndeksten ilk kayıt değerini getirir. |
| 743 | `.Index.getAll()` | İndeksten eşleşen değerleri getirir. |
| 744 | `.Index.getKey()` | İndeksten ilk asıl anahtarı getirir. |
| 745 | `.Index.getAllKeys()` | İndeksten asıl anahtarları getirir. |
| 746 | `.Index.count()` | İndeksteki eşleşmeleri sayar. |
| 747 | `.Index.openCursor()` | İndeks üzerinde kayıt gezgini açar. |
| 748 | `.Index.openKeyCursor()` | İndeks üzerinde anahtar gezgini açar. |
| 749 | `.Cursor.advance()` | Gezgini belirtilen kayıt sayısı ilerletir. |
| 750 | `.Cursor.continue()` | Gezgini sonraki uygun kayda ilerletir. |
| 751 | `.Cursor.continuePrimaryKey()` | İndeks ve asıl anahtara göre ilerler. |
| 752 | `.Cursor.delete()` | Gezginin geçerli kaydını siler. |
| 753 | `.Cursor.update()` | Gezginin geçerli kaydını günceller. |
| 754 | `.KeyRange.only() [statik]` | Tek anahtarı içeren aralık oluşturur. |
| 755 | `.KeyRange.bound() [statik]` | Alt ve üst sınırlı aralık oluşturur. |
| 756 | `.KeyRange.lowerBound() [statik]` | Alt sınırlı anahtar aralığı oluşturur. |
| 757 | `.KeyRange.upperBound() [statik]` | Üst sınırlı anahtar aralığı oluşturur. |
| 758 | `.KeyRange.includes()` | Anahtarın aralıkta olduğunu sınar. |

### Performans ölçümü ve gözlem

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 759 | `.Performance.now()` | Yüksek çözünürlüklü zaman sayacı verir. |
| 760 | `.Performance.mark()` | Adlandırılmış zaman işareti ekler. |
| 761 | `.Performance.measure()` | İşaretler arası süre kaydı üretir. |
| 762 | `.Performance.clearMarks()` | Zaman işaretlerini temizler. |
| 763 | `.Performance.clearMeasures()` | Süre kayıtlarını temizler. |
| 764 | `.Performance.getEntries()` | Performans kayıtlarını getirir. |
| 765 | `.Performance.getEntriesByName()` | Ada göre performans kayıtları getirir. |
| 766 | `.Performance.getEntriesByType()` | Türe göre performans kayıtları getirir. |
| 767 | `.Performance.clearResourceTimings()` | Kaynak zamanlama kayıtlarını temizler. |
| 768 | `.Performance.setResourceTimingBufferSize()` | Kaynak kayıt tamponunun boyutunu ayarlar. |
| 769 | `.Performance.toJSON()` | Performans nesnesini sade nesne yapar. |
| 770 | `.PerformanceObserver.observe()` | Seçilen performans kayıtlarını izler. |
| 771 | `.PerformanceObserver.disconnect()` | Performans izlemeyi durdurur. |
| 772 | `.PerformanceObserver.takeRecords()` | Bekleyen performans kayıtlarını alır. |
| 773 | `.EntryList.getEntries()` | Gözlenen kayıtların hepsini alır. |
| 774 | `.EntryList.getEntriesByName()` | Gözlenen kayıtları ada göre seçer. |
| 775 | `.EntryList.getEntriesByType()` | Gözlenen kayıtları türe göre seçer. |

### DOM gözlemcileri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 776 | `.MutationObserver.observe()` | DOM değişikliklerini izler. |
| 777 | `.MutationObserver.disconnect()` | DOM izlemeyi durdurur. |
| 778 | `.MutationObserver.takeRecords()` | Bekleyen DOM değişimlerini alır. |
| 779 | `.ResizeObserver.observe()` | Öğenin boyut değişimini izler. |
| 780 | `.ResizeObserver.unobserve()` | Öğenin boyut izlemesini durdurur. |
| 781 | `.ResizeObserver.disconnect()` | Bütün boyut izlemelerini durdurur. |
| 782 | `.IntersectionObserver.observe()` | Öğenin görünürlük kesişimini izler. |
| 783 | `.IntersectionObserver.unobserve()` | Öğenin kesişim izlemesini durdurur. |
| 784 | `.IntersectionObserver.disconnect()` | Bütün kesişim izlemelerini durdurur. |
| 785 | `.IntersectionObserver.takeRecords()` | Bekleyen kesişim kayıtlarını alır. |

### Worker ve mesajlaşma nesneleri

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 786 | `.Worker.postMessage()` | Worker'a mesaj gönderir. |
| 787 | `.Worker.terminate()` | Worker yürütmesini sonlandırır. |
| 788 | `.MessagePort.postMessage()` | Port üzerinden mesaj gönderir. |
| 789 | `.MessagePort.start()` | Porta mesaj teslimini başlatır. |
| 790 | `.MessagePort.close()` | Mesaj portunu kapatır. |
| 791 | `.BroadcastChannel.postMessage()` | Aynı adlı kanala mesaj yayınlar. |
| 792 | `.BroadcastChannel.close()` | Yayın kanalını kapatır. |
| 793 | `.WebSocket.send()` | Açık bağlantıda veri gönderir. |
| 794 | `.WebSocket.close()` | WebSocket bağlantısını kapatır. |
| 795 | `.EventSource.close()` | Sunucu olay akışını kapatır. |

### History

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 796 | `.back()` | Geçmişte bir kayıt geri gider. |
| 797 | `.forward()` | Geçmişte bir kayıt ileri gider. |
| 798 | `.go()` | Geçmişte belirtilen miktarda ilerler. |
| 799 | `.pushState()` | Geçmişe sayfa yüklemeden kayıt ekler. |
| 800 | `.replaceState()` | Geçerli geçmiş kaydını değiştirir. |

<a id="bolum-09"></a>
## Bölüm 09: Node.js: dosyalar, yollar ve işletim sistemi


### fs

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 801 | `.access()` | Dosya erişimini geri çağırımla denetler. |
| 802 | `.appendFile()` | Dosyanın sonuna veri ekler. |
| 803 | `.chmod()` | Dosya izinlerini değiştirir. |
| 804 | `.chown()` | Dosyanın sahip ve grubunu değiştirir. |
| 805 | `.close()` | Dosya tanımlayıcısını kapatır. |
| 806 | `.copyFile()` | Dosyayı başka yola kopyalar. |
| 807 | `.cp()` | Dosya veya klasör ağacını kopyalar. |
| 808 | `.createReadStream()` | Dosyadan okunabilir akış açar. |
| 809 | `.createWriteStream()` | Dosyaya yazılabilir akış açar. |
| 810 | `.existsSync()` | Yolun varlığını eşzamanlı denetler. |
| 811 | `.fchmod()` | Açık dosyanın izinlerini değiştirir. |
| 812 | `.fchown()` | Açık dosyanın sahipliğini değiştirir. |
| 813 | `.fdatasync()` | Dosya veri değişikliklerini diske aktarır. |
| 814 | `.fstat()` | Açık dosyanın metaverisini getirir. |
| 815 | `.fsync()` | Dosya değişikliklerini diske eşler. |
| 816 | `.ftruncate()` | Açık dosyanın uzunluğunu değiştirir. |
| 817 | `.futimes()` | Açık dosyanın zamanlarını değiştirir. |
| 818 | `.link()` | Sabit dosya bağlantısı oluşturur. |
| 819 | `.lstat()` | Bağlantıyı izlemeden metaveri okur. |
| 820 | `.mkdir()` | Klasör oluşturur. |
| 821 | `.mkdtemp()` | Benzersiz geçici klasör oluşturur. |
| 822 | `.open()` | Dosyayı açıp tanımlayıcı verir. |
| 823 | `.opendir()` | Klasör okuma nesnesi açar. |
| 824 | `.read()` | Açık dosyadan tampona veri okur. |
| 825 | `.readdir()` | Klasör öğelerini okur. |
| 826 | `.readFile()` | Dosyanın bütün içeriğini okur. |
| 827 | `.readlink()` | Sembolik bağlantının hedefini okur. |
| 828 | `.realpath()` | Bağlantıları çözümlenmiş yol verir. |
| 829 | `.rename()` | Dosya veya klasörü yeniden adlandırır. |
| 830 | `.rm()` | Dosya veya klasörü kaldırır. |
| 831 | `.rmdir()` | Boş klasörü kaldırır. |
| 832 | `.stat()` | Dosya metaverisini getirir. |
| 833 | `.statfs()` | Dosya sistemi istatistiklerini getirir. |
| 834 | `.symlink()` | Sembolik bağlantı oluşturur. |
| 835 | `.truncate()` | Dosyanın uzunluğunu değiştirir. |
| 836 | `.unlink()` | Dosya adını dosya sisteminden kaldırır. |
| 837 | `.unwatchFile()` | Dosya değişikliği yoklamasını durdurur. |
| 838 | `.utimes()` | Dosya erişim ve değişim zamanını ayarlar. |
| 839 | `.watch()` | Dosya veya klasör değişikliklerini izler. |
| 840 | `.watchFile()` | Dosya değişikliklerini yoklayarak izler. |
| 841 | `.write()` | Açık dosyaya veri yazar. |
| 842 | `.writeFile()` | Dosyaya bütün içeriği yazar. |
| 843 | `.writev()` | Birden fazla tamponu dosyaya yazar. |
| 844 | `.readv()` | Dosyadan birden fazla tampona okur. |
| 845 | `.accessSync()` | Dosya erişimini eşzamanlı denetler. |
| 846 | `.appendFileSync()` | Dosyaya eşzamanlı veri ekler. |
| 847 | `.copyFileSync()` | Dosyayı eşzamanlı kopyalar. |
| 848 | `.mkdirSync()` | Klasörü eşzamanlı oluşturur. |
| 849 | `.readFileSync()` | Dosyayı eşzamanlı okur. |
| 850 | `.writeFileSync()` | Dosyayı eşzamanlı yazar. |
| 851 | `.readdirSync()` | Klasör öğelerini eşzamanlı okur. |
| 852 | `.renameSync()` | Yolu eşzamanlı yeniden adlandırır. |
| 853 | `.rmSync()` | Dosya veya klasörü eşzamanlı kaldırır. |
| 854 | `.statSync()` | Metaveriyi eşzamanlı getirir. |

### fs.promises

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 855 | `.access()` | Promise ile erişim denetler. |
| 856 | `.appendFile()` | Promise ile dosyaya veri ekler. |
| 857 | `.copyFile()` | Promise ile dosya kopyalar. |
| 858 | `.cp()` | Promise ile klasör ağacı kopyalar. |
| 859 | `.mkdir()` | Promise ile klasör oluşturur. |
| 860 | `.mkdtemp()` | Promise ile geçici klasör oluşturur. |
| 861 | `.open()` | Promise ile FileHandle açar. |
| 862 | `.opendir()` | Promise ile klasör nesnesi açar. |
| 863 | `.readdir()` | Promise ile klasör öğelerini okur. |
| 864 | `.readFile()` | Promise ile dosya içeriğini okur. |
| 865 | `.readlink()` | Promise ile bağlantı hedefi okur. |
| 866 | `.realpath()` | Promise ile gerçek yolu çözümler. |
| 867 | `.rename()` | Promise ile yolu yeniden adlandırır. |
| 868 | `.rm()` | Promise ile dosya veya klasör kaldırır. |
| 869 | `.stat()` | Promise ile dosya metaverisi getirir. |
| 870 | `.unlink()` | Promise ile dosya bağlantısını siler. |
| 871 | `.writeFile()` | Promise ile dosya içeriğini yazar. |

### path

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 872 | `.basename()` | Yolun son bileşenini getirir. |
| 873 | `.dirname()` | Yolun klasör bölümünü getirir. |
| 874 | `.extname()` | Dosya uzantısını getirir. |
| 875 | `.format()` | Yol nesnesinden metin oluşturur. |
| 876 | `.isAbsolute()` | Yol mutlak mı? |
| 877 | `.join()` | Yol bileşenlerini birleştirir. |
| 878 | `.normalize()` | Ayırıcı ve nokta bileşenlerini düzeltir. |
| 879 | `.parse()` | Yolu bileşen nesnesine ayırır. |
| 880 | `.relative()` | İki yol arasındaki göreli yolu verir. |
| 881 | `.resolve()` | Bileşenlerden mutlak yol çözümler. |
| 882 | `.toNamespacedPath()` | Windows ad alanı yoluna dönüştürür. |

### os

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 883 | `.arch()` | Çalışma zamanının işlemci mimarisini verir. |
| 884 | `.availableParallelism()` | Önerilen paralellik düzeyini verir. |
| 885 | `.cpus()` | Mantıksal işlemci bilgilerini getirir. |
| 886 | `.endianness()` | İşlemcinin bayt sırasını verir. |
| 887 | `.freemem()` | Boş sistem belleğini bayt verir. |
| 888 | `.homedir()` | Kullanıcının ev klasörünü getirir. |
| 889 | `.hostname()` | Makine adını getirir. |
| 890 | `.loadavg()` | Sistem yük ortalamalarını verir. |
| 891 | `.networkInterfaces()` | Ağ arayüzü adreslerini listeler. |
| 892 | `.platform()` | İşletim sistemi platformunu verir. |
| 893 | `.release()` | İşletim sistemi sürümünü verir. |
| 894 | `.tmpdir()` | Geçici dosya klasörünü verir. |
| 895 | `.totalmem()` | Toplam sistem belleğini bayt verir. |
| 896 | `.type()` | İşletim sistemi türünü verir. |
| 897 | `.uptime()` | Sistemin açık kalma süresini verir. |
| 898 | `.userInfo()` | Geçerli kullanıcı bilgisini verir. |
| 899 | `.version()` | İşletim sistemi sürüm metnini verir. |
| 900 | `.machine()` | Makinenin donanım türünü verir. |

<a id="bolum-10"></a>
## Bölüm 10: Node.js: Buffer, kriptografi ve olaylar


### Buffer

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 901 | `.alloc() [statik]` | Başlatılmış bayt tamponu oluşturur. |
| 902 | `.allocUnsafe() [statik]` | İçeriği başlatılmamış tampon ayırır. |
| 903 | `.allocUnsafeSlow() [statik]` | Havuz dışı başlatılmamış tampon ayırır. |
| 904 | `.byteLength() [statik]` | Metnin kodlanmış bayt uzunluğunu verir. |
| 905 | `.compare() [statik]` | İki tamponun bayt sırasını karşılaştırır. |
| 906 | `.concat() [statik]` | Tamponları yeni tampona birleştirir. |
| 907 | `.from() [statik]` | Metin, dizi veya bellekten tampon kurar. |
| 908 | `.isBuffer() [statik]` | Değer Buffer nesnesi mi? |
| 909 | `.isEncoding() [statik]` | Kodlama adı destekleniyor mu? |
| 910 | `.compare()` | Tampon bölümlerini karşılaştırır. |
| 911 | `.copy()` | Baytları başka tampona kopyalar. |
| 912 | `.equals()` | Tampon içerikleri eşit mi? |
| 913 | `.fill()` | Tamponu verilen değerle doldurur. |
| 914 | `.includes()` | Bayt veya alt dizi mevcut mu? |
| 915 | `.indexOf()` | İlk eşleşen bayt konumunu bulur. |
| 916 | `.lastIndexOf()` | Son eşleşen bayt konumunu bulur. |
| 917 | `.readBigInt64BE()` | Büyük uçlu işaretli 64 bit tamsayı okur. |
| 918 | `.readBigInt64LE()` | Küçük uçlu işaretli 64 bit tamsayı okur. |
| 919 | `.readBigUInt64BE()` | Büyük uçlu işaretsiz 64 bit tamsayı okur. |
| 920 | `.readBigUInt64LE()` | Küçük uçlu işaretsiz 64 bit tamsayı okur. |
| 921 | `.readDoubleBE()` | Büyük uçlu 64 bit kayan sayı okur. |
| 922 | `.readDoubleLE()` | Küçük uçlu 64 bit kayan sayı okur. |
| 923 | `.readFloatBE()` | Büyük uçlu 32 bit kayan sayı okur. |
| 924 | `.readFloatLE()` | Küçük uçlu 32 bit kayan sayı okur. |
| 925 | `.readInt8()` | İşaretli sekiz bit tamsayı okur. |
| 926 | `.readInt16BE()` | Büyük uçlu işaretli 16 bit sayı okur. |
| 927 | `.readInt16LE()` | Küçük uçlu işaretli 16 bit sayı okur. |
| 928 | `.readInt32BE()` | Büyük uçlu işaretli 32 bit sayı okur. |
| 929 | `.readInt32LE()` | Küçük uçlu işaretli 32 bit sayı okur. |
| 930 | `.readIntBE()` | Büyük uçlu değişken baytlı tamsayı okur. |
| 931 | `.readIntLE()` | Küçük uçlu değişken baytlı tamsayı okur. |
| 932 | `.readUInt8()` | İşaretsiz sekiz bit tamsayı okur. |
| 933 | `.readUInt16BE()` | Büyük uçlu işaretsiz 16 bit sayı okur. |
| 934 | `.readUInt16LE()` | Küçük uçlu işaretsiz 16 bit sayı okur. |
| 935 | `.readUInt32BE()` | Büyük uçlu işaretsiz 32 bit sayı okur. |
| 936 | `.readUInt32LE()` | Küçük uçlu işaretsiz 32 bit sayı okur. |
| 937 | `.readUIntBE()` | Büyük uçlu işaretsiz tamsayı okur. |
| 938 | `.readUIntLE()` | Küçük uçlu işaretsiz tamsayı okur. |
| 939 | `.subarray()` | Ortak bellekte alt tampon görünümü verir. |
| 940 | `.swap16()` | Her 16 bitlik grubun bayt sırasını değiştirir. |
| 941 | `.swap32()` | Her 32 bitlik grubun bayt sırasını değiştirir. |
| 942 | `.swap64()` | Her 64 bitlik grubun bayt sırasını değiştirir. |
| 943 | `.toJSON()` | Tamponu JSON uyumlu nesne yapar. |
| 944 | `.toString()` | Baytları belirtilen kodlamayla çözer. |
| 945 | `.write()` | Metni tampona kodlayarak yazar. |
| 946 | `.writeBigInt64BE()` | Büyük uçlu işaretli 64 bit tamsayı yazar. |
| 947 | `.writeBigInt64LE()` | Küçük uçlu işaretli 64 bit tamsayı yazar. |
| 948 | `.writeBigUInt64BE()` | Büyük uçlu işaretsiz 64 bit tamsayı yazar. |
| 949 | `.writeBigUInt64LE()` | Küçük uçlu işaretsiz 64 bit tamsayı yazar. |
| 950 | `.writeDoubleBE()` | Büyük uçlu 64 bit kayan sayı yazar. |
| 951 | `.writeDoubleLE()` | Küçük uçlu 64 bit kayan sayı yazar. |
| 952 | `.writeFloatBE()` | Büyük uçlu 32 bit kayan sayı yazar. |
| 953 | `.writeFloatLE()` | Küçük uçlu 32 bit kayan sayı yazar. |
| 954 | `.writeInt8()` | İşaretli sekiz bit tamsayı yazar. |
| 955 | `.writeInt16BE()` | Büyük uçlu işaretli 16 bit sayı yazar. |
| 956 | `.writeInt16LE()` | Küçük uçlu işaretli 16 bit sayı yazar. |
| 957 | `.writeInt32BE()` | Büyük uçlu işaretli 32 bit sayı yazar. |
| 958 | `.writeInt32LE()` | Küçük uçlu işaretli 32 bit sayı yazar. |
| 959 | `.writeUInt8()` | İşaretsiz sekiz bit tamsayı yazar. |
| 960 | `.writeUInt16BE()` | Büyük uçlu işaretsiz 16 bit sayı yazar. |
| 961 | `.writeUInt16LE()` | Küçük uçlu işaretsiz 16 bit sayı yazar. |
| 962 | `.writeUInt32BE()` | Büyük uçlu işaretsiz 32 bit sayı yazar. |
| 963 | `.writeUInt32LE()` | Küçük uçlu işaretsiz 32 bit sayı yazar. |

### crypto

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 964 | `.createHash()` | Özet hesaplama nesnesi oluşturur. |
| 965 | `.createHmac()` | Anahtarlı özet nesnesi oluşturur. |
| 966 | `.createCipheriv()` | Anahtar ve IV ile şifreleyici oluşturur. |
| 967 | `.createDecipheriv()` | Anahtar ve IV ile çözücü oluşturur. |
| 968 | `.createSign()` | Dijital imza nesnesi oluşturur. |
| 969 | `.createVerify()` | Dijital imza doğrulayıcısı oluşturur. |
| 970 | `.randomBytes()` | Kriptografik rastgele baytlar üretir. |
| 971 | `.randomFill()` | Tamponu rastgele baytlarla doldurur. |
| 972 | `.randomInt()` | Kriptografik rastgele tamsayı üretir. |
| 973 | `.randomUUID()` | Rastgele UUID üretir. |
| 974 | `.pbkdf2()` | PBKDF2 ile anahtar türetir. |
| 975 | `.scrypt()` | scrypt ile anahtar türetir. |
| 976 | `.hkdf()` | HKDF ile anahtar türetir. |
| 977 | `.timingSafeEqual()` | Eş uzunluktaki baytları sabit zamanla sınar. |
| 978 | `.generateKeyPair()` | Açık ve özel anahtar çifti üretir. |
| 979 | `.createPublicKey()` | Açık anahtar nesnesi oluşturur. |
| 980 | `.createPrivateKey()` | Özel anahtar nesnesi oluşturur. |
| 981 | `.createSecretKey()` | Simetrik anahtar nesnesi oluşturur. |
| 982 | `.sign()` | Veri için dijital imza üretir. |
| 983 | `.verify()` | Verinin dijital imzasını doğrular. |
| 984 | `.publicEncrypt()` | Açık anahtarla şifreler. |
| 985 | `.privateDecrypt()` | Özel anahtarla şifreyi çözer. |
| 986 | `.getHashes()` | Desteklenen özet algoritmalarını listeler. |
| 987 | `.getCiphers()` | Desteklenen şifre algoritmalarını listeler. |

### EventEmitter

| No | Metot / fonksiyon | Türkçe açıklama |
| --- | --- | --- |
| 988 | `.on()` | Olay dinleyicisi ekler. |
| 989 | `.once()` | Bir kez çalışan dinleyici ekler. |
| 990 | `.off()` | Olay dinleyicisini kaldırır. |
| 991 | `.emit()` | Adlandırılmış olayı tetikler. |
| 992 | `.addListener()` | Dinleyici ekler; on ile eşdeğerdir. |
| 993 | `.removeListener()` | Belirtilen dinleyiciyi kaldırır. |
| 994 | `.removeAllListeners()` | Olayın veya tüm olayların dinleyicisini siler. |
| 995 | `.listeners()` | Olay dinleyicilerini listeler. |
| 996 | `.rawListeners()` | Sarmalayıcılar dahil dinleyicileri verir. |
| 997 | `.listenerCount()` | Olay dinleyicilerini sayar. |
| 998 | `.eventNames()` | Dinleyicisi bulunan olay adlarını listeler. |
| 999 | `.setMaxListeners()` | Dinleyici uyarı eşiğini ayarlar. |
| 1000 | `.getMaxListeners()` | Dinleyici uyarı eşiğini getirir. |
