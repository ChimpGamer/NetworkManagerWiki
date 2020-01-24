---
description: This functionality will be introduced in a future version of NetworkManager.
---

# LanguageMenu

## The Menu Configuration

```
{
  "Options": {
    "Title": "&cLanguageGUI",
    "SelectedGlow": true
  },
  "Items": {
    "English": {
      "Material": "PLAYER_HEAD",
      "DisplayName": "&eEnglish",
      "Lore": [
        "&7&oClick &ehere &7&oto change your language to English"
      ],
      "SkullData": "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYTE3MDFmMjE4MzVhODk4YjIwNzU5ZmIzMGE1ODNhMzhiOTk0YWJmNjBkMzkxMmFiNGNlOWYyMzExZTc0ZjcyIn19fQ==",
      "Slot": 30
    }
  }
}
```

{% hint style="info" %}
The SelectedGlow option does not work with skulls or player heads and some other items.
{% endhint %}

{% hint style="info" %}
A little tip if you're looking for Skulls. Lots of skulls can be found here: [https://minecraft-heads.com/](https://minecraft-heads.com/) and they also provide it's skull data
{% endhint %}

I'll also provide a modified example of the configuration so you'll have a better example on how to add other languages to the configuration

```text
{
  "Options": {
    "Title": "&cLanguageGUI",
    "SelectedGlow": true
  },
  "Items": {
    "English": {
      "Material": "PLAYER_HEAD",
      "DisplayName": "&eEnglish",
      "Lore": [
        "&7&oClick &ehere &7&oto change your language to English"
      ],
      "SkullData": "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYTE3MDFmMjE4MzVhODk4YjIwNzU5ZmIzMGE1ODNhMzhiOTk0YWJmNjBkMzkxMmFiNGNlOWYyMzExZTc0ZjcyIn19fQ==",
      "Slot": 30
    },
    "Nederlands": {
      "Material": "PLAYER_HEAD",
      "DisplayName": "&eNederlands",
      "Lore": [
        "&7&oKlik &ehier &7&oom je taal naar Nederlands te veranderen"
      ],
      "SkullData": "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYzIzY2YyMTBlZGVhMzk2ZjJmNWRmYmNlZDY5ODQ4NDM0ZjkzNDA0ZWVmZWFiZjU0YjIzYzA3M2IwOTBhZGYifX19",
      "Slot": 31
    }
  }
}
```

This configuration file also contains the Nederlands \(Dutch\) language and it has a different skull.

