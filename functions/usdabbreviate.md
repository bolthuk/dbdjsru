# $abbreviate

Эта функция сокращает большие числа

#### Использование

Только одна функция

1. Number \(обязательно\)

Пример использования: `$abbreviate[number]`

#### Опции

* Number - Число которое будет сокращено

#### Аббревиатуры

* k - тысячи
* m - миллионы
* b - миллиарды
* t - триллионы

```javascript
bot.command({
name: "abbr",
code: `
$abbreviate[5000]
`
//Вернёт: 5k
})

//или персональное число

bot.command({
name: "abbr",
code: `
$abbreviate[$message]
`
})
```

