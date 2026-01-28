Google має безплатну онлайн-бібліотеку шрифтів, яка містить понад 1600 варіантів. На спеціальному сайті можна переглядати різні шрифти на прикладі власного тексту, щоб знайти потрібний. Потім Google Fonts дає тобі **HTML**- і **CSS**-код, за допомогою якого можна **привʼязати** або **імпортувати** шрифт на твій сайт.

### Знайди шрифт

Відкрий [fonts.google.com](https://fonts.google.com/){:target="_blank"}.

Введи якийсь текст у поле **Попередній перегляд**.

![Сторінка пошуку шрифтів Google Fonts. У полі попереднього перегляду написано «Lapis Sarawak».](images/custom.png)

**Зверни увагу**, що приклади показують твій текст. Ти можеш побачити, як твої слова виглядатимуть всіма доступними шрифтами.

Можна використати різні фільтри пошуку. Спробуй пошукати за мовою або за певними властивостями шрифтів.

Прокручуй униз, доки не знайдеш шрифт до вподоби. Якщо ти знаєш назву потрібного шрифту, введи його у головне поле пошуку.

![У полі пошуку написано «Bangers».](images/bangers.png)

**Зверни увагу**, що тепер ти бачиш слова з прикладу, написані шрифтом Bangers.

### Вибери розмір шрифту

У цьому прикладі показано розмір у 40 пікселів.

### Отримай код для вставлення

Натисни кнопку «Отримати шрифт» у верхньому правому куті.

Ти побачиш вибрані шрифти.

![Вибрані шрифти.](images/selected-font.png)

Натисни кнопку «Отримати код для вставлення».

Ти можеш скористатися методом `<link>` («посилання») або методом `<import>` («імпортування»).

### Метод посилання

![HTML-код для копіювання.](images/link.png)

Скопіюй та встав HTML-код поміж тегів `<head>` у HTML-документі.

--- code ---
---
language: html
filename: 
line_numbers: 
line_number_start: 1
line_highlights: 2-4
---

  <!-- Імпортуємо шрифти з Google -->

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bangers&display=swap" rel="stylesheet">

--- /code ---

Додай правильний CSS-код, щоби браузер знав, коли використовувати цей шрифт.

Перейди до файлу `default.css` та знайди змінні шрифту (це також може бути файл із твоєю палітрою кольорів, наприклад, `fiesta.css`).

Додай (або заміни) код вибраного шрифту. У нашому прикладі ми використовуємо `Bangers, cursive;`.

--- code ---
---
language: css
filename: default.css
line_numbers: true
line_number_start: 15
line_highlights: 16-18
---
  --body-font: 1.1rem Verdana, sans-serif;
  --header-font: lighter 3rem 'Bangers', cursive;
  --title-font: lighter 2rem 'Bangers', cursive;
  --quote-font: lighter 1.5rem 'Bangers', cursive;

--- /code ---

### Метод імпортування

![CSS-код для копіювання.](images/import.png)

Відкрий файл `style.css`.

Скопіюй і встав код імпорту на початку файлу.

Обовʼязково додай крапку з комою `;` в кінці рядка.

--- code ---
---
language: css
filename: style.css
line_numbers: 
line_number_start: 
line_highlights:
---

@import url('https://fonts.googleapis.com/css2?family=Bangers&display=swap');

--- /code ---

Відкрий файл `default.css` та знайди змінні шрифту (це також може бути файл із твоєю палітрою кольорів, наприклад, `fiesta.css`).

Додай (або заміни) код вибраного шрифту. У нашому прикладі ми використовуємо `Bangers, cursive;`.

--- code ---
---
language: css
filename: default.css
line_numbers: true
line_number_start: 15
line_highlights: 16-18
---
  --body-font: 1.1rem Verdana, sans-serif;
  --header-font: lighter 3rem 'Bangers', cursive;
  --title-font: lighter 2rem 'Bangers', cursive;
  --quote-font: lighter 1.5rem 'Bangers', cursive;

--- /code ---