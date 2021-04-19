# Шарды

{% hint style="danger" %}
Шарды работают только в ботах которые находятся на 2,000+ Серверах
{% endhint %}

### Как поставить шарды

```javascript
const bot = new dbd.bot({
    sharding: true,
    shardAmount: 2,
    token: "token",
    prefix: "prefix"
})
```

### Смотрим Шард на сервере.

```javascript
bot.command({
    name: "shardID",
    code: `Guilds Shard: $shardID`
})
```

{% hint style="danger" %}
Шардинг может привести к высокому пингу/отклика и, в зависимости от вашего хоста, может использовать много памяти и дискового пространства
{% endhint %}

