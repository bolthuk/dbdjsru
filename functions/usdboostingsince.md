# $boostingSince

#### Поля

Эта функция имеет 2 необязательных поля  


1. UserID \(необязательно\)
2. ms \(необязательно\)

Пример: `$boostingSince[User ID(Optional);ms (yes/no) (Optional)]`

#### Опции

* UserID - Пользователь, от которого мы получаем данные
* ms - Возвращает время в миллисекундах

#### Usage

```javascript
bot.command({
    name: "boosting",
    code: `
    $if[$boostingSince!=]
$username has been boosting since $boostingSince
    $else
You're not boosting!
    $endif
    `
});
```

