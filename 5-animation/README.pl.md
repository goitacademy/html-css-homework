**Read in other languages: [Russian](README.md), [Ukrainian](README.ua.md),
[English](README.en.md), [Spanish](README.es.md), [Polish](README.pl.md).**

# Zadanie domowe

- Utwórz repozytorium `goit-markup-hw-05`.
- Sklonuj utworzone repozytorium i skopiuj do niego pliki poprzedniej pracy.
- Dodaj animację efektów dekoracyjnych do stron układu
  [**zadania domowego #5**](https://www.figma.com/file/SqiyweSseH96c3wVZmnGfq/Zadanie-domowe-GOIT-Polska?node-id=3334%3A3).
- Skonfiguruj `GitHub Pages` i dodaj link do aktywnej strony do nagłówka
  repozytorium GitHub.

## Kryteria akceptacji projektu przez mentora

### Projekt

**`«A1»`** Wszystkie style są zapisane w jednym pliku `styles.css`, który
znajduje się w folderze `css`.

**`«A2»`** Kod źródłowy jest sformatowany za pomocą `Prettier`.

**`«A3»`** Wszystkie obrazy i zawartość tekstowa są z układu.

**`«A4»`** Wszystkie strony HTML mają normalizator stylu
[`modern-nomalize`](https://github.com/sindresorhus/modern-normalize).

**`«A5»`** Kod jest napisany zgodnie z [**tutorialem**](https://codeguide.co/).

**`«A6»`** Skrypt do okna modalnego jest zawarty w HTML w oddzielnym pliku
`modal.js`.

### Znaczniki HTML

**`«B1»`** Wykonane jest oznaczenie znacznikami HTML wszystkich elementów
układu.

**`«B2»`** Tagi są używane zgodnie z ich znaczeniem semantycznym.

### Stylizacja

**`«C1»`** Dla wszystkich efektów najechania kursorem i focusu (kolor, tło,
cień) wykonywany jest `transition`. Czas - `250ms`, funkcja rozkładu czasu -
`cubic-bezier(0.4, 0, 0.2, 1)`.

**`«C2»`** Właściwości, które będą animowane są wyraźnie określone w przejściach
i animacjach. Nigdzie nie ma wartości `all`.

**`«C3»`** W sekcji `Czym się zajmujemy` tekst z tłem jest umieszczony nad
obrazem.

**`«C4»`** W głównej nawigacji, używając pseudoelementu `::after`, podkreślono
link do bieżącej strony (na której obecnie jest użytkownik).

**`«C5»`** Niebieska nakładka z tekstem na kartach strony `Portfolio` pojawia
się po najechaniu kursorem w dowolne miejsce na karcie. W każdej karcie jest
tekst jak w pierwszym przykładzie.

**`«C6»`** Niebieska nakładka na kartach strony `Portfolio` wysuwa się z dołu,
jak pokazano [w wideo](./preview.gif).

**`«C7»`** Pseudoelementy nie mają treści tekstowej we właściwości `content`.
Używane są wyłącznie do celów dekoracyjnych.

### Okno modalne

**`«D1»`** Ukończono oznaczanie i dekoracja «backdrop» (ciemnego
półprzezroczystego tła) okna modalnego.

**`«D2»`** «Backdrop» (tło) wypełnia 100% wysokości i szerokości okna
przeglądarki i jest w nim stałe.

**`«D3»`** Ukończono oznaczenie znacznikami HTML i dekorację okna modalnego.

**`«D4»`** Okno modalne jest umieszczone pionowo i poziomo na środku tła
(backdrop).

**`«D5»`** Ukończono oznaczenie znacznikami HTML i dekorację przycisku do
zamykania okna modalnego w prawym górnym rogu.

**`«D6»`** Początkowo okno modalne i backdrop są ukrywane za pomocą klasy
`is-hidden` w backdropie, w selektorze tego elementu używa się właściwości
`visibility`, `opacity` i `pointer-events`.

**`«D7»`** Jeśli usuniesz klasę `is-hidden` z backdrop - pojawi się backdrop i
okno modalne.

**`«D8»`** Pojawienie się i zniknięcie okna modalnego jest animowane przy użyciu
przejścia z dowolnym efektem, takim jak `scale` lub `translate`, i `opacity`.

## Otwieranie/zamykanie okna modalnego

Okno modalne z formularzem zgłoszeniowym otwiera się po kliknięciu na przycisk
`"Zamów usługę"`. Aby skrypt działał, musisz dodać specjalne atrybuty do
znaczników HTML, po których skrypt wyszukuje elementy:

- `data-modal-open` - do przycisku otwierania okna modalnego.
- `data-modal-close` - do przycisku zamykania okna modalnego.
- `data-modal` - do backdrop okna modalnego.

Następnie przed zamykającym tagiem `body` dodaj tag `script` z linkiem do pliku
skryptu okna modalnego. Możesz obejrzeć [instrukcję wideo]
(https://drive.google.com/file/d/1XRqb6W_MObwfcp2psCFLUz7of-hc2NhU/view?usp=sharing).

```html
<body>
  <!-- Wszystkie Twoje znaczniki HTML, w tym znaczniki okna modalnego  -->

  <!-- Umieść przed zamykającym tagiem body -->
  <script src="./js/modal.js"></script>
</body>
```

Skrypt do skopiowania i wklejenia do pliku `modal.js`.

```js
(() => {
  const refs = {
    openModalBtn: document.querySelector('[data-modal-open]'),
    closeModalBtn: document.querySelector('[data-modal-close]'),
    modal: document.querySelector('[data-modal]'),
  };

  refs.openModalBtn.addEventListener('click', toggleModal);
  refs.closeModalBtn.addEventListener('click', toggleModal);

  function toggleModal() {
    refs.modal.classList.toggle('is-hidden');
  }
})();
```
