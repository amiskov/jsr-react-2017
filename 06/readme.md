# Занятие №6, 22 мая
* Immutable

## Immutable

## Работаем с сервером
```
// проксирвоание запросов
devServer: {
    proxy: [{
        path: '/api/', // localhost:8080/api => http://localhost:3001
        target: 'http://localhost:3001'
    }]
}
```


[`redux-thunk`](https://github.com/gaearon/redux-thunk)
