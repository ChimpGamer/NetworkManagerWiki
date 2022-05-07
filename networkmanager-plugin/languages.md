# Languages

This page is W.I.P.

## Changing the language messages

There are two ways to change the messages of your languages.

### 1. The web interface

You can change the languages through the web interface. You login on the web interface and click on the left side bar on "Languages". There you'll find your languages that are available in-game. Click on the orange pencil at the end of the language to enter the language messages editor. Here you'll be able to edit the languages for the selected language. When you leave the textbox your changes will be saved automatically.

### 2. Export/Import

Since NetworkManager version 2.10.9 it is possible to export and import the messages of a language. Exporting them will export the messages of the selected language from the database to a json file. You can use this to modify the language messages or share them with someone else. The command for exporting a language is `/language export <language> [--plugin [pluginName]]` After modifying the json file you can import it back into the database. The command for importing a language file is `/language import <language> [--overwrite]`

``
