---

## 1. HTML HOME / HTML Introduction

**HTML ne?**
Web sayfalarının iskeletini oluşturan işaretleme dilidir. Tarayıcı, yazdığın etiketleri (tag) okuyup ekrana çevirir.

En temel yapı:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>İlk Sayfam</title>
</head>
<body>
    Merhaba dünya!
</body>
</html>
```

**Mini görev:**
`ilk.html` diye dosya aç, yukarıdaki kodu yapıştır, tarayıcıda aç.

---

## 2. HTML Editors

Notepad, Notepad++, VS Code, Sublime… Hepsiyle HTML yazabilirsin. En rahatı: **VS Code**.

Dikkat etmen gerekenler:

* Dosya uzantısı: **`.html`**
* Kod içinde Türkçe karakter için: `<meta charset="UTF-8">`

**Mini görev:**
VS Code’da `index.html` dosyası oluştur ve temel yapıyı yaz.

---

## 3. HTML Basic

Temel etiketler:

* `<h1>…</h1>` : başlık
* `<p>…</p>` : paragraf
* `<br>` : satır sonu
* `<a>` : link
* `<img>` : resim

Örnek:

```html
<body>
    <h1>Benim Web Sitem</h1>
    <p>Bu benim ilk paragrafım.</p>
    <p>Bu da ikinci paragraf.<br>Burada satır atladım.</p>
</body>
```

**Mini görev:**
Başlık + iki paragraf içeren basit bir sayfa yaz.

---

## 4. HTML Elements (Elemanlar)

**Element** = Açılış etiketi + içerik + kapanış etiketi

```html
<p>Bu bir paragraf elemanıdır.</p>
```

İç içe elemanlar:

```html
<p>Bu yazıda <b>kalın</b> bir kelime var.</p>
```

**Mini görev:**
Bir paragraf içinde hem kalın (`<b>`), hem italik (`<i>`) kelimeler kullan.

---

## 5. HTML Attributes (Öznitelikler)

Etiketlere ekstra bilgi ekler.

* `href` → link adresi
* `src` → resim yolu
* `alt` → resim açıklaması
* `id`, `class` → CSS için isimler
* `style` → satır içi stil

Örnek:

```html
<a href="https://www.google.com">Google'a git</a>
<img src="resim.jpg" alt="Profil fotoğrafım">
<p id="ilk-paragraf" class="kirmizi">Merhaba!</p>
```

**Mini görev:**
Kendini tanıtan bir paragraf yaz ve `id="ben"` ver.

---

## 6. HTML Headings (Başlıklar)

```html
<h1>En büyük başlık</h1>
<h2>Biraz daha küçük</h2>
<h3>...</h3>
<h4>...</h4>
<h5>...</h5>
<h6>En küçük başlık</h6>
```

Tarayıcı büyükten küçüğe doğru gösterir ve SEO açısından da önemlidir.

**Mini görev:**
Bir konu seç (örneğin “Oyunlar”)

* Sayfa başlığı: `<h1>`
* Alt başlıklar: `<h2>` (FPS Oyunları, Hikaye Oyunları gibi)

---

## 7. HTML Paragraphs (Paragraflar)

```html
<p>Bu bir paragraf.</p>
<p>Bu da ikinci paragraf.</p>
```

Satır atlamak için:

```html
Satır 1<br>
Satır 2
```

**Mini görev:**
Sevdiğin bir oyunu anlatan 3 paragraf yaz.

---

## 8. HTML Styles (Stiller) – style attribute

Satır içi stil:

```html
<p style="color:red; font-size:20px;">Kırmızı yazı</p>
<p style="text-align:center;">Ortalanmış yazı</p>
```

**Mini görev:**
Biri kırmızı, biri mavi, biri büyük fontlu 3 farklı paragraf yaz.

> Not: Gerçekte stilleri CSS dosyasında toplamak daha doğrudur, aşağıda CSS kısmında gelecek.

---

## 9. HTML Formatting (Biçimlendirme)

Sık kullanılanlar:

```html
<b>kalın</b>
<strong>önemli kalın</strong>
<i>italik</i>
<em>vurgulu italik</em>
<u>altı çizili</u>
<small>küçük yazı</small>
<sub>alt simge</sub>  (H<sub>2</sub>O)
<sup>üst simge</sup>  (x<sup>2</sup>)
```

**Mini görev:**
`x^2 + 3x + 5` ifadesini HTML ile düzgün göster.

---

## 10. HTML Quotations (Alıntılar)

```html
<p>Albert Einstein dedi ki:</p>
<blockquote>
    Hayal gücü bilgiden daha önemlidir.
</blockquote>

