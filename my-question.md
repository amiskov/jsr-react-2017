# Мои вопросы
## ✅ Делать ли всегда компоненты на классах?
Нужно использовать функциональные компоненты когда возможно:

> Это можно сделать Functional Component, по возможности используй их

> А как же консистентность кода? Чтоб все было однотипно.

Не нужна она тут. Надо, чтоб чем проще, тем лучше. Меньше памяти, проще тестировать. Функции проще классов.

## Синтаксис декораторов ES7
Попробовать [синтаксис](https://github.com/wycats/javascript-decorators) ES7 [декораторов](https://medium.com/@goncalvesjoao/react-es7-decorators-how-to-inject-props-to-your-render-method-27a0a7973106): `@accordion`.

## Свойства класса как анонимные функции-стрелки
Часто в Реактовских компонентах вместо методовю юзают свойства с лямбдами:

```jsx harmony
class MyClass {
    updatePropFunc = () => { // часто делают так
        this.setState({
            counter: this.stage.counter + 1
        })
    };
    
    updateMethod() { // ...вместо такого
        this.setState({
            counter: this.stage.counter + 1
        })
    }
}
```

См. [Class properties transform](http://babeljs.io/docs/plugins/transform-class-properties/) на Бабеле.

* `updatePropFunc` — свойство класса, которое будет функцией. Не хранится в прототипе класса, закрепляется за экземпляром и сохраняет за собой контекст (`this` — инстанс класса).
* `updateMethod` — метод класса. Хранится в прототипе.

Какие бонусы?


# На последний урок
## Верстальщик + js-программист
Как идет разработка интерфейса на Реакте, если на проекте есть и верстальщик и js-программист?

## Вложенные компоненты
Можно ли хранить компоненты во вложенной структуре папок, если они везде так и используются? Или лучше все-таки держать все в плоской структуре?

Например, компонет с фильтарми:

```bash
components/

    # лучше так?
    Filters/
        index.js
        style.less
        
        DateRange/
            index.js
            style.less
            
        Select/
            index.js
            style.less
            
    # или так?
    Filters/
        index.js
        style.less
        
    DateRange/
        index.js
        style.less
        
    Select/
        index.js
        style.less
```

и где-то импортим:

```jsx harmony
import Filters from 'Filters'
```