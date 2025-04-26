# Lesson - 04

- `Doctype`


- `Images`

  - img tag
  - favicon
  - formats
  - websites
  - ul tag

- `Path (direction)`

  - / - root
  - ./ or nothing - current
  - ../ - parent
  - no other options (…/, …./)

- `Anchor tag`
  - href
  - target
  - download

<br><br><br><br>


# Doctype

>`<!DOCTYPE html>` — bu HTML hujjatining versiyasini brauzerga bildiradigan deklaratsiya. Bu kod har bir HTML faylning eng boshida yozilishi shart.

## Batafsil:

### 1. DOCTYPE nima?

- `DOCTYPE` — bu Document Type Declaration (hujjat turi deklaratsiyasi) so‘zining qisqartmasi.

- Bu kod brauzerga: “Bu fayl qanday HTML versiyada yozilganini bilib ol” degan ko‘rsatma beradi.

- U HTML elementi emas, shunchaki yo‘riqnoma — brauzerlar uchun.

<br>

### 2. Nega kerak?

- HTML turli versiyalarda mavjud: HTML 4.01, XHTML, HTML5.
- Har bir versiyada sintaksis, xatti-harakat biroz farq qiladi.
- Agar `DOCTYPE` bo‘lmasa, brauzer sahifani `quirks mode` deb ataladigan rejimda ochadi — bu esa eski brauzerlarga moslashadi va `bug`li, noto‘g‘ri ishlash xavfi bor.
- `DOCTYPE` bo‘lsa — sahifa standard mode rejimida ishlaydi, ya’ni eng zamonaviy va to‘g‘ri talqinda.

<br>

### 3. Zamonaviy DOCTYPE qanday yoziladi?

- HTML5 dan boshlab DOCTYPE juda soddalashtirilgan:

```
<!DOCTYPE html>
```
<br>

### 4. Oldingi versiyalardagi DOCTYPE qanday edi? (faqat bilib qo‘yish uchun)

- Masalan, HTML 4.01 da bunday edi:

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```
- Buni o‘qish ham qiyin, yozish ham charchatadi. HTML5 esa bu muammoni oddiy qilib qo‘ydi.
- DOCTYPE HTMLning bir qismi emas – u HTML elementi emas.
- U brauzerga yordam beradi, foydalanuvchiga ko‘rinmaydi.
- Har doim eng yuqoriga yoziladi, hatto <html> tagidan ham oldin.















<br><br><br><br>

# Image

## `img tag`

```
<!-- offline image -->

<img src="" width="" height="" alt="" />
```

<br>

## `websites`

- https://www.pexels.com/
- https://pixabay.com

<br>

## `favicon`

```
<!-- https://favicon.io/favicon-converter -->

<link rel="icon" href="" />
```

<br>

## `Image formats`

- jpeg
- jpg
- png
- gif
- psd
- svg

<br><br>

<h3 >.jpeg / .jpg<h3>

- Siqilgan rasm formati
- Shaffof fon qo‘llab-quvvatlanmaydi
- Real suratlar (fotosuratlar, manzaralar) uchun ideal
- Fayl hajmi kichikroq
- Ko‘p ishlatiladi

<br>

<h3 >.png<h3>

- Shaffof fon qo‘llab-quvvatlanadi
- Grafika, logotip, ikonka uchun ideal
- Sifat yuqori, lekin fayl hajmi kattaroq
- Siqilgan, lekin JPEGdan kamroq

<br>

<h3 >.gif<h3>

- Animatsiyali rasm formati
- 256 tagacha rangni qo‘llab-quvvatlaydi (cheklangan)
- Shaffoflik bor, lekin yarim shaffoflik yo‘q
- Qisqa animatsiyalar, stikerlar uchun ishlatiladi

<br>

<h3 >.psd<h3>

- Photoshop fayli
- Rasm qatlamlarini (layers) saqlaydi
- Faqat Adobe Photoshop yoki uni qo‘llovchi dasturlarda ochiladi
- Webda ishlatilmaydi, faqat dizayn uchun

<br>

<h3 >.svg<h3>

- Vektor format (kod asosida)
- Cheksiz kattalashtiriladi – sifat yo‘qolmaydi
- Shaffof fon mavjud
- Ikonkalar, logolar, diagrammalar uchun ideal
- Kichik hajm, tez yuklanadi

<br>

.webp


<br>

---

| Format | Shaffof Fon | Animatsiya | Siqilgan | Ishlatish joyi              | Webga mos |
| ------ | ----------- | ---------- | -------- | --------------------------- | --------- |
| JPEG   | Yo‘q        | Yo‘q       | Ha       | Suratlar, manzaralar        | Ha        |
| PNG    | Ha          | Yo‘q       | Ha       | Logolar, ikonka, grafik     | Ha        |
| GIF    | Ha          | Ha         | Ha       | Qisqa animatsiyalar, stiker | Ha        |
| PSD    | Ha (layers) | Yo‘q       | Yo‘q     | Dizayn fayllari (Photoshop) | Yo‘q      |
| SVG    | Ha          | Ha (basic) | Yo‘q     | Ikonkalar, vektor grafik    | Ha        |

---

<br><br>

## `ul tag in img`

```
<ul style="list-style-image: url();"></ul>
```

<br><br><br><br>

# Path (direction)

- ### `/` → Root (asosiy ildiz papka)

> Bu belgilar root, ya'ni loyihaning eng boshidagi papkani bildiradi.
> Masalan: `/images/photo.jpeg` → bu fayl loyihaning boshidagi images papkasida joylashgan.

<br>

- ### `./` yoki hech narsa yozmaslik → Joriy (hozirgi) papka

> `./` – hozir o‘zimiz turgan, ya'ni joriy papkani bildiradi.
> Masalan: `./style.css` yoki shunchaki `style.css` → bu fayl hozirgi papkada joylashgan.

<br>

- ### `../` → Bitta yuqoridagi (ota) papka

> `../` – bir pog‘ona yuqoridagi, ya'ni parent (ota) papkaga chiqishni bildiradi.
> Masalan: `../img/logo.png` → hozirgi papkadan bitta yuqoriga chiqib, img ichidagi logo.png faylini chaqiradi.

<br>

- ## 🚫 Boshqa variantlar yo‘q:

> `.../`, `..../` kabi yo‘llar mavjud emas va ishlamaydi.

> Faqat: `/`, `./`, `../` — shu uchta to‘g‘ri ishlaydi.

<br><br><br><br>

# Anchor tag

## `href`

```
<!-- relative (ichki) -->

<a href="pages/about.html">About Us</a>

<!-- absolute (tashqi) -->

<a href="https://www.instagram.com/najottalim">Instagram</a>
<a href="https://t.me/najottalim">Telegram</a>

<!-- other examples -->

<a href="#">Don't update</a>
<a href="tel: +998943371102">Phone number</a>
<a href="mailto: samandarkhodiev04@gmail.com">Email</a>
```
<br>

## `target`

```
<a href="url" target="_self">Self tab</a>
<a href="url" target="_blank">Other tab</a>
```
<br>

## `download`

```
<a href="url" download>Download</a>
```



<br><br><br><br>

#  Html haqida mustaqil qo'shimcha documentatsiya o'qish uchun

##  https://www.w3schools.com/