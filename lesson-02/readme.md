# Lesson - 02

<br>

## Tags - Teglar

- Headings
- Paragraphs
- Formatting
- Quotations
- Other tags...

<br><br><br><br><br>

##  Heading Tags – HTML


| Teg nomi | Tavsif (Sarlavha darajasi) | Standart shrift o‘lchami (px) |
|----------|-----------------------------|-------------------------------|
| `<h1>`   | Eng katta sarlavha          | 32px                          |
| `<h2>`   | Ikkinchi darajali sarlavha | 24px                          |
| `<h3>`   | Uchinchi darajali sarlavha | 20.8px                        |
| `<h4>`   | To‘rtinchi darajali sarlavha| 16px                          |
| `<h5>`   | Beshinchi darajali sarlavha | 12.8px                        |
| `<h6>`   | Eng kichik sarlavha         | 11.2px                        |


<br><br><br><br>



## Paragraph Tags – HTML

| Teg nomi | Ma’nosi (Tarjimasi)       | Vazifasi / Qoida                                               |
|----------|----------------------------|----------------------------------------------------------------|
| `<p>`    | Paragraph (paragraf)       | Matnni paragraflarga bo‘ladi. Har paragraf yangi qatorda chiqadi. |
| `<hr>`   | Horizontal rule (chiziq)   | Sahifadagi mavzular orasiga gorizontal chiziq chizadi.         |
| `<br>`   | Line break (satr uzilishi) | Matnda yangi qatorga o‘tish uchun ishlatiladi.                 |
| `<pre>`  | Preformatted text          | Matnni qanday yozilgan bo‘lsa, shunday ko‘rsatadi (bo‘sh joy, qator). |


<br><br><br><br>



##  Formatting Tags – HTML

| Teg nomi        | Ma’nosi (Tarjimasi)          | Vazifasi / Qoida                                                                 |
|------------------|-------------------------------|----------------------------------------------------------------------------------|
| `<b>`            | Bold (qalin)                  | Matnni qalin ko‘rinishda chiqaradi, lekin urg‘u bermaydi.                        |
| `<strong>`       | Strong (kuchli urg‘u)         | Matnni qalin qiladi va semantik jihatdan muhimligini bildiradi.                 |
| `<i>`            | Italic (kursiv)               | Matnni qiyshiq yozuvda ko‘rsatadi, urg‘usiz.                                     |
| `<em>`           | Emphasis (urg‘u)              | Matnni kursiv qiladi va urg‘u berilgan matn deb belgilaydi.                      |
| `<u>`            | Underline (tagiga chizilgan)  | Matn ostiga chiziq chizadi.                                                      |
| `<ins>`          | Inserted text (qo‘shilgan matn)| Yangi qo‘shilgan matn sifatida belgilaydi, odatda tagiga chiziq bilan.           |
| `<del>`          | Deleted text (o‘chirilgan)    | O‘chirilgan matn sifatida ko‘rsatadi, ustidan chiziq bilan.                      |
| `<mark>`         | Highlight (belgilash)         | Matnni marker bilan ajratib ko‘rsatadi (sariq fon bilan).                        |
| `<small>`        | Small text (kichik shrift)    | Matnni oddiy matnga qaraganda kichikroq shrift bilan ko‘rsatadi.                |
| `<sub>`          | Subscript (past indeks)       | Pastki indeksdagi matn uchun ishlatiladi (masalan: H<sub>2</sub>O).             |
| `<sup>`          | Superscript (yuqori indeks)   | Yuqori indeksdagi matn uchun ishlatiladi (masalan: x<sup>2</sup>).              |


<br><br><br><br>


## Quotation Tags – HTML

| Teg nomi       | Ma’nosi (Tarjimasi)           | Vazifasi / Qoida                                                                 |
|----------------|-------------------------------|----------------------------------------------------------------------------------|
| `<blockquote>` | Block quotation (uzun iqtibos) | Boshqa manbadan olingan uzun matnni ko‘rsatadi. `cite` atributi bilan manba URL’si belgilanadi. |
| `<abbr>`       | Abbreviation (qisqartma)       | Qisqartma yoki akronimlar uchun ishlatiladi. `title` atributida to‘liq ma’no beriladi. |



<br><br><br><br>


##  Other Tags – HTML

# HTML Tags Reference

| **Teg nomi**     | **Ma’nosi (Tarjimasi)**      | **Vazifasi / Qoida** | **Misol** |
|------------------|------------------------------|----------------------|-----------|
| `<code>`         | Code (kod)                   | Kod yozuvi uchun ishlatiladi. Monospace shrift bilan ko‘rsatadi. | `<code>let x = 5;</code>` |
| `<kbd>`          | Keyboard input (klaviatura)  | Klaviaturadan kiritiladigan tugmalarni ko‘rsatadi (masalan: Ctrl + C). | `Press <kbd>Ctrl + C</kbd> to copy.` |
| `<samp>`         | Sample output (natija)       | Dastur natijasi yoki komanda chiqishini ko‘rsatadi. | `<samp>Error: File not found.</samp>` |
| `<var>`          | Variable (o‘zgaruvchi)       | Matematik yoki dasturlashdagi o‘zgaruvchini ifodalaydi. | `The value of <var>x</var> is 10.` |
| `<time>`         | Time (vaqt)                  | Sana yoki vaqtni belgilash uchun ishlatiladi. SEO va mashinalar uchun qulay. | `<time datetime="2025-04-10">April 10, 2025</time>` |
| `<progress>`     | Progress bar (jarayon paneli)| Vaqtinchalik jarayonni (loading, progress) vizual ko‘rsatish uchun. | `<progress value="50" max="100"></progress>` |
| `<meter>`        | Measurement (o‘lchov)        | Belgilangan oraliqda qiymatni ko‘rsatadi (masalan: CPU yuki, reyting). | `<meter value="0.7" min="0" max="1">70%</meter>` |
| `<details>`      | Details (detallar)           | Bosilganda ochiladigan qo‘shimcha matnni yaratadi. | |
| `<summary>`      | Summary (sarlavha)           | `<details>` tegi ichida ko‘rinadigan sarlavha bo‘lib xizmat qiladi. |  |



<br><br><br><br>

## `README.md` faylining qisqacha tavsifi


>`README.md` fayli — bu bir dastur yoki loyiha haqida foydalanuvchilar va ishlab chiquvchilar uchun ma'lumotlar taqdim etadigan matnli fayl. U odatda loyiha manba kodining birinchi darajali hujjatidir va uni ko'proq tushunish yoki ishlatish uchun kerakli barcha ma'lumotlarni beradi. README.md fayli Markdown (MD) formatida yoziladi, bu esa matnni shakllantirish uchun juda qulay bo'ladi.