<p>O "ben geliyorum" dedi.</p>
<q>Bu kısa bir alıntı.</q>
```

**Mini görev:**
Sevdiğin bir sözü `<blockquote>` içinde yaz.

---

## 11. HTML Comments (Yorumlar)

Tarayıcıda görünmez, sadece kod içinde not:

```html
<!-- Bu bir yorum satırıdır -->
<p>Bu görünür.</p>
```

**Mini görev:**
Sayfana kendi adınla ilgili bir yorum ekle (`<!-- Burayı Kiran yazdı -->` gibi).

---

## 12. HTML Colors (Renkler)

Renk verme şekilleri:

```html
<p style="color: red;">İsim ile</p>
<p style="color: #00ff00;">Hex ile</p>
<p style="color: rgb(0, 0, 255);">RGB ile</p>
<p style="background-color: yellow;">Arka plan rengi</p>
```

**Mini görev:**
Arka planı açık gri, yazıyı lacivert yap.

---

## 13. HTML CSS

CSS, stilleri ayrı bir yerde yönetmek için kullanılır.

### a) Dahili CSS (internal)

```html
<head>
<style>
    body { background-color: #f0f0f0; }
    h1 { color: darkblue; }
    p  { color: #333333; }
</style>
</head>
```

### b) Harici CSS (external)

`style.css` dosyası:

```css
body {
    background-color: #f0f0f0;
}
h1 {
    color: darkblue;
}
```

HTML:

```html
<link rel="stylesheet" href="style.css">
```

**Mini görev:**
`style.css` oluştur, body arka planını farklı bir renk yap.

---

## 14. HTML Links (Bağlantılar)

```html
<a href="https://www.youtube.com" target="_blank">YouTube</a>
```

* `target="_blank"` → yeni sekmede aç

Sayfa içi link:

```html
<a href="#alt-kisim">Alta git</a>

...

<h2 id="alt-kisim">Sayfanın alt kısmı</h2>
```

**Mini görev:**
Bir sayfanda 3 farklı siteye link ekle.

---

## 15. HTML Images (Resimler)

```html
<img src="resim.jpg" alt="Açıklama" width="300" height="200">
```

* `alt` → resim yüklenmezse görülen metin
* Genişlik, yükseklik px olarak verilebilir.

**Mini görev:**
Masaüstünden bir resim dosyasını proje klasörüne kopyala ve sayfada göster.

---

## 16. HTML Favicon

Sekme yanında görünen küçük ikon.

```html
<head>
    <link rel="icon" type="image/x-icon" href="favicon.ico">
</head>
```

**Mini görev:**
Herhangi bir 32x32 png’yi bul, online favicon dönüştürücüsü ile `.ico` yap, projene koy.

---

## 17. HTML Page Title (Sayfa Başlığı)

Tarayıcı sekmesinde görünen isim:

```html
<head>
    <title>Kiran'ın İlk Sitesi</title>
</head>
```

**Mini görev:**
Her farklı sayfana mantıklı bir `title` ver (Ana Sayfa, Hakkımda, İletişim gibi).

---

## 18. HTML Tables (Tablolar)

Temel yapı:

```html
<table border="1">
    <tr>
        <th>Ders</th>
        <th>Gün</th>
        <th>Saat</th>
    </tr>
    <tr>
        <td>Matematik</td>
        <td>Pazartesi</td>
        <td>10:00</td>
    </tr>
</table>
```

* `<table>` : tablo
* `<tr>` : satır
* `<th>` : başlık hücresi (kalın, ortalı)
* `<td>` : normal hücre

**colspan / rowspan:**

```html
<td colspan="2">2 sütunu birleştir</td>
<td rowspan="3">3 satırı birleştir</td>
```

**Mini görev:**
Kendi haftalık ders programını tablo ile yap.

---

## 19. HTML Lists (Listeler)

### Sırasız liste (noktalı) – `<ul>`

```html
<ul>
    <li>Elma</li>
    <li>Armut</li>
    <li>Muz</li>
</ul>
```

### Sıralı liste (numaralı) – `<ol>`

```html
<ol>
    <li>Adım 1</li>
    <li>Adım 2</li>
</ol>
```

**Mini görev:**
Favori oyunlarını bir `<ul>`, yapılacak işlerini bir `<ol>` ile yaz.

---

## 20. HTML Block & Inline

**Block elemanlar**: satırın tamamını kaplar, alt satıra geçer.
Örnek: `<div>`, `<p>`, `<h1>`, `<ul>`, `<table>`

**Inline elemanlar**: Sadece içeriği kadar yer kaplar, satırı bölmez.
Örnek: `<span>`, `<a>`, `<img>`, `<b>`, `<i>`

Örnek:

```html
<p>Bu bir block elemandır.</p>
<a href="#">Bu link</a> ve <span>bu span</span> aynı satırda.
```

**Mini görev:**
Bir paragrafın içinde birkaç kelimeyi `<span>` ile renklendir (inline stil ver).

---

## 21. HTML Div

`<div>` = “kutu” gibi düşünebilirsin. Sayfayı bölmek için kullanılır (header, sidebar, content vs.).

```html
<div style="background-color: lightgray; padding: 10px;">
    <h2>Başlık</h2>
    <p>Bu kutunun içindeki yazı.</p>
</div>
```

Genelde CSS ile beraber:

```html
<style>
.kutu {
    background-color: #222;
    color: white;
    padding: 20px;
    width: 300px;
}
</style>

<div class="kutu">
    Bu bir kutu.
</div>
```

**Mini görev:**
Üstte “Başlık” div’i, altta “İçerik” div’i olan basit bir layout yap.

---

## Hepsini Birleştiren Küçük Proje Önerisi

`index.html` içinde:

* Başlıklar (`h1`, `h2`)
* Paragraflar
* Liste (oyunlar, hobiler)
* Bir resim
* Bir tablo (ders programı)
* Birkaç link
* Div’lerle bölünmüş alanlar
* Basit CSS (arka plan rengi, yazı rengi)

İstersen bir sonraki mesajında yazdığın kodu at, birlikte düzeltelim ve güzelleştirelim.
