---
description: Установка ссылки внутри слова
---

# Гиперссылка



{% hint style="danger" %}
Должно находится в $description
{% endhint %}

```javascript
bot.command({
name: "hyperlink", 
code: `
$description[[Package](https://www.npmjs.com/package/dbd.js)]` 
})
```

