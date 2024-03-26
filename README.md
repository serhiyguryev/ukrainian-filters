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

> Цей фільтр видаляє скрипти та html-елементи систем коментування (Disqus, Facebook Comments Plugin тощо) на новинних та деяких інших сайтах. Якщо для вас це неприйнятно, не використовуйте цей фільтр.

```
https://www.awwwwesome.org/data/filters/UF/privacy.txt
```

### Ukrainian Security Filter (Український безпековий фільтр)

Це [фільтр шкідливих веб-ресурсів](https://github.com/braveinnovators/ukrainian-security-filter) (фішинг, онлайн-шахрайство, шкідливе програмне забезпечення тощо), що орієнтовані на громадян України.

> На відміну від трьох вищезгаданих фільтрів, цей фільтр сумісний з усіма браузерами, розширеннями та іншим програмним забезпеченням, що підтримує синтаксис AdBlock (див. розділ «Сумісність з браузерами та розширеннями»).

```
https://www.awwwwesome.org/data/filters/USF/adblock.txt
```

## Сумісність з браузерами та розширеннями

Фільтри `Ukrainian Ad Filter`, `Ukrainian Annoyance Filter` та `Ukrainian Privacy Filter` створені з використанням специфічного синтаксису фільтрації розширення [uBlock Origin](https://github.com/gorhill/uBlock) (uBO), при цьому, більшість правил фільтрації все ж сумісні як з іншими популярними сторонніми розширеннями, так і з браузерами з вбудованими модулями фільтрації контенту.

Однак, з точки зору ефективності, приватності та безпеки, найбільш оптимальним для користувачів персональних комп'ютерів буде використання розширення [uBlock Origin](https://ublockorigin.com/) разом з браузером [Firefox](https://www.mozilla.org/firefox/) (якщо ви не плануєте змінювати браузер, все одно розгляньте можливість встановлення саме розширення uBlock Origin).

Браузер Firefox підтримує роботу розширень і на мобільних пристроях, проте, розширення uBlock Origin працює лише на ОС Android. Тому альтернативою для мобільних пристроїв, що працюють на базі ОС Android та iOS, може стати використання браузера [Brave](https://brave.com/), який має власний модуль фільтрації контенту.

> Починаючи з версії 0.5, розробники розширення **Adblock** [вирішили прибрати](https://web.archive.org/web/20111206122411/http://adblockplus.org/en/faq_features#siteblock) функцію блокування веб-сторінок (strict blocking). Це означає, що ані **Adblock**, ані **Adblock Plus** не можуть блокувати доступ до шкідливих веб-ресурсів на рівні доменного ім'я. Розширення **AdGuard** так само має проблеми з обробкою правил фільтрації ([Issue #2760](https://github.com/AdguardTeam/AdguardBrowserExtension/issues/2760)), навіть тих, що прямо прописані в документації цього розширення. Відповідно, ці розширення не можуть забезпечити обробку правил фільтрації, що повністю відповідають вимогам сучасних версій синтаксису Adblock, тому вони не є сумісними з фільтром `Ukrainian Security Filter (Український безпековий фільтр)`.

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

## Співпраця

Якщо ви створили правила фільтрації та бажаєте, щоб вони були додані до профільних списків фільтрів, ви можете створити **fork** проекту та додати їх до файлів (списків) з відповідними фільтрами (`ads.txt`, `annoyances.txt` або `privacy.txt`), що містяться в окремій директорії під назвою `sandbox`. Потім ви створюєте **commit** і, після проходження тестування, ваші правила будуть додані до профільних списків фільтрів безпосередньо мейнтейнерами проекту із зазначенням авторства.

При додаванні нових правил фільтрації до файлів ads.txt, annoyances.txt або privacy.txt, що містяться у директорії sandbox, слід керуватися наступними стандартами (стилями), що застосовуються при створенні нових правил фільтрації:

```adblock
! Веб-адреса (URL-адреса) веб-ресурсу, щодо якого будуть застосовані правила фільтрації
example.com##rule1
example.com##rule2
example.com##rule3
```

## Підтримати проект

Ви можете підтримати подальший розвиток цього проекту, обравши зручний для вас спосіб перерахування донатів:

* **Дебетова/кредитна картка**: [https://donatello.to/serhiyguryev](https://donatello.to/serhiyguryev)
* **Bitcoin (BTC)**: bc1q6qtnwc2pdktvl48mr9hf0qmhaxfm7xseftp78a
* **Ether (ETH)**: 0x185e4FB1f662223B011dedbBd42A444891b094f5

## Ліцензія

На Ukrainian Filters (Українські фільтри) поширюються умови ліцензії [GNU General Public License v3.0](https://github.com/serhiyguryev/ukrainian-filters/blob/main/LICENSE)
