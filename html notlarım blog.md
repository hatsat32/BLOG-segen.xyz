# HTML NOTLARI
Html çalışırken not aldığım html notlarım. Biraz acemice olabilir. 

# ETİKETLER
## TEMEL YAPISI
```html
<!DOCTYPE html>

<html>
	<head>
		<meta charset="utf-8">
		<title>ilk web site</title>
	</head>

	<body>
		merhaba nasılsın
	</body>
</html>
```

- `<!DOCTYPE html>` bu etiket en başa konulmalıdır. belgenin html olduğunu gösterir. browserin web sayfasını doğru göstermesine yardımcı olur. html taginden önce gelmelidir.

- `<html> </html>`  bütün html bu etiket ile başlar ve biter. Html elementlerinin root elemanıdır.

- Bütün html ifadeleri taglardan oluşur. bir taba başla bir tane bitiş tagi. `<tagismi> içerik </tagismi>` gibi. bitiş tagi "/" içermelidir. Ayrıca bütün taglarin ekstra özellikleri olabilir. bu normaldir. etiketle ilgili ekstra bilgi verir ve başlangıç taginin içinde bulunur. `isim="değer"` şeklinde yazılır. tag türkçesi etikettir.
- `<html lang="en-US"></html>` "lang" html etiketinin bir özelliğidir. dili belirtir.

Genellikle html tag leri küçük karakterler ile yazılır. büyük karakterlerde kullanılabilir fakat bu neredeyse hiç tercih edilmez ve birçok developer küçük harfler kullanır.

### TEMEL BİLGİLER
```html
<head>
		<meta charset="utf-8">
		<title>ilk web site</title>
</head>

<body>
	merhaba nasılsın
</body>
```

- `<head></head>` bu etiket html sayfasının temel bilgilerini verir. Html ile ilgili meta data içerir. içeriğini değil.
- `<body></body>`	bu etiket içeriğini barındırır. yani sayfada görünen her şey.
- `<meta charset="utf-8">` sayfanın karakter kodlamasını gösterir. genellikle utf-8 kullanılır.
- `<title>ilk web site</title>` web sitesinin başlığıdır. sekme çubuğunda görünür.


## BAŞLIKLAR PARAGRAFLAR BİÇİMLENDİRME ...
```html
<h1>baslik1</h1>
<h2>baslik2</h2>
<h3>baslik3</h3>
<h4>baslik4</h4>
<h5>baslik5</h5>
<h6>baslik6</h6>
```

bu tagler html de başlık koymal için kullanılır. h1 en büyük h6 en küçük başlıktır. kalın yazılır ve alt satıra otomatik geçer. bu etiketi kalın yazmak için kullanma. çünkü google bu tagleri indexlemede kullanıyor. arama sonuçlarında alt sıralara düşebilirsin.

- `<h1 style="font-size:60px;">Heading 1</h1>` bu şekilde başlığın boyutu büyültülebilir.

- `<p>nasılsın</p>`	bir paragraf  örniğidir.
- `<p style="color:red">I am a paragraph</p>` `style="color:renk"` paragrafı kırmızı yada başka bir renk gösterir.
- `<p title="tooltip"> paragraf</p>` mouse ı paragrafın üstüne getirip beklediğimizde bir ipucu gösterir.

pre etiketi formatlı yada biçimlendirilmiş yazıları gösterir. 
```html
<pre>
  merhaba
  kod da enter ile yeni satıra inersen
  browser da görünür.
</pre>
```

- `<strong></strong>`		bu etiketin arasındaki her şey bold yani kalın yazılır.
- `<em></em>`  			bu etiketin arasındaki her şey italik yazılır.
- `<!-- yorumlar olmazsa olmaz -->`  yorum satırları olmadan olmaz :).

```html
<br>
<hr>
<br/>
<hr/>
```
- br etiketi alt sarıra geçmemizi sağlar.
- hr etikeri çizgi çekmemizi sağlar. mesela iki paragraf arasını bir çizgi ile ayırabiliriz.
---
## LİSTELER
```html
<ul>
	<li>1. öğe</li>
	<li>2. öğe</li>
	<li>3. öğe</li>
</ul>
<ol>
	<li>1. öğe</li>
	<li>2. öğe</li>
	<li>3. öğe</li>
</ol>
```

- `<ul>` unordered list yanı numaralandırılmamış listedir. yani liste öğeleri noktalar ile gösterilir.
- `<ol>` ordered list yani liste öğeleri numaralı olarak gösterilir.
- `<li></li>` liste öğeleridir. 

---
## LİNKLER
- `<a href="deneme2.html">link</a>` link yazısına tıkladığımızda bizi deneme2.html sayfasına gönderir.

- `href="deneme2.html"` buradaki `href` linkin yoludur. buraya http://www.google.com da yazabiliriz.
- `<a href="default.asp">  <img src="resim.gif">  </a>` resimlerde link olarak kullanılabilir.

Bir yazıya yada metine id ve link atayabiliriz. Linke tıkladığımızda **aynı sayfada** bir yere gidebilir. Mesela aşağıda "atla" ya tıkladığımızda bizi aynı sayfada "C4" id li başlığa götütür. Sani sayfayı başlığa getirir.
```html
<h2 id="C4">Chapter 4</h2>
<a href="#C4">atla</a>
```
---
## RESİM VİDEO SES MEDYA ...
### resim
```html
<img src="Isparta.jpg" alt="ısparta gülü" width="300" height="250">
```
- `src` resmin yoludur.
- `alt` resmin yüklenememesi gibi bir durumda resmin yerine bir metin görünmesini sağlar. alternatif bir text tir.
- `width` resmin genişliği `height` resmin yüksekliğidir.

