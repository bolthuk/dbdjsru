---
description: Эта страница поможет в начале создания бота
---

# Начало

## Установка DBD.JS

```
npm i aoi.js
```

{% hint style="info" %}
 Некоторые хостинги \(glitch, repl.it, danbot\) сами устанавливают
{% endhint %}

## Ваш основной файл server.js

```bash
const Aoijs = require("aoi.js")
 
const bot = new Aoijs.Bot({
  sharding: false, // true - есть шарды. false - нет шардов 
  shardAmount: 2, // Кол-во шардов 
  mobile: false, // true - Включить активность с телефона. false - Активность с ПК
  token: "TOKEN", // Токен бота
  prefix: ["PREFIX"] // Измените PREFIX на нужный
})
 
bot.onMessage() // Нужно что бы команды выполнялись
 
bot.command({
name: "ping", 
code: `Понг! \`$ping\`` 
})
```

## package.json

Файл, в который ваш проект может "попасть" aoi.js

```bash
{
    "name": "-asdf",
    "version": "1.0.0",
    "description": "",
    "main": "server.js",
    "scripts": {
      "start": "node server.js"
    },
    "engines": {
      "node": "12.x"
    },
    "author": "",
    "license": "ISC",
    "dependencies": {
      "aoi.js": "^1.0.5"
    }
  }
```

{% hint style="warning" %}
Для обновления AOI.JS, измените на последнюю версию из \#изменения
{% endhint %}

## Обычный шаблон команды

```bash
bot.command({
      name: "имя",
      code: `ваш код/сообщение`
})
```

## **Обычный код статуса**

```bash
bot.status({
      text: "aoi.js",
      type: "PLAYING",
      time: 12
})
```

## Имеются несколько видов статуса

* PLAYING - Играет
* WATCHING - Смотрит
* LISTENING - Слушает
* COMPETING - Сражается

 Больше информации о статусах только в англ версии: [https://aoi.leref.ga/guide/bot-status](https://dbd.leref.ga/guide/bot-status)

Весь гайд по началу. Для большей помощи вы можете зайти на сайт [https://aoi.leref.ga/](https://dbd.leref.ga/) или задать вопрос в \#помощь

{% hint style="danger" %}
Если вы используете glitch или repl.it или danbot   
Не используйте npm i aoi.js   
Ваш package.json, Всё установит сам!
{% endhint %}

