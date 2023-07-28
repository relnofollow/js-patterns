# Observer

> Позволяет создать механизм подписки, который позволит некоторым 
> сущностям следить и реагировать на события, происходящие в других
> сущностях, как следствие обеспечивая слабую связанность.

- Type: Behavioral
- Complexity: ⭐⭐

Пожалуйста, реализуйте методы `subscribe` класса `NewsChannel`
к-й позволит всем желающим пользователям подписаться на новостные
сообщения, и метод `notify` к-й будет заниматься рассылкой этих сообщений для всех
подписчиков.

Также реализуйте метод `receiveMessage` класса `User` для получения сообщений и их
записи в поле `messageHistory`.