# TextChat
An in-game TextChat plugin for SCP:SL.

## Minimum requirements
[EXILED](https://github.com/galaxy119/EXILED) **2.1.8.1+**

[LiteDB](https://github.com/mbdavid/LiteDB) **5.0.9+**

## How to install
Put **TextChat.dll** inside `%appdata%\Plugins` if you're on **Windows** or `~/.config/Plugins` on **Linux**.

Put **LiteDB.dll** inside `%appdata%\Plugins\dependencies` folder if you're using **Windows** or `~/.config/Plugins/dependencies` if you're on **Linux**.

## How to use it
Press **ò** or **\`** on your keyboard to open the in-game console, with that, you'll be able to execute commands to chat with other players.

## How to submit a new language

**First method**
- Fork my repository.
- Copy `Localizations\Language.resx` into the `Localization` folder and rename it to `Localizations\Language.XX.resx` where XX are the [language code letters](https://lonewolfonline.net/list-net-culture-country-codes/).
- For example: I want to add the french language into the game, then I'll have to rename the file to `Language.fr.resx`.
- Translate the file with any text editor or C# IDE and push it into your forked repository.
- Open a pull request on my repository with the language you added, if everything is correct, I'll accept it and add it into the plugin.

**Second method**
- Download [Language.resx](https://github.com/iopietro/TextChat/blob/master/TextChat/Localizations/Language.resx), translate it in your language and send it to me on Discord: iopietro#1717, if everything is correct, I'll add it into te plugin.

### Player Commands
| Command | Description | Arguments | Example |
| --- | --- | --- | --- |
| .chat public | Sends a chat message to everyone in the server. | **[Message]** | **.chat Hi all!** |
| .chat team | Sends a chat message to your team. | **[Message]** | **.chat_team I love being SCP!** |
| .chat private | Sends a private chat message to a player. | **[Nickname/UserID/PlayerID] [Message]** | **.chat_private iopietro Hello!** | 

### Administrator Commands
| Command | Description | Arguments | Permission | Example |
| --- | --- | --- | --- | --- |
| chat mute add | Mutes a player from the chat. | **[Nickname/UserID/PlayerID] [Duration (Minutes)] [Reason]** | tc.mute | **chat_mute iopietro 600 Spamming** |
| chat mute remove | Unmutes a player from the chat by removing its last mute or removes all of its mutes. | **[Nickname/UserID/PlayerID]** | tc.unmute | **chat_unmute iopietro** |
| chat mute show | Shows all mutes stored in the database or mutes of a specific player. | **None/[Nickname/UserID/PlayerID]** | tc.showmutes | **chat_show_mutes/chat_show_mutes iopietro** |

### List of available languages
| Name | Config Value |
| --- | --- |
| English | en |
| Italian | it |
| Portuguese | pt |
| Korean | ko |
| German | de |

### List of available colors
| Name |
| --- |
| yellow |
| green |
| cyan |
| red |
| magenta |
| black |
| white |
| blue |
| grey |
