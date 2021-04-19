---
description: Как поставить статус боту
---

# Статус Бота

### Как я могу установить статус боту? 

Это очень легко

{% hint style="info" %}
Вам нужно добавить это в основной файл
{% endhint %}

```javascript
bot.status({
  text: "Текст",
  type: "PLAYING",
  time: 12
})
```

{% hint style="info" %}
Для нескольких статусов используйте следующее:
{% endhint %}

```javascript
bot.status({
  text: "текст1",
  type: "PLAYING",
  time: 12
})

bot.status({
  text: "текст2",
  type: "WATCHING",
  time: 12
})
```

## Различные Типы:

* PLAYING - Играет
* WATCHING - Смотрит
* LISTENING - Слушает
* STREAMING - Стримит
* COMPETING - Сражается

## Статус бота

Если вы хотите изменить статус бота используйте следующее:

```javascript
bot.status({
  text: "текст",
  type: "PLAYING",
  status: "idle",
  time: 12
})
```

## Различные типы:

* idle - Занят
* dnd - Не беспокоить
* online - Онлайн
* invisible - Оффлайн

## Статус стрима:

{% hint style="info" %}
Если вы хотите ввести URL-адрес, введите следующее:
{% endhint %}

```javascript
bot.status({
text: "Текст", 
type: "STREAMING", 
url: "Ссылка"
})
```

## Мобильный статус

```javascript
const bot = new dbd.Bot({
token: "TOKEN", 
prefix: "!",
mobile: true
})
```

