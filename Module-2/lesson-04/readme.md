<h1 style="color:orange;">Lesson - 04</h1>

## Flexbox

- What is it?

- Parent
   - justify-content
   - flex-wrap
   - flex-direction
   - align-items
   - align-content

- Child
   - flex-grow
   - flex-shrink
   - flex-basis
   - flex
   - align-self
   - order

<br>
<br>
<br>
<br>
<br>

<h1 style="color:yellow;">Flexbox nima.?</h1>

> CSS’dagi Flexbox (Flexible Box) — bu elementlarni bir qatorga yoki ustunga joylashtirish va ularni moslashuvchan qilib boshqarish uchun ishlatiladigan layout modelidir.

```
display: flex;
```

>Bu qoidani biror konteynerga berilsa, uning ichidagi elementlar flex item bo‘ladi va ularni yo‘nalish, joylashuv, o‘lcham bo‘yicha boshqarish mumkin bo‘ladi.

<br><br><br><br>

<h1 style="color:yellow;">Flexbox – Parent Element Xususiyatlari</h1>

| **Xususiyat**     | **Qiymatlar**                                                                       | **Tavsif**                                                                                                |
| ----------------- | ----------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `justify-content` | `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly` | Elementlarni **gorizontal yo‘nalishda** joylashtiradi.                                                    |
| `flex-wrap`       | `nowrap`, `wrap`, `wrap-reverse`                                                    | **Elementlarning qatorda joylashishini** boshqaradi. Agar joy kam bo‘lsa, ular boshqa qatorda joylashadi. |
| `flex-direction`  | `row`, `row-reverse`, `column`, `column-reverse`                                    | Elementlarning **joylashuv yo‘nalishini** (gorizontal yoki vertikal) belgilaydi.                          |
| `align-items`     | `flex-start`, `flex-end`, `center`, `stretch`, `baseline`                           | Elementlarning **vertikal hizalashini** boshqaradi (1 qator yoki ustun uchun).                            |
| `align-content`   | `flex-start`, `flex-end`, `center`, `space-around`, `space-between`, `space-evenly` | **Bir nechta qatorlar yoki ustunlar** orasidagi bo‘shliqni boshqaradi.                                    |

<br><br><br>


## > `"Hizalanadi"` degan so‘z — bu "tekislanadi", "joylashtiriladi", "bir chiziqqa qo‘yiladi" degani.



---
<h3 style="color:greenyellow;">justify-content<h3>

> Asosiy yo‘nalishda `default: gorizontal` elementlar orasidagi gorizontal bo‘shliqni boshqaradi.

### 1. `flex-start`
➡️ Elementlar chapga (yoki boshlanishga) yopishtiriladi.(Default qiymat).

### 2. `flex-end`
➡️ Elementlar o‘ngga (yoki oxirga) yopishtiriladi.

### 3. `center`
➡️ Elementlar markazga hizalanadi.

### 4. `space-between`
➡️ Birinchi va oxirgi element chetlarga yopishtiriladi, orasidagi bo‘shliq teng bo‘ladi.

### 5. `space-around`
➡️ Har bir element atrofida teng bo‘shliq bo‘ladi.
Lekin chetdagi elementlarda ichkaridagilarga nisbatan yarim bo‘shliq bo‘ladi.

### 6. `space-evenly`
➡️ Barcha elementlar orasida va chetlarda teng bo‘shliq bo‘ladi.


---

<br><br>

---

<h3 style="color:greenyellow;">flex-wrap<h3>

> Elementlar qatorga sig‘may qolsa, ularni yangi qatorga o‘tkazish yoki yo‘q qilmaslikni belgilaydi.

### 1. `nowrap`
➡️ (Default qiymat).
Elementlar bitta qatorda qoladi, sig‘masa siqiladi yoki konteynerdan chiqib ketadi.

### 2. `wrap`
➡️ Elementlar sig‘masa, avtomatik yangi qatorga tushadi.
Yuqoridan pastga yo‘nalishda joylashadi.

### 3. `wrap-reverse`
➡️ Elementlar sig‘masa, yangi qatorga tushadi,
lekin teskari tartibda — pastdan yuqoriga qarab joylashadi.

