---
description: Позволяет использовать несколько версий команды
---

# Псевдонимы



**Обычные псевдонимы**

```javascript
bot.command({
name: "имя",
aliases: ['имя2','имя3'], // Если вы хотите только один псевдоним ['name2'] или 'name2'
code: `код`
})
```

**Псевдонимы для обработчика команд**

{% hint style="warning" %}
Переделайте ваш server.js под это
{% endhint %}

```javascript
const dbd = require("dbd.js")

const bot = new dbd.Bot({
token: "TOKEN", 
prefix: "!" 
})

bot.onMessage()

const fs = require('fs')

const folders = fs.readdirSync("./commands/")

for (const files of folders) {
const folder = fs.readdirSync(`./commands/${files}/`).filter(file => file.endsWith(".js"))

for (const commands of folder) {
const command = require(`./commands/${files}/${commands}`) 
bot.command({
name: command.name,
aliases: command.aliases, // Это правильно читает псевдонимы
code: command.code
})
}
}
```

**Ваш файл command.js**

```javascript
module.exports = ({
name: "name",
aliases: ['name2','name3','etc'],
code: `code`
})
```

