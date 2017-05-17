# Заметки к курсу по Реакту
## Домашки
Мои домашки лежат в [форке `js_ru_20_04_19_30`](https://github.com/amiskov/js_ru_20_04_19_30). На компе репа лежит в `~/Projects/edu/js_ru_20_04_19_30`.

## Тулзы
* [ReactDevTools](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=ru)
* [Live Templates form JetBrains IDEs](https://github.com/minwe/jetbrains-react) — установил.

## Как обновлять форкнутый репозиторий
В [форкнутой репе](https://github.com/amiskov/js_ru_20_04_19_30) есть 2 ремоута:
* `remotes/origin` — мой
* `remotes/romabelka/master` — оригинальный

```bash
git fetch romabelka # достаем апдейты из оригинального удаленного репозитория
git co master # идем в мастер своего форка
git merge romabelka/master # обновляемся из мастера оригинальной репы
```
