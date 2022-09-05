---
description: This functionality will be introduced in a future version of NetworkManager.
---

# TagsMenu

## The Menu Configuration

```
{
  "Options": {
    "Title": "&cTagsGUI",
    "ShowNoAccessItems": false,
    "SelectedGlow": true
  },
  "Items": {
    "PreviousPage": {
      "Material": "ARROW",
      "DisplayName": "Previous",
      "Amount": 1,
      "Lore": [],
      "Slot": 45,
      "Extras": {}
    },
    "ClearTag": {
      "Material": "BARRIER",
      "DisplayName": "Clear Tag",
      "Amount": 1,
      "Lore": [],
      "Slot": 52,
      "Extras": {}
    },
    "Tag": {
      "Material": "NAME_TAG",
      "DisplayName": "&o%name%",
      "Amount": 1,
      "Lore": [
        "%tag%",
        "%description%"
      ],
      "Extras": {}
    },
    "CloseMenu": {
      "Material": "BOOK",
      "DisplayName": "Close",
      "Amount": 1,
      "Lore": [],
      "Slot": 49,
      "Extras": {}
    },
    "TagNoAccess": {
      "Material": "RED_STAINED_GLASS_PANE",
      "DisplayName": "&o%name%",
      "Amount": 1,
      "Lore": [
        "%tag%",
        "%description%"
      ],
      "Extras": {}
    },
    "NextPage": {
      "Material": "ARROW",
      "DisplayName": "Next",
      "Amount": 1,
      "Lore": [],
      "Slot": 53,
      "Extras": {}
    }
  }
}
```

{% hint style="info" %}
A little tip if you're looking for Skulls. Lots of skulls can be found here: [https://minecraft-heads.com/](https://minecraft-heads.com/) and they also provide it's skull data
{% endhint %}

```
"NextPage": {
  "Material": "PLAYER_HEAD",
  "DisplayName": "Next",
  "Amount": 1,
  "Lore": [],
  "Slot": 53,
  "SkullData": "eyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvYzIzY2YyMTBlZGVhMzk2ZjJmNWRmYmNlZDY5ODQ4NDM0ZjkzNDA0ZWVmZWFiZjU0YjIzYzA3M2IwOTBhZGYifX19",
  "Extras": {}
}
```
