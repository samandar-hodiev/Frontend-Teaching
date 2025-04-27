<h1 style="color:orange;">Lesson - 03 | html & Css3</h1>

Html
- Non-semantic elements
- Semantic elements
- Container

Css
- CSS text styles
- Link and button style
- Transition


<br><br><br><br><br><br>




<h1 style="color:yellow;">Non-Semantic HTML Elements</h1>

>Non-semantic HTML elementlar — bu `teglardir`, ular faqat struktura va dizaynni belgilash uchun ishlatiladi, ammo mazmun haqida hech qanday ma'lumot bermaydi.

| Element      | Vazifasi | Misol |
|--------------|----------|-------|
| `<div>`      | Strukturani tashkil qilish uchun ishlatiladi. Mazmuni haqida hech qanday ma'lumot bermaydi. | `<div class="container">Content here</div>` |
| `<span>`     | Qisqa matnli elementlar yoki kichik bo‘limlar uchun ishlatiladi. Kichik vizual o‘zgarishlar uchun. | `<span style="color: red;">Important</span>` |
| `<b>`        | Matnni qalin qiladi, ammo semantik ma'no bermaydi. | `<b>This text is bold</b>` |
| `<i>`        | Matnni kursiv qiladi, ammo semantik ma'no bermaydi. | `<i>This text is italic</i>` |
| `<br>`       | Satrni ajratish (yangi qatorga o‘tish) uchun ishlatiladi. | `First line<br>Second line` |
| `<hr>`       | Gorizontal chiziq (bo‘shliq) yaratadi. | `<hr>` |
| `<u>`        | Matnni ostiga chiziq qo‘yadi. | `<u>Underlined text</u>` |

---

## Qaysi holatlarda non-semantic elementlar ishlatiladi?

- **Tuzilish**: Kengaytirilgan layoutlarni yaratishda (masalan, `div` yoki `span`).
- **Stil va dizayn**: Ko‘pincha o‘zgarishlar yoki effektlar qo‘shish uchun (masalan, `b`, `i`, `u`).
- **Bo‘linmalar**: Sahifada bo‘linmalarni ajratish uchun (masalan, `hr`).

>Non-semantic elementlar matnning ma'no va mazmuni haqida hech qanday ma'lumot bermaydi, shuning uchun ular faqat tuzilishni tashkil etish va dizaynni boshqarishda ishlatilishi kerak.

<br><br><br><br>


<h1 style="color:yellow;">Semantic HTML Elements</h1>

>Semantic HTML elements — bu teglardir, ular sahifadagi ma'lumotning mazmuni yoki strukturasini aniq belgilaydi. Ular dizayn emas, balki ma'no taqdim etishga yordam beradi.

