---
description: >-
  Этот обратный вызов срабатывает всякий раз, когда кто-то присоединяется,
  покидает или обновляет свои параметры vc
---

# bot.onVoiceStateUpdate

```javascript
bot.voiceStateUpdateCommand({
channel: "id",
code: `code`
})

bot.onVoiceStateUpdate()
```

#### Пример

```javascript
bot.voiceStateUpdateCommand({ 
channel: "772414449839636490" 
code: `
ГК обновлён
$username - 
$oldState[selfMute] - $newState[selfMute]
` 
})

bot.onVoiceStateUpdate() 
```