---

<br><br>


---

<h3 style="color:greenyellow;">flex-direction<h3>

> Elementlarning asosiy yo‘nalishini (gorizontal yoki vertikal) belgilaydi.

### 1. `row`
➡️ Default qiymat.
Elementlar chapdan o‘ngga — gorizontal yo‘nalishda joylashadi.

### 2. `row-reverse`
➡️ Elementlar o‘ngdan chapga — teskari gorizontal yo‘nalishda joylashadi.

### 3. `column`
➡️ Elementlar yuqoridan pastga — vertikal yo‘nalishda joylashadi.

### 4. `column-reverse`
➡️ Elementlar pastdan yuqoriga — teskari vertikal yo‘nalishda joylashadi.

---

<br><br>

---

<h3 style="color:greenyellow;">align-items<h3>

 >Cross axis bo‘yicha ya'ni, `flex-direction` ga teskari yo‘nalishda elementlarning vertikal joylashuvini boshqaradi.


> ⚠️ Agar flex-direction: row; bo‘lsa - vertikal yo‘nalishda ishlaydi
<br>
> ⚠️ Agar flex-direction: column; bo‘lsa - gorizontal yo‘nalishda ishlaydi

### 1. `flex-start`
➡️ Elementlar cross axis’ning boshlanishiga yopishtiriladi.
Agar yo‘nalish row bo‘lsa — yuqoriga hizalanadi.

### 2. `flex-end`
➡️ Elementlar cross axis’ning oxiriga yopishtiriladi.
Agar yo‘nalish row bo‘lsa — pastga hizalanadi.

### 3. `center`
➡️ Elementlar cross axis bo‘yicha markazga hizalanadi.

### 4. `stretch`
➡️ Elementlar bo‘sh joyni to‘liq egallaydi (balandlik yoki kenglik bo‘yicha).
✅ Faqat elementning height yoki width belgilanmagan bo‘lsa ishlaydi.
🟢 Default qiymat.

### 5. `baseline`
➡️ Elementlar matnning asosiy chizig‘i (baseline) bo‘yicha hizalanadi.
Bu ayniqsa har xil o‘lchamdagi matnli bloklarda foydali.

---

<br><br>

---

<h3 style="color:greenyellow;">align-content<h3>

>Ko‘p qatorli flex elementlar bo‘lsa, ularning cross axis bo‘yicha qatorlar orasidagi bo‘shliqni boshqaradi.

> Faqat `flex-wrap: wrap;` yoki `flex-wrap: wrap-reverse;` bo‘lsa ishlaydi.
> Agar faqat bitta qatordagi elementlar bo‘lsa — bu hech narsa qilmaydi.

### 1. `flex-start`
➡️ Barcha qatorlar yuqoriga (yoki boshlanishga) yig‘iladi.

### 2. `flex-end`
➡️ Barcha qatorlar pastga (yoki oxirga) yig‘iladi.

### 3. `center`
➡️ Qatorlar markazga yig‘iladi.

### 4. `space-around`
➡️ Qatorlar orasida teng atrofiy bo‘shliq bo‘ladi.
Chetdagi qatorlar — yarim bo‘shliq bilan joylashadi.

### 5. `space-between`
➡️ Birinchi va oxirgi qatorlar chetlarga yopishtiriladi,
o‘rtadagi qatorlar orasida teng bo‘shliq bo‘ladi.

### 6. `space-evenly`
➡️ Barcha qatorlar orasida va chetlarda teng bo‘shliq bo‘ladi.

>`align-items` — elementlar orasidagi vertikal joylashuv

>`align-content` — qatorlar orasidagi vertikal joylashuv

---

<br><br><br><br><br><br><br><br>

<h1 style="color:yellow;">Flexbox – CHild Element Xususiyatlari</h1>

