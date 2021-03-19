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

## Stylizacja

**`«C1»`** Nie ma stylów globalnych dla elementów innych niż `<body>`.

**`«C2»`** Do stylizacji służą selektory klasy.

**`«C3»`** W stylach nie ma `!important`.

**`«C4»`** Elementy interaktywne (przyciski i linki) po najechaniu myszką 
lub focusie z klawiatury mają stan aktywny wskazany w układzie 
(zmiana koloru). 

**`«С5»`** Tekst kontaktów w nagłówku i stopce zmienia kolor po najechaniu kursorem i focusie. 

**`«C6»`** Do przechowywania palety kolorów układu (tekst, tło, zaznaczenie)
używane są zmienne CSS. 

**`«С7»`** Element `<body>` ma właściwość `font-family` z dominującą czcionką
`Roboto` w układzie.

**`«С8»`** Alternatywne opcje czcionek i typ rodziny (bezszeryfowa) są określone 
na końcu wyliczenia `font-family` dla elementu `<body>`.

**`«С9»`** Rodzina czcionek `Roboto` jest wyraźnie określona tylko dla elementu `<body>`,
pozostałe elementy go dziedziczą. 

**`«С10»`** Element `<body>` ma właściwość `color` z dominującym w 
układzie kolorem tekstu. Reszta tekstu dziedziczy lub zastępuje tę wartość. 

**`«С11»`** Rozmiar czcionki (właściwość `font-size`) wszystkich elementów tekstowych 
dokładnie odpowiada wartościom z układu. 

**`«С12»`** Wysokość wiersza (właściwość `line-height`) wszystkich elementów tekstowych
dokładnie odpowiada wartościom z układu i jest określona jako mnożnik, a nie w `px`.

**`«С13»`** Kolor (właściwość `color`) wszystkich elementów tekstowych dokładnie 
odpowiada wartościom z układu. 

**`«С14»`** Waga czcionki (właściwość `font-weight`) wszystkich elementów tekstowych 
dokładnie odpowiada wartościom z układu. 

**`«С15»`** Waga czcionki (właściwość `font-weight`) jest wyraźnie określona tylko wtedy, gdy wartość
w układzie różni się od domyślnej dla tego elementu w przeglądarce. 

**`«С16»`** Przyciski mają określoną właściwość `cursor` z wartością `pointer`.

**`«С17»`** W stylach nie powtarza się domyślnych wartości właściwości ustawionych przez 
przeglądarkę. Na przykład, linki nie muszą mieć `cursor: pointer`, akapity nie muszą mieć
`font-style: normal` lub `font-weight: 400`.
