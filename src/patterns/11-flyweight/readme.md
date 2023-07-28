# Flyweight

> Позволяет экономить память, разделяя общее состояние объектов 
> между собой, вместо хранения одинаковых данных в каждом объекте.

- Type: Structural
- Complexity: ⭐

Представьте что Вы работаете над магазином, Вы уже разработали класс
`ProductStore` для хранения товаров в системе.

Но проанализировал данные о товарах, Вы обнаружили что каждый из них
содержит общую информацию, хранимую в св-ве `info`:

```js
{
  model: "m1",
  info: {
    name: "Apple",
    country: "USA",
    color: "silver"
  }
},
{
  model: "m2",
  info: {
    name: "Apple",
    country: "USA",
    color: "silver"
  }
},
...
```

Для оптимизации памяти, требуемой для хранения товаров, Вы приняли решение
воспользоваться паттерном "Flyweight".

Пожалуйста, реализуйте методы `addProduct` и `getOrCreateFlyweight` класса
`ProductStore`, а также связь с классом `Flyweight` в котором будет
храниться общее состояние продуктов, а именно данные из св-ва `info`.