| **Xususiyat**  | **Qiymatlar**                                     | **Tavsif**                                                                 |
|----------------|----------------------------------------------------|-----------------------------------------------------------------------------|
| `flex-grow`    | `0` (default), `1`, `2`, `3`, ...                  | Bo‘sh joyni nechta bo‘lakka bo'lishini belgilaydi.                         |
| `flex-shrink`  | `1` (default), `0`, `2`, ...                       | Ekran kichrayganda elementning qisqarish nisbatini belgilaydi.            |
| `flex-basis`   | `auto`, `100px`, `50%`, ...                        | Elementning boshlang‘ich (asosiy) o‘lchamini belgilaydi.                   |
| `flex`         | `<grow> <shrink> <basis>`                         | `flex-grow`, `flex-shrink`, va `flex-basis` ni qisqargan yozuvi.          |
| `align-self`   | `auto`, `flex-start`, `flex-end`, `center`, `baseline`, `stretch` | Faqat bitta elementning vertikal hizalashini boshqaradi.                   |
| `order`        | `0` (default), `1`, `2`, `-1`, ...                 | Elementning tartibini (qatordagi joylashuvini) o‘zgartiradi.              |


<br><br>

---

<h3 style="color:greenyellow;">flex-grow<h3>

> Bo‘sh joyni olish uchun elementning o‘sish nisbatini belgilaydi.
Agar konteynerda bo‘sh joy bo‘lsa, elementlar o‘sishiga imkon beradi.

> `flex-grow` qiymati necha bo‘lsa, element o‘sha miqdorda ko‘proq o‘sadi.


### 1. `0` (default)
➡️ Element bo‘sh joyni egallamaydi.
O‘z o‘lchamini saqlaydi va boshqa elementlar o‘sgan bo‘lsa, ular barchani qamrab oladi.

### 2. `1`
➡️ Element bo‘sh joyning 1-qismiga teng bo‘lib, o‘zgaradi.
Ya'ni, agar konteynerda bo‘sh joy bo‘lsa, bu element ko‘proq o‘sadi, lekin boshqa elementlar bilan birgalikda.

### 3. `2`
➡️ Element bo‘sh joyning 2-qismiga teng bo‘lib, o‘zgaradi.
Agar boshqa elementlarda flex-grow: 1; bo‘lsa, bu element ikkita qismga ko‘proq bo‘lishi mumkin.

### 4. `3` va boshqalar
➡️ Elementlar flex-grow qiymati 3 va undan katta bo‘lsa, ular bo‘sh joyning 3-qismiga teng o‘sadi.
Qanday qilib ko‘p joy olishini osonlik bilan tushunish mumkin: katta sonlar — ko‘proq o‘sish.

<br>

## Misol:
>Agar 3 ta element bo‘lsa va ularning flex-grow qiymatlari 1, 2, 3 bo‘lsa,
bo‘sh joy to‘liq 6 qismga bo‘linadi (1 + 2 + 3). Har bir elementga tegishli bo‘sh joy miqdori bunga qarab belgilanadi.

---

<br><br>

---

<h3 style="color:greenyellow;">flex-shrink<h3>

> Siqilish stavkasini belgilaydi, ya'ni element qancha siqilishini boshqaradi.


### 1. `1` (default)
➡️ Elementlar siqiladi, lekin ular boshqa elementlar bilan teng miqdorda siqiladi.
>Agar konteyner kichik bo‘lsa va bo‘sh joy yo‘q bo‘lsa, barcha elementlar bir xil darajada siqiladi.

### 2. `0`
➡️ Element siqilmaydi.
Agar flex-shrink: 0 bo‘lsa, bu element o‘z hajmini saqlaydi, u boshqa elementlar siqilsa ham, o‘z o‘lchamiga tegishli o‘zgarishsiz qoladi.

### 3. `2` va boshqalar
➡️ Element siqilishi 2 yoki undan ko‘p bo‘ladi, ya'ni katta sonlar — ko‘proq siqilish.
>Agar konteynerda joy etishmasa, bu element boshqalarga qaraganda ikki baravar ko‘proq siqiladi.

## Misol:
>Agar 3 ta element bo‘lsa va ularning flex-shrink qiymatlari 1, 0, 2 bo‘lsa,
bo‘sh joy yo‘q bo‘lsa, ikkinchi element siqilmaydi (0), birinchi va uchinchi elementlar esa siqiladi, lekin uchinchi element ikki baravar ko‘proq siqiladi.

