# Languages

This page is W.I.P.

## Creating a new language

New languages have to be created through the web interface. You login on the web interface and click on the left side bar on "Languages". Click on "Create Language", this will open a modal where you can enter the name of the new language. Click on "Create" to create the new language. After you clicked on "Create" it will copy all message of the English language and put it in the language you created. After that you can start translating!

## Changing the language messages

There are two ways to change the messages of your languages.

### 1. The web interface

You can change the languages through the web interface. You login on the web interface and click on the left side bar on "Languages". There you'll find your languages that are available in-game. Click on the orange pencil at the end of the language to enter the language messages editor. Here you'll be able to edit the languages for the selected language. When you leave the textbox your changes will be saved automatically.

### 2. Export/Import

Since NetworkManager version 2.10.9 it is possible to export and import the messages of a language. Exporting them will export the messages of the selected language from the database to a json file. You can use this to modify the language messages or share them with someone else. The command for exporting a language is `/language export <language> [--plugin [pluginName]]`. After modifying the json file you can import it back into the database. The command for importing a language file is `/language import <language> [--overwrite]`

## Formatting

NetworkManager uses the adventure minimessage library to turn the messages into components which is being used natively by minecraft itself.

You can find more information about the minimessage format [here](https://docs.adventure.kyori.net/minimessage/format.html). There is also a helpful online tool which will help you style your messages and can be found [here](https://webui.adventure.kyori.net/).



## Useful tools

The official [MiniMessage Web Viewer](https://webui.adventure.kyori.net/) can be used for previewing and testing your formats and styles.

If you need something to convert legacy colorcodes to minimessage then you can use either this [tool ](https://tehbrian.xyz/legacy-to-minimessage/)by Brian or this [tool](https://nm-colors.remividon.fr/) by Rémi.



