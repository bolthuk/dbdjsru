---
description: >-
  Этот обратный вызов срабатывает каждый раз, когда ваш бот получает ограничение
  скорости
---

# bot.onRateLimit

```javascript
bot.rateLimitCommand({
channel: "ID"
code: `your code`
})

bot.onRateLimit()
```

#### Пример

```javascript
bot.rateLimitCommand({ 
channel: "772414449839636490" 
code: `I've been rate limited!
Timeout: $rateLimt[timeout]
Limit: $rateLimit[limit]
Method: $rateLimit[method]
Path: $rateLimit[path]
Route: $rateLimit[route]
`
})

bot.onRateLimit()
```

#### Options for $rateLimit

*  `timeout` - Время до перезапуска этого ограничения скорости сеанса 
* `limit` - Количество раз, когда вы можете запросить эту конечную точку перед сбоем 
* `method` - Метод, используемый для этой конечной
* `path` - Путь к конечной точке api, которая вызвала маршрут ограничения скорости 
* `route` - Маршрут, который вызвал это событие