---

<br><br>

---

<h3 style="color:greenyellow;">flex-basis<h3>

>Elementning asosiy `initial` o‘lchamini belgilaydi, ya'ni flex element boshlanishda qancha joy egallasin degan buyruq.
Bu qiymat flex-grow va flex-shrink ishlashidan avval hisoblanadi.

1. auto (default)
➡️ Element o‘zining content’iga yoki width/height’iga qarab o‘lcham oladi.
Agar width/height berilgan bo‘lsa — o‘sha ishlaydi, aks holda content’ga qaraydi.

2. 100px, 50%, va boshqalar
➡️ Bu yerda aniq boshlang‘ich o‘lcham beriladi.

- 100px — har bir element boshlanishda 100px joy egallaydi
- 50% — konteynerning 50 foizini egallaydi
- va hokazo

---

<br><br>

---

<h3 style="color:greenyellow;">flex<h3>

> `grow` `shrink` `basis` —  xususiyatlarini bir qatorda yozish uchun ishlatiladi:

```
flex: 1 0 100px;

/*
bu degani:
   flex-grow: 1;
   flex-shrink: 0;
   flex-basis: 100px;
*/
```
---

<br><br>

---

<h3 style="color:greenyellow;">align-self<h3>

> bitta elementga nisbatan vertikal hizalanishni belgilaydi.
Ya'ni: birgina element boshqalar bilan bir xil hizalanmaydi, o‘zi alohida turadi.

>Bu `align-items` qoidasi barcha elementlarga ta’sir qilsa, `align-self` faqat tanlangan elementga ta’sir qiladi.

## Qiymatlar:

### 1. `auto` (default)
➡️ Hech narsa qilmaydi, ya’ni align-items qiymatini meros oladi.

### 2. `flex-start`
➡️ Element konteynerning yuqori qismida joylashadi (asosiy o‘qga perpendikulyar).

### 3. `flex-end`
➡️ Element quyi (pastki) qismga joylashadi.

### 4. `center`
➡️ Element vertikal markazda hizalanadi.

### 5. `baseline`
➡️ Element matn tag chizig‘i (baseline) bo‘yicha hizalanadi.

### 6. `stretch`
➡️ Element bo‘yi konteynerni to‘liq egallaydi (agar balandlik belgilanmagan bo‘lsa).

> Bu default effekt bo‘lishi mumkin, shuning uchun ba’zida align-self: stretch; bo‘yicha cho‘ziladi.

<br>

### Misol:

```
.item1 {
  align-self: flex-end;
}
.item2 {
  align-self: center;
}
```

> Bu kodda `.item1` pastda, `.item2` markazda bo‘ladi, qolganlar esa `align-items` qoidasiga bo‘ysunadi.

---



---

<h3 style="color:greenyellow;">order<h3>

> flex elementlarning tartibini boshqaradi.
Ya’ni, HTML’da qanday ketma-ketlikda yozilganidan qat'i nazar, qaysi element birinchi, qaysi biri oxirgi chiqishini belgilaydi.

###  Default: `order: 0;`
>Agar order berilmasa, barcha elementlar 0 hisoblanadi va HTML’da qanday ketma-ket yozilgan bo‘lsa, shunday chiqadi.

### 1. `order: 1, order: 2, ...`
➡️ Katta son — keyinroq chiqadi.
Masalan, order: 2 bo‘lgan element, order: 1 bo‘lganidan keyin keladi.

### 2. `order: -1, order: -2, ...`
➡️ Manfiy son — avvalroq chiqadi.
Masalan, order: -1 bo‘lgan element, order: 0 va 1 dan ham oldin chiqadi.

```
<div class="item1" style="order: 2">1</div>
<div class="item2" style="order: -1">2</div>
<div class="item3" style="order: 1">3</div>
```

> Bu holda sahifada 2, 3, 1 tartibda chiqadi.

- Kichik order → avval chiqadi
- Katta order → keyin chiqadi

---