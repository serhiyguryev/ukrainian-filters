# Ukrainian Filters

Ukrainian Filters (Українські фільтри) — це веб-фільтри, які автоматично видаляють небажаний контент з українських сайтів, включно з рекламою, дратівливими елементами, трекерами та шкідливими скриптами.

## Фільтри

### Ukrainian Ad Filter

Фільтр видаляє рекламу з українських сайтів.

```
https://www.awwwwesome.org/data/filters/UF/ads.txt
```

### Ukrainian Annoyance Filter

Фільтр блокує дратівливі елементи на українських та деяких популярних іноземних сайтах (повідомлення про файли cookie, спливаючі вікна, банери тощо).

```
https://www.awwwwesome.org/data/filters/UF/annoyances.txt
```

### Ukrainian Privacy Filter

Фільтр блокує трекери та шкідливі скрипти, зменшує можливість третіх сторін збирати дані про вашу поведінку в Інтернеті.

**Увага**: цей фільтр видаляє скрипти та html-елементи систем коментування (Disqus, Facebook Comments Plugin тощо) на новинних та деяких інших сайтах. Якщо для вас це неприйнятно, не використовуйте цей фільтр.

```
https://www.awwwwesome.org/data/filters/UF/privacy.txt
```

### Ukrainian Security Filter (Український безпековий фільтр)

Це [фільтр шкідливих веб-ресурсів](https://github.com/braveinnovators/ukrainian-security-filter) (фішинг, онлайн-шахрайство, шкідливе програмне забезпечення тощо), що орієнтовані на громадян України. На відміну від трьох вищезгаданих фільтрів, цей фільтр сумісний з усіма браузерами, розширеннями та іншим програмним забезпеченням, що підтримує синтаксис AdBlock (див. розділ «Сумісність з браузерами та розширеннями»).

```
https://www.awwwwesome.org/data/filters/USF/adblock.txt
```

## Сумісність з браузерами та розширеннями

Фільтри `Ukrainian Ad Filter`, `Ukrainian Annoyance Filter` та `Ukrainian Privacy Filter` створені з використанням специфічного синтаксису фільтрації розширення [uBlock Origin](https://github.com/gorhill/uBlock) (uBO), при цьому, більшість правил фільтрації все ж сумісні як з іншими популярними сторонніми розширеннями, так і з браузерами з вбудованими модулями фільтрації контенту.

Однак, з точки зору ефективності, приватності та безпеки, найбільш оптимальним для користувачів персональних комп'ютерів буде використання розширення [uBlock Origin](https://ublockorigin.com/) разом з браузером [Firefox](https://www.mozilla.org/firefox/) (якщо ви не плануєте змінювати браузер, все одно розгляньте можливість встановлення саме розширення uBlock Origin).

Браузер Firefox підтримує роботу розширень і на мобільних пристроях, проте, розширення uBlock Origin працює лише на ОС Android. Тому альтернативою для мобільних пристроїв, що працюють на базі ОС Android та iOS, може стати використання браузера [Brave](https://brave.com/), який має власний модуль фільтрації контенту та вбудовані різноманітні функції захисту.

### Як імпортувати фільтри

#### Brave

<details>
<summary>Windows, macOS та Linux</summary>

1. У меню `Settings` відкрити вкладку `Shields` й змінити налаштування `Trackers & ads blocking` на `Aggressive`
2. У вкладці `Shields` відкрити розділ `Content filtering` і у розділі `Add custom filter lists` у поле вводу вставити скопійовані адреси необхідних фільтрів.
</details>

<details>
<summary>Android та iOS</summary>

1. У меню `Settings` відкрити розділ меню `Brave Shields & privacy` й змінити налаштування `Block trackers & ads` на `Aggressive`
2. У розділі меню `Brave Shields & privacy` відкрити `Content filtering`, далі `Add custom filter list` і у поле вводу вставити скопійовані адреси необхідних фільтрів, зберігши зміни шляхом натискання на кнопку `Add`.
</details>

#### uBlock Origin

<details>
<summary>Windows, macOS та Linux</summary>

1. Відкрити меню `Preferences` розширення uBlock Origin, клацнути мишею на вкладку `Filter lists` і прокрутити до розділу `Custom`
2. Клацнути мишею на `Import...` і у поле вводу вставити скопійовані адреси необхідних фільтрів, зберігши зміни.

Додаткова інструкція доступна за адресою: [https://github.com/gorhill/uBlock/wiki/Filter-lists-from-around-the-web](https://github.com/gorhill/uBlock/wiki/Filter-lists-from-around-the-web)
</details>

## Підтримати проект

Ви можете підтримати подальший розвиток цього проекту, обравши зручний для вас спосіб перерахування донатів:

* Bitcoin: bc1q6qtnwc2pdktvl48mr9hf0qmhaxfm7xseftp78a
* Ethereum: 0x185e4FB1f662223B011dedbBd42A444891b094f5

## Ліцензія

На Ukrainian Filters (Українські фільтри) поширюються умови ліцензії [GNU General Public License v3.0](https://github.com/spicy-pixels/ultimatelist/blob/main/LICENSE)
