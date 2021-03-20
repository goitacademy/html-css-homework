**Czytaj w innych językach: [Rosyjski](README.md), [Ukraiński](README.ua.md),
[Polski](README.pl.md).**

# Zadanie domowe

- Utwórz repozytorium `goit-markup-hw-05`.
- Sklonuj utworzone repozytorium i skopiuj do niego pliki poprzedniej pracy. 
- Dodaj animację efektów dekoracyjnych do stron układu
  [**zadania domowego #5**](<https://www.figma.com/file/oTYBECAN79dXy19hzWObO4/Web-Studio-(Version-2.1)?node-id=1%3A836>).
- Skonfiguruj `GitHub Pages` i dodaj link do aktywnej strony do 
  nagłówka repozytorium GitHub. 

## Kryteria akceptacji projektu przez mentora

### Projekt

**`«A1»`** Wszystkie style są zapisane w jednym pliku `styles.css`, który znajduje się 
w folderze `css`.

**`«A2»`** Kod źródłowy jest sformatowany za pomocą `Prettier`.

**`«A3»`** Wszystkie obrazy i zawartość tekstowa są z układu.

**`«A4»`** Wszystkie strony HTML mają normalizator stylu 
[`modern-nomalize`](https://github.com/sindresorhus/modern-normalize).

**`«A5»`** Kod jest napisany zgodnie z
[**tutorialem**](http://sadcitizen.me/code-guide/).

**`«A6»`** Skrypt do okna modalnego jest zawarty w HTML w oddzielnym pliku `modal.js`.

### Znaczniki HTML

**`«B1»`** Wykonane są znaczniki HTML wszystkich elementów układu. 

**`«B2»`** Tagi są używane zgodnie z ich znaczeniem semantycznym. 

### Stylizacja

**`«C1»`** Для всех эффектов ховера и фокуса (цвет, фон, тень) сделаны переходы.
Время - `250ms`, функция распределения времени - `cubic-bezier(0.4, 0, 0.2, 1)`.

**`«C2»`** В переходах и анимациях явно указаны анимируемые свойства. Нигде нет
значения `all`.

**`«C3»`** В секции `Чем мы занимаемся` текст с фоном спозиционирован поверх
изображения.

**`«C4»`** В главной навигации, при помощи псевдоэлемента `::after`, сделано
подчёркивание ссылки текущей страницы (на которой сейчас находится
пользователь).

**`«C5»`** Синий оверлей с текстом на карточках страницы `Портфолио` появляется
при ховере в любом месте карточки.

**`«C6»`** Синий оверлей в карточках страницы `Портфолио` выезжает снизу, как
показано [на видео](./preview.gif).

**`«C7»`** У псевдоэлементов нет текстового контента в свойстве `content`. Они
использованы исключительно для декоративного оформления.

### Модальное окно

**`«D1»`** Выполнена разметка и оформление «бекдропа» (тёмного полупрозрачного
фона) модального окна.

**`«D2»`** «Бекдроп» заполняет 100% высоты и ширины вьюпорта браузера и
фиксирован в нём.

**`«D3»`** Выполнена разметка и оформление модального окна.

**`«D4»`** Модальное окно вертикально и горизонтально спозиционировано
посередине бекдропа.

**`«D5»`** Выполнена разметка и оформление кнопки закрытия модального окна в
верхнем правом углу.

**`«D6»`** Изначально модальное окно и бекдроп скрыты при помощи класса
`is-hidden` на бекдропе, в селекторе которого используются свойства
`visibility`, `opacity` и `pointer-events`.

**`«D7»`** Если убрать с бекдропа класс `is-hidden` - появляется бекдроп и
модальное окно.

**`«D8»`** Появление и скрытие модального окна анимировано при помощи перехода с
произвольным эффектом, например `scale` или `translate`, и `opacity`.

## Открытие/закрытие модального окна

Модальное окно с формой заявки открывается по клику на кнопку
`"Заказать услугу"`. Для того чтобы скрипт сработал необходимо добавить в
разметку специальные атрибуты, по которым скрипт ищет элементы:

- `data-modal-open` - на кнопку открытия модального окна.
- `data-modal-close` - на кнопку закрытия модального окна.
- `data-modal` - на бекдроп модального окна.

После чего, перед закрывающим тегом `body` добавить тег `script` со ссылкой на
файл скрипта для модально окна. Можно посмотреть
[видео-инструкцию](https://drive.google.com/file/d/1yasixN2K-9DdsYtKCJWVay9WbyTZai0t/view?usp=sharing).

```html
<body>
  <!-- Вся твоя разметка, включая разметку модалки -->

  <!-- Ставим перед закрывающим тегом body -->
  <script src="./js/modal.js"></script>
</body>
```

Скрипт который необходимо скопировать и вставить в файл `modal.js`.

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
