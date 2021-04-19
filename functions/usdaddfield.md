# $addField

Эта функция отвечает за добавление нового поля во встраивание, содержащего ограничение в 1000 символов каждое и позволяющего использовать 10 полей на встраивание.

#### Функции

Эта функция имеет 2 функции

1. Name \(Обязательно\)
2. Content \(Обязательно\)
3. Inline \(Необязательно\)

Пример использования: `$addField[title;description;inline (optional)]`

#### Опции

* Name - Заголовок поля
* Content - Описание поля
* Inline \(yes/no\) - Устанавливает поле во встроенное поле

#### Использование

Без встраивания

```javascript
bot.command({
    name: "embed",
    code: `$addField[This is an example field;And this is the content!]`
});
```

Со встраиванием

```javascript
bot.command({
    name: "embed",
    code: `
    $addField[Inline #;3;yes]
    $addField[Inline #;2;yes]
    $addField[Inline #;1;yes]
    `
});
```





