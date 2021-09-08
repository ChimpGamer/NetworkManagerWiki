# Announcements

### What does it do?

This system will announce chat, actionbar or title messages every x seconds depending on your configuration. Read more about it below on how to configure it.

### Settings

The announcements have only three global settings which are interval settings.  
Interval is in seconds!  
setting\_actionbar\_announcements\_interval  
setting\_chat\_announcements\_interval  
setting\_title\_announcements\_interval

### How to create announcement

![](../../.gitbook/assets/image%20%289%29.png)

| Field |  |
| :--- | :--- |
| Type | Select the type of announcment you want/need. Click [here ](https://networkmanager.gitbook.io/wiki/networkmanager-plugin/modules/announcements#announcement-types)to find more information about each announcement type. |
| Message | Pretty straight forward. You enter the message in this field. You can use \[center\] on a new line to center that line. More information about centering text can be found [here](https://networkmanager.gitbook.io/wiki/networkmanager-plugin/modules/announcements#how-to-center-messages). When you select the title type of announcements you need to use a specific format here. Click [here ](https://networkmanager.gitbook.io/wiki/networkmanager-plugin/modules/announcements#announcement-types)to find more information about title messages. |
| Sound | One of [these ](https://networkmanager.gitbook.io/wiki/networkmanager-plugin/modules/announcements#announcement-sounds)sounds. These will be played when a player receives the announcement. NOTE: Only works when NetworkManager is also installed on your spigot server\(s\). |
| Server | Name of the server that the announcement will be executed on \(depending on the announcement type\). You can only put one server here. If you want the announcement to use multiple servers you'll have to use a servergroup. |
| Expires | You can select a date of time that the announcement will automatically be disabled. |
| Active | Whether you want it to be active after creation or not. |

### Announcement Types

The announcement types explained!

* CHATALLSERVERS - Send the chat announcement to all servers on your network.
* CHATSERVERSONLY - Send the chat announcement to specified servers only.
* CHATSERVERSEXCEPT - Send the chat announcement to all servers except the specified servers.
* ACTIONBARALLSERVERS - Send the actionbar announcement to all servers on your network.
* ACTIONBARSERVERSONLY - Send the actionbar announcement to specified servers only.
* ACTIONBARSERVERSEXCEPT - Send the actionbar announcement to all servers except the specified servers.
* TITLEALLSERVERS - Send the title announcement to all servers on your network.
* TITLESERVERSONLY - Send the title announcement to specified servers only.
* TITLESERVERSEXCEPT - Send the title announcement to all servers except the specified servers.

### Announcement permissions

If you enabled the permission for a specific announcement then you'll have to assign the permission node to a specific group or player in order to allow them to see the announcement. The permission node is: networkmanager.announcement.&lt;id&gt;.

### How to create a title?

In NetworkManager we use json for creating titles. It's pretty simple.   
Example:

```javascript
{"title": "Title here", "subtitle": "Subtitle here"}
```

Since NetworkManager v2.6.3 you can also define fadeOut, fadeIn and stay.   
Example:

```javascript
{"title": "Title here", "subtitle": "Subtitle here", "fadeOut": 20, "fadeIn": 20, "stay": 60}
```

### How to center messages?

Since NetworkManager v2.6.3 you can center messages. It's pretty simple. You add \[center\] to the line you want to center. Example:

```javascript
&c&m-----------------------
[center]&6Hey this message is centered!
This message isn't centered :(
[center][{"text":"This message is centered!","color":"gold","hoverEvent":{"action":"show_text","value":{"text":"","extra":[{"text":"With JSON! :D","color":"green"}]}}}]
&c&m-----------------------
```

### Announcement sounds

You can use sounds with Announcements. All sounds listed below will work with 1.8 - 1.14.

NOTE: To use this feature you'll need NetworkManager v2.6.3 or higher on your spigot servers.

```text
AMBIENCE_CAVE
AMBIENCE_RAIN
AMBIENCE_THUNDER
ANVIL_BREAK
ANVIL_LAND
ANVIL_USE
ARROW_HIT
BURP
CHEST_CLOSE
CHEST_OPEN
CLICK
DOOR_CLOSE
DOOR_OPEN
DRINK
EAT
EXPLODE
FALL_BIG
FALL_SMALL
FIRE
FIRE_IGNITE
FIZZ
FUSE
GLASS
HURT_FLESH
ITEM_BREAK
ITEM_PICKUP
LAVA
LAVA_POP
LEVEL_UP
MINECART_BASE
MINECART_INSIDE
NOTE_BASS
NOTE_PIANO
NOTE_BASS_DRUM
NOTE_STICKS
NOTE_BASS_GUITAR
NOTE_SNARE_DRUM
NOTE_PLING
ORB_PICKUP
PISTON_EXTEND
PISTON_RETRACT
PORTAL
PORTAL_TRAVEL
PORTAL_TRIGGER
SHOOT_ARROW
SPLASH
SPLASH2
STEP_GRASS
STEP_GRAVEL
STEP_LADDER
STEP_SAND
STEP_SNOW
STEP_STONE,
STEP_WOOD,
STEP_WOOL,
SWIM,
WATER,
WOOD_CLICK,
BAT_DEATH,
BAT_HURT,
BAT_IDLE,
BAT_LOOP,
BAT_TAKEOFF,
BLAZE_BREATH,
BLAZE_DEATH,
BLAZE_HIT,
CAT_HISS,
CAT_HIT,
CAT_MEOW,
CAT_PURR,
CAT_PURREOW,
CHICKEN_IDLE,
CHICKEN_HURT,
CHICKEN_EGG_POP,
CHICKEN_WALK,
COW_IDLE,
COW_HURT,
COW_WALK,
CREEPER_HISS,
CREEPER_DEATH,
ENDERDRAGON_DEATH,
ENDERDRAGON_GROWL,
ENDERDRAGON_HIT,
ENDERDRAGON_WINGS,
ENDERMAN_DEATH,
ENDERMAN_HIT,
ENDERMAN_IDLE,
ENDERMAN_TELEPORT,
ENDERMAN_SCREAM,
ENDERMAN_STARE,
GHAST_SCREAM,
GHAST_SCREAM2,
GHAST_CHARGE,
GHAST_DEATH,
GHAST_FIREBALL,
GHAST_MOAN,
IRONGOLEM_ATTACK,
IRONGOLEM_DEATH,
IRONGOLEM_HIT,
IRONGOLEM_WALK,
MAGMACUBE_WALK,
MAGMACUBE_WALK2,
MAGMACUBE_JUMP,
PIG_IDLE
PIG_DEATH
PIG_WALK
SHEEP_IDLE
SHEEP_SHEAR
SHEEP_WALK
SILVERFISH_HIT
SILVERFISH_KILL
SILVERFISH_IDLE
SILVERFISH_WALK
SKELETON_IDLE
SKELETON_DEATH
SKELETON_HURT
SKELETON_WALK
SLIME_ATTACK
SLIME_WALK
SLIME_WALK2
SPIDER_IDLE
SPIDER_DEATH
SPIDER_WALK
WITHER_DEATH
WITHER_HURT
WITHER_IDLE
WITHER_SHOOT
WITHER_SPAWN
WOLF_BARK
WOLF_DEATH
WOLF_GROWL
WOLF_HOWL
WOLF_HURT
WOLF_PANT
WOLF_SHAKE
WOLF_WALK
WOLF_WHINE
ZOMBIE_METAL
ZOMBIE_WOOD
ZOMBIE_WOODBREAK
ZOMBIE_IDLE
ZOMBIE_DEATH
ZOMBIE_HURT
ZOMBIE_INFECT
ZOMBIE_UNFECT
ZOMBIE_REMEDY
ZOMBIE_WALK
ZOMBIE_PIG_IDLE
ZOMBIE_PIG_ANGRY
ZOMBIE_PIG_DEATH
ZOMBIE_PIG_HURT
DIG_WOOL
DIG_GRASS
DIG_GRAVEL
DIG_SAND
DIG_SNOW
DIG_STONE
DIG_WOOD
FIREWORK_BLAST
FIREWORK_BLAST2
FIREWORK_LARGE_BLAST
FIREWORK_LARGE_BLAST2
FIREWORK_LAUNCH
FIREWORK_TWINKLE
FIREWORK_TWINKLE2
SUCCESSFUL_HIT
HORSE_ANGRY
HORSE_ARMOR
HORSE_BREATHE
HORSE_DEATH
HORSE_GALLOP
HORSE_HIT
HORSE_IDLE
HORSE_JUMP
HORSE_LAND
HORSE_SADDLE
HORSE_SOFT
HORSE_WOOD
DONKEY_ANGRY
DONKEY_DEATH
DONKEY_HIT
DONKEY_IDLE
HORSE_SKELETON_DEATH
HORSE_SKELETON_HIT
HORSE_SKELETON_IDLE
HORSE_ZOMBIE_DEATH
HORSE_ZOMBIE_HIT
HORSE_ZOMBIE_IDLE
VILLAGER_DEATH
VILLAGER_TRADE
VILLAGER_HIT
VILLAGER_IDLE
VILLAGER_NO
VILLAGER_YES
```