| Element      | Vazifasi | Misol |
|--------------|----------|-------|
| `<header>`   | Sahifaning yuqori qismi yoki bo‘limining sarlavhasini belgilaydi | `<header><h1>Welcome to My Website</h1></header>` |
| `<nav>`      | Navigatsiya menyulari yoki havolalar ro‘yxatini tashkil qiladi | `<nav><a href="#home">Home</a> <a href="#about">About</a></nav>` |
| `<article>`  | Mustaqil kontent bo‘limi (masalan, maqola yoki blog post) | `<article><h2>Blog Post Title</h2><p>Content here</p></article>` |
| `<section>`  | Sahifadagi ma'lum bir bo‘lim yoki mavzu | `<section><h2>About Us</h2><p>Information about our company</p></section>` |
| `<footer>`   | Sahifaning pastki qismi, odatda huquqiy ma'lumotlar yoki aloqa ma'lumotlarini o‘z ichiga oladi | `<footer><p>© 2025 Company Name</p></footer>` |
| `<main>`     | Sahifaning asosiy kontenti (o‘zgartirishlar, foydalanuvchiga asosiy ma'lumotlarni ko‘rsatish uchun) | `<main><p>This is the main content of the page</p></main>` |
| `<aside>`    | Sahifaning asosiy kontentidan tashqarida, lekin tegishli bo‘lgan ma'lumotlar | `<aside><h2>Related Articles</h2><p>Article 1</p></aside>` |
| `<figure>`   | Rasm, diagramma yoki video kabi elementlarni, ularning tasvirlari yoki tushuntirishlari bilan bog‘laydi | `<figure><img src="image.jpg" alt="An example image"><figcaption>Image Caption</figcaption></figure>` |
| `<figcaption>`| `<figure>` elementining tavsifi | `<figcaption>This is a description of the image</figcaption>` |

---

## Semantic Elementlarning Afzalliklari:

- **SEO (Search Engine Optimization)**: Qidiruv tizimlari sahifani yaxshiroq tushunadi.
- **Accessibility**: Ekran o‘qiydigan qurilmalar va brauzerlar uchun sahifani tushunishni osonlashtiradi.
- **Readability**: Kodni o‘qish va tushunish osonlashadi, chunki har bir element ma'lum bir ma'no anglatadi.

> Semantic HTML elementlardan foydalanish sahifangizni yaxshilash va foydalanuvchi tajribasini oshirishga yordam beradi.

<br><br><br><br>

<h1 style="color:yellow;">Container</h1>

**Container** — bu dizaynda elementlar va bo‘limlarni tartibga solish va markazlashtirish uchun ishlatiladigan HTML element yoki konteynerdir. U sahifaning o‘lchamini boshqarish, moslashuvchanlik va responsivlikni ta’minlash uchun ishlatiladi.

## CSS Container Xususiyatlari

| CSS xususiyati   | Vazifasi | Misol |
|------------------|----------|-------|
| `max-width`      | Konteynerning maksimal kengligini belgilaydi | `container { max-width: 1200px; }` |
| `width`          | Konteynerning kengligini belgilaydi | `container { width: 100%; }` |
| `margin`         | Konteynerni markazlashtirish uchun ishlatiladi | `container { margin: 0 auto; }` |
| `padding`        | Konteyner ichidagi bo‘shliqni sozlash | `container { padding: 20px; }` |
| `box-sizing`     | Konteynerning o‘lchamini hisoblashni boshqaradi | `container { box-sizing: border-box; }` |

<br><br><br><br>

<h1 style="color:yellow;">CSS Text Xususiyatlari</h1>

| CSS xususiyati    | Vazifasi                                                                    | Misol                                         |
| ----------------- | --------------------------------------------------------------------------- | --------------------------------------------- |
| `color`           | Matnning rangini o'zgartiradi                                               | `color: red;`                                 |
| `font-size`       | Matnning o‘lchamini belgilaydi                                              | `font-size: 20px;`                            |
| `font-family`     | Matn uchun shrift (harf turi) tanlaydi                                      | `font-family: Arial, sans-serif;`             |
| `font-weight`     | Matnning qalinligini belgilaydi                                             | `font-weight: bold;` yoki `font-weight: 700;` |
| `font-style`      | Matnni oddiy yoki kursiv (egilgan) qiladi                                   | `font-style: italic;`                         |
| `font-variant`    | Matnni small-caps (kichik katta harf) ko‘rinishida chiqaradi                | `font-variant: small-caps;`                   |
| `font`            | Font xususiyatlarini qisqacha yozish imkonini beradi                        | `font: italic bold 20px Arial;`               |
| `text-align`      | Matnni chapga, o‘rtaga, o‘ngga yoki justified (har ikki tomonga) tekislaydi | `text-align: center;`                         |
| `text-decoration` | Matnga ostiga chizish yoki o'chirish effektini qo‘shadi                     | `text-decoration: underline;`                 |
| `text-transform`  | Matnni katta harf, kichik harf yoki bosh harfga o‘zgartiradi                | `text-transform: uppercase;`                  |
| `letter-spacing`  | Harflar orasidagi masofani belgilaydi                                       | `letter-spacing: 2px;`                        |
| `word-spacing`    | So‘zlar orasidagi masofani belgilaydi                                       | `word-spacing: 5px;`                          |
| `line-height`     | Satrlar orasidagi balandlikni belgilaydi                                    | `line-height: 1.5;`                           |
| `direction`       | Matn yo‘nalishini o‘zgartiradi (`ltr`, `rtl`)                               | `direction: rtl;`                             |
| `white-space`     | Matndagi bo‘sh joylar va satr ko‘chirishlarni boshqaradi                    | `white-space: nowrap;`                        |
| `text-indent`     | Paragraf boshi bo‘sh joyini belgilaydi                                      | `text-indent: 30px;`                          |
| `overflow-wrap`   | Uzun so‘zlarni qatorga sig'dirish uchun qirqadi                             | `overflow-wrap: break-word;`                  |
| `word-break`      | So‘zlarni qanday sindirishni belgilaydi                                     | `word-break: break-all;`                      |
| `writing-mode`    | Matn yo‘nalishini o‘zgartiradi (vertikal yoki gorizontal)                   | `writing-mode: vertical-rl;`                  |

<br><br><br><br>

<h1 style="color:yellow;">Link (a) va Button (button) Style Xususiyatlari</h1>

| Element | CSS xususiyati     | Vazifasi                                              | Misol                                          |
| ------- | ------------------ | ----------------------------------------------------- | ---------------------------------------------- |
| Link    | `color`            | Link rangini o'zgartiradi                             | `a { color: blue; }`                           |
| Link    | `text-decoration`  | Link osti chizig'ini boshqaradi                       | `a { text-decoration: none; }`                 |
| Link    | `hover`            | Link ustiga bosilganda o'zgaradigan holat             | `a:hover { color: red; }`                      |
| Link    | `active`           | Link bosilganda (click vaqtida) style o'zgarishi      | `a:active { color: green; }`                   |
| Link    | `visited`          | Oldin bosilgan link uchun style                       | `a:visited { color: purple; }`                 |
| Button  | `background-color` | Tugma orqa fon rangini belgilaydi                     | `button { background-color: blue; }`           |
| Button  | `color`            | Tugma ichidagi matn rangini belgilaydi                | `button { color: white; }`                     |
| Button  | `border`           | Tugmaga ramka (chegara) qo‘shadi yoki olib tashlaydi  | `button { border: none; }`                     |
| Button  | `padding`          | Tugma ichidagi matn atrofidagi bo'sh joyni belgilaydi | `button { padding: 10px 20px; }`               |
| Button  | `border-radius`    | Tugma burchaklarini yumalatadi                        | `button { border-radius: 8px; }`               |
| Button  | `hover`            | Tugmaga kursor kelganda o'zgaradigan holat            | `button:hover { background-color: darkblue; }` |
| Button  | `cursor`           | Tugma ustida kursorni o'zgartiradi (masalan, pointer) | `button { cursor: pointer; }`                  |

<br><br><br><br>

<h1 style="color:yellow;"> CSS Transition Xususiyatlari</h1>

| CSS xususiyati               | Vazifasi                                                                                              | Misol                                    |
| ---------------------------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| `transition`                 | Bir yoki bir nechta property'ni o‘tish (o'zgarish) effektini belgilaydi                               | `transition: all 0.3s ease;`             |
| `transition-property`        | Qaysi xususiyat(lar) uchun transition bo'lishini aniqlaydi                                            | `transition-property: background-color;` |
| `transition-duration`        | O‘tish davomiyligini belgilaydi                                                                       | `transition-duration: 0.5s;`             |
| `transition-timing-function` | O‘tishning tezlik egri chizig‘ini belgilaydi (`ease`, `linear`, `ease-in`, `ease-out`, `ease-in-out`) | `transition-timing-function: ease-in;`   |
| `transition-delay`           | O‘tish boshlanishidan oldin kutish vaqtini belgilaydi                                                 | `transition-delay: 0.2s;`                |
