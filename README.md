# Ukrainian Filters

Ukrainian Filters (Українські фільтри) — це веб-фільтри, які автоматично видаляють небажаний контент з українських сайтів, включно з рекламою, дратівливими елементами, трекерами та шкідливими скриптами.

## Фільтри

**Ukrainian Ad Filter** — видаляє рекламу з українських сайтів.

```
https://www.awwwwesome.org/data/filters/UF/ads.txt
```

**Ukrainian Annoyance Filter** — блокує дратівливі елементи на українських та деяких популярних іноземних сайтах (повідомлення про файли cookie, спливаючі вікна, банери тощо).

```
https://www.awwwwesome.org/data/filters/UF/annoyances.txt
```

**Ukrainian Privacy Filter** — блокує трекери та шкідливі скрипти, зменшує можливість третіх сторін збирати дані про вашу поведінку в Інтернеті.

```
https://www.awwwwesome.org/data/filters/UF/privacy.txt
```

**Ukrainian Security Filter (Український безпековий фільтр)** — це фільтр шкідливих веб-ресурсів (фішинг, онлайн-шахрайство, шкідливе програмне забезпечення тощо), що орієнтовані на громадян України. Фільтр створений та підтримується командою громадської організації «[Соціальні інноватори](https://github.com/braveinnovators/ukrainian-security-filter)». На відміну від трьох вищезгаданих фільтрів, цей фільтр сумісний з усіма браузерами, розширеннями та іншим програмним забезпеченням, що підтримує синтаксис AdBlock (див. розділ «Сумісність з браузерами та розширеннями»).

```
https://www.awwwwesome.org/data/filters/USF/adblock.txt
```

### Сумісність з браузерами та розширеннями

Фільтри Ukrainian Ad Filter, Ukrainian Annoyance Filter та Ukrainian Privacy Filter створені з використанням специфічного синтаксису фільтрації розширення [uBlock Origin](https://github.com/gorhill/uBlock) (uBO), при цьому, більшість правил фільтрації все ж сумісні як з іншими популярними сторонніми розширеннями (наприклад, [Adblock Plus](https://adblockplus.org/)), так і з браузерами з вбудованими модулями фільтрації контенту ([Brave](https://brave.com/), [Vivaldi](https://vivaldi.com/)).

Однак, з точки зору ефективності, приватності та безпеки, найбільш оптимальним є використання розширення [uBlock Origin](https://ublockorigin.com/) разом з браузером [Firefox](https://www.mozilla.org/firefox/).

### Як імпортувати фільтри

#### uBlock Origin

<details>
<summary>Windows, macOS та Linux</summary>

1. Відкрити меню `Preferences` розширення uBlock Origin, клацнути мишею на вкладку `Filter lists` і прокрутити до розділу `Custom`
2. Клацнути мишею на `Import...` і у поле вводу вставити скопійовані адреси необхідних фільтрів, зберігши зміни.

Додаткова інструкція доступна за адресою: [https://github.com/gorhill/uBlock/wiki/Filter-lists-from-around-the-web](https://github.com/gorhill/uBlock/wiki/Filter-lists-from-around-the-web)
</details>

#### Adblock Plus

<details>
<summary>Windows, macOS та Linux</summary>

1. Відкрити меню налаштування розширення Adblock Plus, клацнути мишею на вкладку `Advanced` і прокрутити до розділу `My filter list`
2. У поле вводу вставити скопійовані адреси необхідних фільтрів, зберігши зміни.

Додаткова інструкція доступна за адресою: [https://help.adblockplus.org/hc/en-us/articles/360062859913-Add-a-custom-filter](https://help.adblockplus.org/hc/en-us/articles/360062859913-Add-a-custom-filter)
</details>

#### Brave

<details>
<summary>Windows, macOS та Linux</summary>

1. У меню `Settings` відкрити вкладку `Shields` й змінити налаштування `Trackers & ads blocking` на `Aggressive`
2. У вкладці `Shields` відкрити розділ `Content filtering` і у розділі `Add custom filter lists` у поле вводу вставити скопійовані адреси необхідних фільтрів.
</details>

<details>
<summary>Android та iOS</summary>

1. У меню `Settings` відкрити розділ меню `Brave Shields & privacy` й змінити налаштування `Block trackers & ads` на `Aggressive`
2. Вийти з меню, відкрити нову вкладку та ввести наступну адресу: `brave://adblock`
3. Перейти до розділу `Subscribe to filter list`, натиснути на кнопку `Add filter list via URL` і у поле вводу вставити скопійовані адреси необхідних фільтрів, зберігши зміни шляхом натискання на кнопку `Submit`.

Додаткова інструкція доступна за адресою: https://brave.com/privacy-updates/10-custom-filter-lists/
</details>

#### Vivaldi

<details>
<summary>Windows, macOS та Linux</summary>

1. Перейдіть у `Налаштування` > `Приватність` > `Блокування трекерів та реклами` > `Показати списки`
2. Натисніть на кнопку `Додати список`, вставте скопійовані адреси необхідних фільтрів та натисніть кнопку `Імпорт`.

Додаткова інструкція доступна за адресою: [https://help.vivaldi.com/uk/desktop-uk/privacy-uk/tracking-and-ad-blocking/](https://help.vivaldi.com/uk/desktop-uk/privacy-uk/tracking-and-ad-blocking/)
</details>

## Підтримати проект

Ви можете підтримати подальший розвиток цього проекту, обравши зручний для вас спосіб перерахування донатів:

* [PayPal або дебетова/кредитна картка](https://www.paypal.com/donate/?hosted_button_id=AQ9BB34WHFADC)
* [Платформа Ko-fi](https://ko-fi.com/serhiyguryev)

<a href="https://ko-fi.com/serhiyguryev" title="Support me on Ko-fi"><img src="assets/kofi_bg_tag_white.svg" alt="Support me on Ko-fi" width="200px" style="display: inline-block; margin: 5px 0;"></a>

## Ліцензія

На Ukrainian Filters (Українські фільтри) поширюються умови ліцензії [GNU General Public License v3.0](https://github.com/spicy-pixels/ultimatelist/blob/main/LICENSE)
