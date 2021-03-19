**Czytaj w innych językach: [Rosyjski](README.md), [Ukraiński](README.ua.md),
[Polski](README.pl.md).**

# Zadanie domowe

- Utwórz repozytorium `goit-markup-hw-02`.
- Sklonuj utworzone repozytorium i skopiuj do niego pliki poprzedniej pracy.
- Wykonaj znaczniki HTML i projektowanie układu strony
  [**zadania domowego #2**](<https://www.figma.com/file/oTYBECAN79dXy19hzWObO4/Web-Studio-(Version-2.1)?node-id=1%3A94>).
- Do optymalizacji obrazów skorzystaj z usługi
  [**squoosh**](https://squoosh.app/).
- Skonfiguruj `GitHub Pages` i dodaj link do aktywnej strony do nagłówka
  repozytorium GitHub.

## Kryteria akceptacji projektu przez mentora

### Projekt

**`«A1»`** W katalogu głównym projektu znajduje się folder `images` z obrazami.

**`«A2»`** W katalogu głównym projektu znajduje się folder `css` z plikami stylów. 

**`«A3»`** Wszystkie style są zapisane w jednym pliku `styles.css`, który znajduje się 
w folderze `css`.

**`«A4»`** W nazwach plików nie ma wielkich liter, spacji i transliteracji, 
a jedynie litery i słowa w języku angielskim. 

**`«A5»`** Kod źródłowy jest sformatowany za pomocą `Prettier`.

**`«A6»`** Wszystkie obrazy i zawartość tekstowa są z układu. 

**`«A7»`** Wszystkie mapy bitowe są optymalizowane przy użyciu 
[squoosh](https://squoosh.app/).

**`«A8»`** Kod jest napisany zgodnie z
[**tutorialem**](http://sadcitizen.me/code-guide/).

### Znaczniki HTML

**`«B1»`** Znaczniki HTML strony `Portfolio` wpisują się w pliku `portfolio.html`.

**`«B2»`** Wykonane są znaczniki HTML wszystkich elementów układu. 

**`«B3»`** Tagi są używane zgodnie z ich znaczeniem semantycznym. 

**`«B4»`** HTML jest weryfikowany przez [**walidator**](http://validator.w3.org/nu/)
bez błędów.

**`«B5»`** Nazwy klas są opisowe i zrozumiałe dla innego programisty. 

**`«B6»`** Nazwy klas nie zawierają wielkich liter, spacji, transliteracji i 
nazw tagów, a jedynie litery i słowa w języku angielskim. Jeśli nazwa klasy składa 
się z kilku słów, są one oddzielone myślnikiem. 

**`«B7»`** Atrybut `href` linków nawigacyjnych `Studio` i `Portfolio` zawiera
względną ścieżkę do plików HTML tych stron. Kliknięcie linku powoduje przejście 
do odpowiedniej strony w bieżącej karcie przeglądarki.  

**`«B8»`** Tagi `<img>` mają atrybuty wymiarów, co najmniej `width`.

**`«B9»`** Obrazy są wyeksportowane z układu w formacie `jpg`.

**`«B10»`** Grupy elementów tego samego typu są gromadzone na listach `<ul>`.

**`«B11»`** Filtr na stronie `Portfolio` jest tworzony przez listę przycisków, 
z których każdy ma ustawiony atrybut `type="button"`.

**`«B12»`** Znaczniki nagłówka i stopki są takie same na wszystkich stronach. 

**`«B13»`** Wszystkie czcionki i ich odmiany wymagane dla układu (grubość i styl) 
są podłączone z usługi Google Fonts za pomocą jednego linku. Wymagana waga dla `Raleway` –
700, a dla `Roboto` – 400, 500, 700 i 900.

**`«B14»`** Wewnątrz znaczników przycisku nie ma żadnych dodatkowych elementów, 
takich jak spany lub linki. 

## Оформление

**`«C1»`** Нет глобальных стилей элементов кроме `<body>`.

**`«C2»`** Для оформления используются селекторы класса.

**`«C3»`** В стилях отсутствует `!important`.

**`«C4»`** У интерактивных элементов (кнопок и ссылок), при наведении мышкой или
фокусе с клавиатуры, есть активное состояние указанное в макете (изменение
цвета).

**`«С5»`** Текст контактов в хедере и футере меняет цвет при ховере и фокусе.

**`«C6»`** Для хранения палитры цветов макета (текст, фон, выделение)
используются CSS-переменные.

**`«С7»`** Для элемента `<body>` задано свойство `font-family` с доминантным на
макете шрифтом `Roboto`.

**`«С8»`** Указаны альтернативные варианты шрифта и тип семейства (без засечек)
в конце перечисления `font-family` у элемента `<body>`.

**`«С9»`** Семейство шрифтов `Roboto` явно задано только для элемента `<body>`,
остальные элементы наследуют его.

**`«С10»`** Для элемента `<body>` задано свойство `color` с доминантным на
макете цветом текста. Остальной текст наследует или переопределяет это значение.

**`«С11»`** Размер шрифта (свойство `font-size`) всех текстовых элементов точно
соответствует значениям из макета.

**`«С12»`** Высота строки (свойство `line-height`) всех текстовых элементов
точно соответствует значениям из макета и задана как множитель, а не в `px`.

**`«С13»`** Цвет (свойство `color`) всех текстовых элементов точно соответствует
значениям из макета.

**`«С14»`** Вес шрифта (свойство `font-weight`) всех текстовых элементов точно
соответствует значениям из макета.

**`«С15»`** Вес шрифта (свойство `font-weight`) явно указан только если значение
в макете отличается от стандартного для этого элемента в браузере.

**`«С16»`** Кнопкам задано свойство `cursor` со значением `pointer`.

**`«С17»`** В стилях не повторяются значения свойств, которые заданы браузером
по умолчнаию. Например, ссылкам не нужно указывать `cursor: pointer`, а абзацам
`font-style: normal` или `font-weight: 400`.
