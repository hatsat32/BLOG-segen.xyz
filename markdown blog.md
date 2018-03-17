# MARKDOWN NEDİR

Markdown yazmayı kolaylaştıran bir yazım dilidir. normal web sayfaları html ile yazılır ve yayınlanır. fakat html yazı dilinden daha çok yayın dilidir. bu ne demek şimdi? html ile yazmak zordur. mesela `<` , `>` ,`/` gibi işaretleri devamlı olarak kullanmamız gerekir. buda yazımızı yazmamızı ve değiştirmemizi zorlaştırır ve okunabilirliği zordur. işte bu noktada markdown yardımımıza yetişiyor.

Markdown yazmayı kolaylaştıran bir yazım dilidir. **kalın** *italik* ~~üstü çizgili~~ ifadeler çok kolay bir şekilde yazılabilir, değiştirilebilir. üstelik markdown yazarken basit bir texteditor hatta notepad bile yeter. Üstelik html'e kolaycana dönüştürülebilmeside cabası. 

Bunu yapmak için Word gibi programlarda kullanılabilir fakat Word gibi programlarda çok fazla seçenek vardır. Renklendirme, hizalama, yazı boyutu yazı tipi vs. Ve ayrıca Word de yazarken sık sık fare ile seçim yapmamız gerekir. buda bizi yazmaktan uzaklaştırır ve dikkatimizi dağıtır. Elbette görsel ögeler önemlidir fakat önce yazı yazılmalıdır daha sonra görsellik eklenmelidir.

Neyse fazla uzatmadan markdown dan devam edelim.

---
# Markdown Syntax
Markrown'ın syntaxı çok kolaydır. Öğrenmek için 30 dakika yeterlidir. Çoğu zaman daha az sürer. İnanmıyorsanız hemen görelim.

---
## Başlıklar
`#` karakteri başlık koymaya yarar. 1 tane # en önemli başlıktır ve # sayısı arttıkça önem azalır.

```markdown
# başlık 1
## başlık 2
### başlık 3
#### başlık 4
##### başlık 5
###### başlık 6
```
bu kodun çıktısı aşağıdaki gibidir. ayrıca her başlıktan sonra bir alt satıra otomatik olarak iner.

# başlık 1
## başlık 2
### başlık 3
#### başlık 4
##### başlık 5
###### başlık 6

---
## Kalın İtalik Üstüçizgili vs.
İtalik yazmak için `*italik*` veya `_italik_` kullanırız. yani alttire veya yıldız işaretini.  
Kalın yazmak için `**kalın**` veya  `__kalın__` kullanırız. yani 2 tane * veya alttire.  
üstü çizgili yazmak için `~~üstü çizgili~~` kullanırız. yani 2 tane "~~"işareti.

---
## Linkler ve Resimler
Link koymak ta oldukça kolay. sadece "[] ()" parantezlerini bilmek yeter. "[isim](link)"
``[Link](https://www.google.com.tr)`` sonuç: [Link](https://www.google.com.tr)

Eğer çok sayıda link eklememiz gerekirse aşağıdaki gibi sayı verip daha sonra linkleri yazabiliriz. bu markdown yazımızın okunabilirliğini arttırır.
```markdown
[Link][1]

[1]: http://b.org
```

Resim koymakta linke benzer sadece başına ! (ünlem) getirmek yeterlidir.  
`![resim](http://URL/a.png)` bu şekilde resim gösterilegilir.

Çok sayıda resim eklerken numara ile ekleyebiliriz. linklerde olduğu gibi.
```markdown
![Link][1]

[1]: http://url/b.jpg
```

---
## Listeler

sırasız liste * veya - ile oluşturulur.
```markdown
* liste
* liste
* liste
``` 
* liste
* liste
* liste

veya
```markdown
- liste
- liste
- liste
``` 
- liste
- liste
- liste

Sıralı liste ise aşağıdaki şekilde oluşturulur.
```markdown
1. One
2. Two
3. Three
```
Listeleri içiçede kullanabiliriz. Nasıl mı?
```markdown
1. one
	* elma
	* ekmek
		- kepekli
		- kepeksiz
	* muz
2. Two
	+ bir
	+ iki
	+ üç
3. Three
	1. matematik
	2. fizik
	3. kimya
```
İşte buda çıktısı.  
1. one
	* elma
	* ekmek
		- kepekli
		- kepeksiz
	* muz
2. Two
	+ bir
	+ iki
	+ üç
3. Three
	1. matematik
	2. fizik
	3. kimya

---
## Birkaç Şey Daha
Markdown da aşağı satıra inmek için 2 tane boşluk ve enter kullanılır.  
Çizgi çekmek için `---` veya  `***` kullanılır. Bazen metni yada iki paragrafı bir çizgi ile ayırmak istediğinizde çok kullanışlıdır.  
Markdown da özel karakterleri "\\" ile yazabilirsiniz. Mesela \` karakterini ben böyle yazdım.

---
## Kod Yazmadan OLMAZ
kod yazmak için  \` karakteri kullanılır. \`kod\` gibi. Eğer bir satırdan daha fazla kod yazmak istersek 3 tane \` kullanırız. bu işaretler kod blokları açar. kod bittiğinde aynı işaret ile kapatmamız gerekir. aşağıdiki gibi.

\`\`\`python   
\# code block
print("hello world")  
\`\`\`

## Tablolar
Tablo için `|` işareti ve `-` kullanılır. | ile kolonlar çizilir. - ilede tablo başlığı. Çok kolay değil mi?
```markdown
| İsim  | Soyisim| Yaş|
|:------|:------ |:---|
| ali  | soy1 | 15 |
|veli | soy2 | 10 |
|ayşe | soy3 | 8 |
```

sonuç mu:
| İsim  | Soyisim| Yaş|
|:------|:------ |:---|
| ali  | soy1 | 15 |
|veli | soy2 | 10 |
|ayşe | soy3 | 8 |

---
## Alıtı Yapmak
Alıntı yapmak için `>` karakteri kullanılır. bu işaretten sonra alıntımızı yazabiliriz.
>bu bir alıntı orneğidir. 

### Bana gelince...
ben blog yazılarımı markdown ile yazıyorum. daha sonra html'e dönüştürüp yayınlıyırum. ve Markdown benim işimi çok kolaylaştırıyor. Sizlerede **şiddetle** tavsiye ederim.

# Kaynaklar
Markdown'ın daha birçok özelliği var fakat ben burada sadece temel özelliklerini anlattım. Aşağıdaki linklerden daha ayrıntılı bilgiye ulaşabilirsiniz.

[bloğumda paylaştığım yazıların markdown halleri][6]  
[Markdown][1]  
[markdown tutorial][2]  
[markdown github tutorial][3]  
[markdown summary][4]  
[markdon guide][5]  

[1]: https://daringfireball.net/projects/markdown/
[2]: https://www.markdowntutorial.com/
[3]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[4]: http://commonmark.org/help/
[5]: https://www.markdownguide.org/
[6]: https://github.com/hatsat32/BLOG-segen.xyz