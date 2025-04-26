<h1 style="color:orange;">Lesson - 01 | Css</h1>

<br>

# Css introduction

- css - what is it.?
- css comments
- inline style
- internal style
- external style
- style overriding
- colors
- selectors and specificity
- text style
- prettier
- dev tools

<br><br><br><br><br><br><br>

<h1 style="color:yellow;">Css - what is it.?<h3>

>`CSS` degani — `Cascading Style Sheets`, ya'ni "Kaskadli uslub sahifalari". Bu — veb-sahifalarga ko‘rinish (dizayn) berish uchun ishlatiladigan til. HTML orqali sahifa tarkibi (matn, rasm, tugma va h.k.) yaratiladi, CSS esa bu elementlarga:

- rang berish,
- shrift o‘zgartirish,
- joylashuvni aniqlash,
- oraliq va chekka (margin/padding) sozlash,
- animatsiya yoki o'tish effektlari qo‘shish
- kabi ko‘rinishdagi o‘zgarishlarni amalga oshirish imkonini beradi.

<br><br><br><br><br>

<h1 style="color:yellow;">Css comments<h3>

`/* -- … --*/` (Ctrl + /)

<br><br><br><br><br>

<h1 style="color:yellow;">Inline style<h3>

> `Inline style` — bu CSS uslublarini to‘g‘ridan-to‘g‘ri HTML elementining style atributi ichida yozishdir.

<br>

### Syntax:

```
<tag style="property: value;">Kontent</tag>
```

<br><br><br><br><br>

<h1 style="color:yellow;">Internal style<h3>

### Syntax:

```
<head>
  <style>
    selector {
      property: value;
    }
  </style>
</head>
```

<br>

### Example:

```
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <title>Internal Style Misol</title>
  <style>
    h1 {
      color: blue;
      text-align: center;
    }

    p {
      font-size: 16px;
      color: gray;
    }
  </style>
</head>
<body>
  <h1>Salom, CSS!</h1>
  <p>Bu paragraf internal style bilan yozilgan.</p>
</body>
</html>

```

<br><br><br><br><br>

<h1 style="color:yellow;">External style<h3>

### Syntax:

.html

```
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

.css

```
/* style.css faylida yoziladi */
selector {
  property: value;
}
```

<br>

### Example:

.html

```
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <title>External Style Misol</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Salom, CSS!</h1>
  <p>Bu paragraf external style bilan bezatilgan.</p>
</body>
</html>

```

.css

```
h1 {
  color: darkred;
  text-align: center;
}

p {
  font-size: 18px;
  color: green;
}
```

<br><br><br><br><br>

<h1 style="color:yellow;">Style overriding<h3>

```
h1 {
  color: red;
  color: green;
}
```

<br><br><br><br><br>

<h1 style="color:yellow;">Colors<h3>

- ### `Names`
- ### `RGB and RGBA`
- ### `HEX`
- ### `HSL`

<br><br>

### `Names`

- red, orange, blue, green, white, black ...

<br>

### `RGB and RGBA`

- RGB → red [0, 255], green [0, 255], blue [0, 255]
- RGBA → red, green, blue, alpha [0, 1]

### Example:

RGB

```
h1 {
  color: rgb(0, 128, 255); /* ko'k rang */
}
```

RGBA

```
p {
  color: rgba(255, 0, 0, 0.5); /* yarim shaffof qizil */
}
```

<br>

### `HEX`

- hexadecimal - rr, gg, bb

### Example:

```
h1 {
  color: #ff6600; /* to'q sariq rang */
}
```

<br>

### `HSL`

- hue (0 – red, 120 – green, 240 – blue)
- saturation (0 – gray, 100 – full color)
- light (0 – black, 100 – white)

### Example:

```
p {
  color: hsl(200, 100%, 50%);
}
```

<br><br><br><br><br>

<h1 style="color:yellow;"> CSS Selectors and Specificity<h3>


CSS’da bir nechta selector turlari mavjud va ularning ustunlik darajasi (specificity) farq qiladi. Specificity — bu qaysi style qoida boshqa biridan ustun turishini belgilovchi tizim.

---

### 📊 Jadval: Selectorlar va Specificity darajalari

| Selector turi      | Misol                    | Specificity     | Ustunlik darajasi              | Izoh                                |
| ------------------ | ------------------------ | --------------- | ------------------------------ | ----------------------------------- |
| `!important`       | `color: red !important;` | **∞ (cheksiz)** | 🥇 Eng kuchli (har doim ustun) | Specificity tizimini ham yengadi.   |
| Inline style       | `style="..."`            | **1000**        | 🥈 Juda kuchli                 | Element ichida yoziladi.            |
| ID selector        | `#id`                    | **0100**        | 🥉 Kuchli                      | Har sahifada unikal bo‘lishi kerak. |
| Class selector     | `.class`                 | **0010**        | O‘rtacha kuch                  | Ko‘p ishlatiladi.                   |
| Attribute selector | `[type="text"]`          | **0010**        | O‘rtacha kuch                  | Klass kuchida.                      |
| Pseudo-class       | `:hover`, `:focus`       | **0010**        | O‘rtacha kuch                  | Klass kabi.                         |
| Element selector   | `h1`, `p`, `div`         | **0001**        | Past kuch                      | Oddiy selector.                     |
| Pseudo-element     | `::before`, `::after`    | **0001**        | Past kuch                      | Element selector darajasida.        |
| Universal selector | `*`                      | **0000**        | Juda zaif                      | Specificity yo‘q deyarli.           |

---

### 🧠 Specificity qanday hisoblanadi?

Specificity 4 xonali son sifatida hisoblanadi: `(a, b, c, d)`

- `a` — Inline styles (1000 ball)
- `b` — ID selectors (100 ball)
- `c` — Class, attribute, pseudo-class selectors (10 ball)
- `d` — Element va pseudo-element selectors (1 ball)

📌 `!important` esa bu tizimdan tashqarida va **har doim ustun**.

---

<br><br><br><br><br>

<h1 style="color:yellow;">Text style<h3>

- text-decoration
- text-transform
- text-indent
- word-spacing
- letter-spacing
- line-height
- white-space (nowrap)
- pseudo-elements (first-line, first-letter)
- opacity
- text-shadow