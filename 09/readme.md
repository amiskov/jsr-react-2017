# Занятие №9, 1 июня

## Локализация
[react-intl](https://github.com/yahoo/react-intl) от Yahoo

## TypeScript + Redux
Говорит, что боль. Не любит ТайпСкрипт. Простой интеграции с Редаксом нет.

Советует Flow для типизации, но специализированно под Реакт и работает лучше в экосистеме Реакт.

Короче, в Реакте не нужен ТайпСкрипт.

Flow/TypeScript — статическая типизация, на этапе написание кода.
ПропТайпсы — в рантайме, динамическая.

[redux-form](http://redux-form.com/6.7.0/) — для форм на Реакте.

## saga
Редакт хорош, когда синхронный поток данных.

При сайд эффектах ФП дает слабину. Их надо обрабатывать отдельно. Для этого есть инструменты. Мы разбирали redux-thunk. Есть еще redux-saga — он сложный это для продвинутых.

## redux orm
Не стабильно, не советует.

##
Пропсы — основной механизм передачи данных. Явно их передаем.

`context` — такие себе глобальные переменные для Реакта.

## Вебпак для прода

## Серверный рендер
Relay + GraphQL + React — там норм. Иначе очень сложно.

https://www.youtube.com/watch?v=Y30z17PSnTk&list=LLea6gGvMo_HLrNYQUkgBB9A — доклад Романа про это.

GraphQL — мощный инструмент запроса к серверу.

## ReactNative
В основном 1 код-бейз для Айос и Андроид.

Если в браузере все синхронно, то в Нейтиве — многопоточная система: UI, JS. И поэтому есть особенности.

## SEO
 