Herhangi bir resme link atamak istersek `a` etiketleri arasına alabiliriz: 
```html
<a href="http://www.google.com.tr"><img src="Isparta.jpg" alt="ısparta gülü" width="300" height="250"></a>
```

### Ses
ses dosyaları ve müzikler `audio` etiketi ile eklenebilir.
```html
<audio controls>
	<source src="den.mp3" type="audio/mpeg">
		bu ses dosyası desteklenmiyor.
</audio>
```

- `controls` ifadesi medya playeri açar. eğer bu olmazsa tarayıcıda sesi oynatacak bir player gelmez
- `<source>` etiketi arasına dosyanın yolunu ve tipini veririz.
eğer ses dosyası yüklenemez ise bir açıklama yazılabilir. açıklama için özel bir etiket gerekmez. doğrudan  `audio` etiketleri arasına yazılabilir

### Video
videolar `video` etiketi ile eklenir.
```html
<video width="640" height="360" controls autoplay loop>
	<source src="video.mp3" type="video/mp4">
	bu video tarayıcı tarafından desteklenmiyor.
</video>
``` 

1. `width` ve `height` videonun boyutu
2. `controls` video playerin çalışması için gerekli
3. `autoplay` sayfa yüklendiği anda videoyu oynatmaya başlar.
4. `loop` videoyu devamlı olarak tekrar oynatır. yani video bittiğinde baştan başlar.

### Klasör Yapıları
".." iki nokra ile üst dizine çıkılır. "/" ile alt dizine inilir.

---
## HTML Styles
html etiketleri stil özelliklerine sahip olabilir. `<tagname style="property:value;">` gibi.

1. `style="background-color:powderblue;"` arkaplan rengini verir.
2. `style="color:blue;"`  renk verir.
3. `style="font-family:verdana`;  özel font kullanmak için kullanılır.
4. `style="font-size:300%;`  font boyutunu belirler.
5. `style="text-align:center;`  metin hizalamasını ayarlar.

## HTML FORMATLAMA

1. `<b>` - Bold text
2. `<strong>` - önemli text. bold gibi gösterir.
3. `<i>` - italik text
4. `<em>` - Emphasized text. italik gibi görüntüler fakat daha önemlidir.
5. `<mark>` - Marked text üstü sarı işaretli gösterir
6. `<small>` - küçük text
7. `<del>` - üstü çizgili text
8. `<ins>` - altı çizgili text
9. `<sub>` - Subscript text. yazıyı biraz aşağıda gösterir.
10. `<sup>` - Superscript text. yazıyı biraz yukarıda gösterir.

---
## TABLOLAR
tablolar `<table>` etiketi ile tanımlanır. tablo satırları `<tr>` (table row) , tablo hücreleri `<td>` (table data), tablo başlıkları `<th>` (table header) ile tanımlanır. tabloya caption ile başlık verilebilir. aşağdaki gibi

```html
<table>
  <caption>başlık</caption>
  <tr>
    <th>isim</th>
    <th>meslek</th> 
    <th>yaş</th>
  </tr>
  <tr>
    <td>ali</td>
    <td>mühendis</td> 
    <td>50</td>
  </tr>
  <tr>
    <td>veli</td>
    <td>mimar</td> 
    <td>94</td>
  </tr>
</table>
```
#### Tabloya Verilebilecek Bazı Stiller
```css
padding: 15px
text-align: left
border-spacing: 5px
rowspan="2"
colspan="2"
```
---
## LİSTELER
### Sırasız liste

Listeleri numaralandırmadan gösterir.
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

Farklı stil seçenekleri kullanabiliriz.
```css
style="list-style-type:none"
style="list-style-type:square"
style="list-style-type:circle"
style="list-style-type:disc"
```

### Sıralı liste
Listeyi sıralı gösterir. yani liste elemanlarına numara verir.
```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

Farklı şekillerde gösterimleri var.
```css
type="1"
type="a"
type="A"
type="I"
type="i"
```

`start="50"` listeyi bir sayıdan başlatabiliriz.

liste içinde liste kullanılabilir.

---
## HTML Iframe
web sayfası içinde web sayfası göstermek için kullanılır.
- `<iframe src="demo_iframe.htm" height="200" width="300"></iframe>`
- `src="web_sayfası_linki"`


## HTML HEAD
head etiketinde bazı metadata bilgiler bulunabilir.
```html
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---
[w3schools](https://www.w3schools.com/html/default.asp) html için muhteşem bir kayanak. Benim çalıştığım yerlerden en beğendiği burası. Tavsiye ederim.

**Bir hatam varsa bana iletmekten çekinmeyin ki bende düzeltebileyim.**

## KAYNAKLAR
1. [W3SCHOOLS HTML](https://www.w3schools.com/html/default.asp)
2. [Yazılım bilimi kanalı](https://www.youtube.com/playlist?list=PLIHume2cwmHcfOVGqekxB-Q4z7gHfm7Qx)
3. [tutorialspoint html](https://www.tutorialspoint.com/html/index.htm)

