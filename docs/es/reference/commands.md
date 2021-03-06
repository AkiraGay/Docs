# Commands

To get a list of available commands, do !help on your server.

## Arguments & Flags

Most commands accept arguments and/or flags.  
According to the **Type** of the argument or flag you can provide different values.

### Boolean

This arguments expects `true` or `false`. You can also use `yes` and `no`.

### Number

This arguments expects a number

### Enum

This arguments expects a value from a specific set of valid values.

> Depending on the command the valid values can vary. Use `!help <command>` (eg. `!help addRank`) to get more information about the command and the valid values for the enum.

### Invite Code

This arguments expects a Discord Invite Code.

> You can put only the part after `https://discord.gg/` to prevent Discord from creating a preview.

### User

This arguments expects a Discord User. You can use any of the following methods to provide a user:

- Mention the user: `@Valandur`
- Use their ID: `102785693046026240`
- Use their name: `Valandur`
- Use their name and discriminator: `Valandur#3581`
- Use quotes if their name has a space: `"Valandur with a space"`

### Rol

This arguments expects a Discord Role. You can use any of the following methods to provide a role:

- Mention the role: `@Admin`
- Use the ID: `102785693046026240`
- Use the name: `Admin`
- Use quotes if the name has a space: `"Admin with a space"`

### Canal

This arguments expects a Discord Channel. You can use any of the following methods to provide a channel:

- Mention the channel: `#general`
- Use the ID: `409846838129197057`
- Use the name: `general`
- Use quotes if the name has a space: `"general with a space"`

### Comando

This argument expects a command of this bot. You can use any of the following methods to provide a command:

- Use the command name: `invites`
- Use an alias of the command: `p`

### Text

This arguments expects any text. You can use quotes (`"Text with quotes"`) for text that has spaces.

> If the text is the last argument you don't have to use quotes.

### Date

This argument expects a date. You can use various formats, but we recommend: `YYYY-MM-DD`

### Duration

This argument expects a duration. The following duration types are supported:

- Seconds: `s` (`5s` = 5 seconds)
- Minutes: `min` (`3min` = 3 minutes)
- Hours: `h` (`4h` = 4 hours)
- Days: `d` (`2d` = 2 days)
- Weeks: `w` (`1w` = 1 week)
- Months: `mo` (`6mo` = 6 months)
- Years: `y` (`10y` = 10 years)

## Overview

### Invites

| Command                           | Description                                            | Usage                                                            |
| --------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------- |
| [addInvites](#addInvites)         | A??ade/remueve invitaciones a/de un miembro.            | !addInvites \<user\> \<amount\> [reason]                         |
| [clearInvites](#clearInvites)     | Limpia invitaciones del servidor/un usuario.           | !clearInvites [-d value\|--date=value][-cb\|--clearbonus] [user] |
| [createInvite](#createInvite)     | Crea c??digos de invitaci??n ??nicos.                     | !createInvite \<name\> [channel]                                 |
| [info](#info)                     | Muestra informaci??n de un miembro en especifico.       | !info \<user\> [details][page]                                   |
| [inviteCodes](#inviteCodes)       | Obt??n una lista de todos tus c??digos de invitaci??n.    | !inviteCodes                                                     |
| [inviteDetails](#inviteDetails)   | Muestra detalles sobre donde son tus invitaciones.     | !inviteDetails [user]                                            |
| [invites](#invites)               | Muestra invitaciones personales.                       | !invites [user]                                                  |
| [leaderboard](#leaderboard)       | Mostrar a los miembros con m??s invitaciones.           | !leaderboard [page]                                              |
| [removeInvites](#removeInvites)   | Removes a specified amount of invites from a user.     | !removeInvites \<user\> \<amount\> [reason]                      |
| [restoreInvites](#restoreInvites) | Restaura todas las invitaciones previamente limpiadas. | !restoreInvites [user]                                           |
| [subtractFakes](#subtractFakes)   | Remueve invitaciones falsas de todos los usuarios.     | !subtractFakes                                                   |
| [subtractLeaves](#subtractLeaves) | Remueve salidas de todos los usuarios.                 | !subtractLeaves                                                  |

### Ranks

| Command                   | Description                                   | Usage                                |
| ------------------------- | --------------------------------------------- | ------------------------------------ |
| [addRank](#addRank)       | A??ade un nuevo rango.                         | !addRank \<role\> \<invites\> [info] |
| [fixRanks](#fixRanks)     | Deletes any ranks where the role was deleted. | !fixRanks                            |
| [ranks](#ranks)           | Mostrar todos los rangos.                     | !ranks [page]                        |
| [removeRank](#removeRank) | Remueve un rango.                             | !removeRank \<rank\>                 |

### Config

| Command                                 | Description                                                                  | Usage                                       |
| --------------------------------------- | ---------------------------------------------------------------------------- | ------------------------------------------- |
| [botConfig](#botConfig)                 | Mostrar y cambiar la configuraci??n del Bot.                                  | !botConfig [key][value]                     |
| [config](#config)                       | Muestra y cambia la configuraci??n del servidor.                              | !config [key][value]                        |
| [interactiveConfig](#interactiveConfig) | Configuraci??n interactiva                                                    | !interactiveConfig                          |
| [inviteCodeConfig](#inviteCodeConfig)   | Muestra y cambia la configuraci??n de los c??digos de invitaci??n del servidor. | !inviteCodeConfig [key][invitecode] [value] |
| [memberConfig](#memberConfig)           | Muestra y cambia la configuraci??n de los miembros del servidor.              | !memberConfig [key][user] [value]           |
| [permissions](#permissions)             | Configura permisos para usar comandos.                                       | !permissions [cmd][role]                    |

### Info

| Command             | Description                                                                                        | Usage           |
| ------------------- | -------------------------------------------------------------------------------------------------- | --------------- |
| [botInfo](#botInfo) | Obt??n informaci??n general sobre el bot.                                                            | !botInfo        |
| [credits](#credits) | Mostrar desarrolladores y colaboradores del bot.                                                   | !credits        |
| [getBot](#getBot)   | Consigue un link de invitaci??n para el bot.                                                        | !getBot         |
| [help](#help)       | Mostrar ayuda.                                                                                     | !help [command] |
| [members](#members) | Muestra el conteo de miembros del servidor actual.                                                 | !members        |
| [ping](#ping)       | Mencionar al Bot                                                                                   | !ping           |
| [prefix](#prefix)   | Muestra el prefijo actual del bot.                                                                 | !prefix         |
| [setup](#setup)     | Ayuda con la configuraci??n del bot y la comprobaci??n de problemas (por ejemplo, falta de permisos) | !setup          |
| [support](#support) | Consigue un link de invitaci??n a nuestro servidor de soporte.                                      | !support        |

### Premium

| Command                   | Description                                                                          | Usage             |
| ------------------------- | ------------------------------------------------------------------------------------ | ----------------- |
| [export](#export)         | Exporta informaci??n de Invite Succubi a una hoja csv.                                 | !export \<type\>  |
| [premium](#premium)       | Informaci??n sobre la versi??n premium de Invite Succubi.                               | !premium [action] |
| [tryPremium](#tryPremium) | Prueba la versi??n premium de Invite Succubi gratis por un limitado periodo de tiempo. | !tryPremium       |

### Moderation

| Command                               | Description                                                                                                                                   | Usage                                                            |
| ------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| [ban](#ban)                           | Banea a un usuario del servidor.                                                                                                              | !ban [-d value\|--deleteMessageDays=value] \<user\> [reason]     |
| [caseDelete](#caseDelete)             | Eliminar un caso en espec??fico.                                                                                                               | !caseDelete \<caseNumber\> [reason]                              |
| [caseView](#caseView)                 | Ver informaci??n sobre un caso espec??fico.                                                                                                     | !caseView \<caseNumber\>                                         |
| [check](#check)                       | Revisa el historial de violaciones y castigos del usuario.                                                                                    | !check \<user\>                                                  |
| [clean](#clean)                       | Elimina mensajes de cierto tipo en un canal.                                                                                                  | !clean \<type\> [numberOfMessages]                               |
| [cleanShort](#cleanShort)             | Borrar mensajes cortos                                                                                                                        | !cleanShort \<maxTextLength\> [numberOfMessages]                 |
| [cleanText](#cleanText)               | Eliminar mensajes que contengan ciertas palabras claves.                                                                                      | !cleanText \<text\> [numberOfMessages]                           |
| [kick](#kick)                         | Expulsa a un miembro del servidor.                                                                                                            | !kick \<member\> [reason]                                        |
| [lockdown](#lockdown)                 | Lockdown a specific channel (Prevents anyone without special roles from sending messages)                                                     | !lockdown [-t value\|--timeout=value][channel]                   |
| [mute](#mute)                         | Mute a user                                                                                                                                   | !mute [-d value\|--duration=value] \<user\> [reason]             |
| [punishmentConfig](#punishmentConfig) | Configura castigos cuando una cierta cantidad de strikes es alcanzada.                                                                        | !punishmentConfig [punishment][strikes] [args]                   |
| [purge](#purge)                       | Elimina mensajes en un canal.                                                                                                                 | !purge \<quantity\> [user]                                       |
| [purgeUntil](#purgeUntil)             | Elimina mensajes en un canal hasta un mensaje especifico.                                                                                     | !purgeUntil \<messageID\>                                        |
| [softBan](#softBan)                   | Banea y despu??s autom??ticamente desbanea a un miembro del servidor.                                                                           | !softBan [-d value\|--deleteMessageDays=value] \<user\> [reason] |
| [strike](#strike)                     | Add strikes to a user                                                                                                                         | !strike \<member\> \<type\> \<amount\>                           |
| [strikeConfig](#strikeConfig)         | Configura strikes recibidos por varias violaciones.                                                                                           | !strikeConfig [violation][strikes]                               |
| [unban](#unban)                       | Unban a user                                                                                                                                  | !unban \<user\> [reason]                                         |
| [unhoist](#unhoist)                   | Add a character in front of all members with a special character in front of their name, so they will be shown at the end of the member list. | !unhoist                                                         |
| [unmute](#unmute)                     | Unmute a user                                                                                                                                 | !unmute \<user\>                                                 |
| [warn](#warn)                         | Advertir a un miembro                                                                                                                         | !warn \<member\> [reason]                                        |

### Music

| Command                   | Description                                                                                                 | Usage                                                   |
| ------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------- |
| [disconnect](#disconnect) | Disconnect the bot from the current voice channel.                                                          | !disconnect                                             |
| [lyrics](#lyrics)         | Show lyrics of the currently playing song.                                                                  | !lyrics [-l\|--live]                                    |
| [mashup](#mashup)         | Create a mashup of 2 songs.                                                                                 | !mashup \<videos\>                                      |
| [nowPlaying](#nowPlaying) | Shows information about the currently playing song                                                          | !nowPlaying [-p\|--pin]                                 |
| [pause](#pause)           | Pause the current song.                                                                                     | !pause                                                  |
| [play](#play)             | Reproducir la canci??n si la cola esta vac??a, en caso contrario la canci??n ser?? a??adida al final de la cola. | !play [-p value\|--platform=value][-n\|--next] \<link\> |
| [queue](#queue)           | Display the songs in the queue.                                                                             | !queue                                                  |
| [repeat](#repeat)         | Set the song to be played on repeat.                                                                        | !repeat                                                 |
| [resume](#resume)         | Resume the current song.                                                                                    | !resume                                                 |
| [rewind](#rewind)         | Rewind the song and start from the beginning.                                                               | !rewind                                                 |
| [search](#search)         | Search for the search term and let you chose one of the results.                                            | !search [-p value\|--platform=value] \<search\>         |
| [seek](#seek)             | Skip to a specific part of the song.                                                                        | !seek [duration]                                        |
| [skip](#skip)             | Skip the current song and play the next song in the queue.                                                  | !skip [amount]                                          |
| [volume](#volume)         | Set the volume if an argument is passed, or show the current volume.                                        | !volume [volume]                                        |

### Other

| Command         | Description                                                  | Usage                      |
| --------------- | ------------------------------------------------------------ | -------------------------- |
| [graph](#graph) | Muestra gr??ficos sobre varias estad??sticas en este servidor. | !graph \<type\> [from][to] |

<a name='addInvites'></a>

---

## !addInvites

A??ade/remueve invitaciones a/de un miembro.

### Usage

```text
!addInvites <user> <amount> [reason]
```

### Aliases

- `!add-invites`

### Arguments

| Argument | Type              | Required | Description                                                                                                    | Details |
| -------- | ----------------- | -------- | -------------------------------------------------------------------------------------------------------------- | ------- |
| user     | [User](#User)     | Yes      | El usuario que recibir??/perder?? las invitaciones bonus.                                                        |         |
| amount   | [Number](#Number) | Yes      | La cantidad de invitaciones el usuario recibir??/perder??. Usa un n??mero negativo (-) para remover invitaciones. |         |
| reason   | [Text](#Text)     | No       | La raz??n para a??adir/remover invitaciones.                                                                     |         |

### Examples

```text
!addInvites @User 5
```

```text
!addInvites "Name with space" -30 Removed for cheating
```

<a name='addRank'></a>

---

## !addRank

A??ade un nuevo rango.

### Usage

```text
!addRank <role> <invites> [info]
```

### Aliases

- `!add-rank`
- `!set-rank`
- `!setrank`

### Arguments

| Argument | Type              | Required | Description                                                            | Details |
| -------- | ----------------- | -------- | ---------------------------------------------------------------------- | ------- |
| role     | [Rol](#Rol)       | Yes      | El rol que el usuario recibir?? cuando llegue a este rango.             |         |
| invites  | [Number](#Number) | Yes      | La cantidad de invitaciones necesarias para alcanzar este rango.       |         |
| info     | [Text](#Text)     | No       | La descripci??n que los usuarios ver??n para saber m??s sobre este rango. |         |

### Examples

```text
!addRank @Role 5
```

```text
!addRank "Role with space" 10 Wow, already 10 people!
```

<a name='ban'></a>

---

## !ban

Banea a un usuario del servidor.

### Usage

```text
!ban [-d value|--deleteMessageDays=value] <user> [reason]
```

### Arguments

| Argument | Type          | Required | Description                     | Details |
| -------- | ------------- | -------- | ------------------------------- | ------- |
| user     | [User](#User) | Yes      | Usuario a banear.               |         |
| reason   | [Text](#Text) | No       | Por qu?? fue baneado el usuario. |         |

### Flags

| Flag                              | Short     | Type              | Description                                                                           |
| --------------------------------- | --------- | ----------------- | ------------------------------------------------------------------------------------- |
| &#x2011;&#x2011;deleteMessageDays | &#x2011;d | [Number](#Number) | Si se especifica, eliminar?? los mensajes de los miembros prohibidos hace muchos d??as. |

### Examples

<a name='botConfig'></a>

---

## !botConfig

Mostrar y cambiar la configuraci??n del Bot.

### Usage

```text
!botConfig [key] [value]
```

### Aliases

- `!bot-config`
- `!botsetting`
- `!bot-setting`

### Arguments

| Argument | Type            | Required | Description                                                        | Details                                                                                                                                     |
| -------- | --------------- | -------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| key      | [Enum](#Enum)   | No       | El ajuste de la configuraci??n del Bot que quieres mostrar/cambiar. | Use one of the following values: `activityEnabled`, `activityMessage`, `activityStatus`, `activityType`, `activityUrl`, `embedDefaultColor` |
| value    | [Value](#Value) | No       | El nuevo valor del ajuste.                                         |                                                                                                                                             |

### Examples

```text
!botConfig
```

<a name='botInfo'></a>

---

## !botInfo

Obt??n informaci??n general sobre el bot.

### Usage

```text
!botInfo
```

### Aliases

- `!bot-info`

### Examples

```text
!botInfo
```

<a name='caseDelete'></a>

---

## !caseDelete

Eliminar un caso en espec??fico.

### Usage

```text
!caseDelete <caseNumber> [reason]
```

### Aliases

- `!case-delete`
- `!deletecase`
- `!delete-case`

### Arguments

| Argument   | Type              | Required | Description                     | Details |
| ---------- | ----------------- | -------- | ------------------------------- | ------- |
| caseNumber | [Number](#Number) | Yes      | N??mero del caso.                |         |
| reason     | [Text](#Text)     | No       | La raz??n para eliminar el caso. |         |

### Examples

```text
!caseDelete 5434 User apologized
```

<a name='caseView'></a>

---

## !caseView

Ver informaci??n sobre un caso espec??fico.

### Usage

```text
!caseView <caseNumber>
```

### Aliases

- `!case-view`
- `!viewcase`
- `!view-case`

### Arguments

| Argument   | Type              | Required | Description     | Details |
| ---------- | ----------------- | -------- | --------------- | ------- |
| caseNumber | [Number](#Number) | Yes      | N??mero del caso |         |

### Examples

```text
!caseView 5434
```

<a name='check'></a>

---

## !check

Revisa el historial de violaciones y castigos del usuario.

### Usage

```text
!check <user>
```

### Aliases

- `!history`

### Arguments

| Argument | Type          | Required | Description        | Details |
| -------- | ------------- | -------- | ------------------ | ------- |
| user     | [User](#User) | Yes      | Usuario a revisar. |         |

### Examples

```text
!check @User
```

```text
!check "User with space"
```

<a name='clean'></a>

---

## !clean

Elimina mensajes de cierto tipo en un canal.

### Usage

```text
!clean <type> [numberOfMessages]
```

### Aliases

- `!clear`

### Arguments

| Argument         | Type              | Required | Description                             | Details                                                                                                            |
| ---------------- | ----------------- | -------- | --------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| type             | [Enum](#Enum)     | Yes      | El tipo de mensaje que ser?? eliminado.  | Use one of the following values: `bots`, `embeds`, `emojis`, `images`, `links`, `mentions`, `reacted`, `reactions` |
| numberOfMessages | [Number](#Number) | No       | El n??mero de mensajes que ser?? buscado. |                                                                                                                    |

### Examples

<a name='cleanShort'></a>

---

## !cleanShort

Borrar mensajes cortos

### Usage

```text
!cleanShort <maxTextLength> [numberOfMessages]
```

### Aliases

- `!clean-short`
- `!clearshort`
- `!clear-short`

### Arguments

| Argument         | Type              | Required | Description                                        | Details |
| ---------------- | ----------------- | -------- | -------------------------------------------------- | ------- |
| maxTextLength    | [Number](#Number) | Yes      | Los mensajes m??s cortos que este ser??n eliminados. |         |
| numberOfMessages | [Number](#Number) | No       | El n??mero de mensajes que ser??n buscados.          |         |

### Examples

<a name='cleanText'></a>

---

## !cleanText

Eliminar mensajes que contengan ciertas palabras claves.

### Usage

```text
!cleanText <text> [numberOfMessages]
```

### Aliases

- `!clean-text`
- `!cleartext`
- `!clear-text`

### Arguments

| Argument         | Type              | Required | Description                                                     | Details |
| ---------------- | ----------------- | -------- | --------------------------------------------------------------- | ------- |
| text             | [Text](#Text)     | Yes      | Todos los mensajes que contengan esta palabra ser??n eliminados. |         |
| numberOfMessages | [Number](#Number) | No       | Cantidad de mensajes que ser??n buscados.                        |         |

### Examples

<a name='clearInvites'></a>

---

## !clearInvites

Limpia invitaciones del servidor/un usuario.

### Usage

```text
!clearInvites [-d value|--date=value] [-cb|--clearBonus] [user]
```

### Aliases

- `!clear-invites`

### Arguments

| Argument | Type          | Required | Description                                                                            | Details |
| -------- | ------------- | -------- | -------------------------------------------------------------------------------------- | ------- |
| user     | [User](#User) | No       | El usuario a limpiar todas las invitaciones. Si se omite, limpia a todos los usuarios. |         |

### Flags

| Flag                       | Short      | Type                | Description                                                                                                                                   |
| -------------------------- | ---------- | ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| &#x2011;&#x2011;date       | &#x2011;d  | [Date](#Date)       | La fecha de inicio en la cual se comenzar??n a contar las invitaciones. Por defecto; hoy.                                                      |
| &#x2011;&#x2011;clearBonus | &#x2011;cb | [Boolean](#Boolean) | Agregue esta bandera para borrar las invitaciones de bonificaci??n tambi??n. De lo contrario, las invitaciones de bonificaci??n quedan intactas. |

### Examples

```text
!clearInvites
```

```text
!clearInvites @User
```

```text
!clearInvites -cb "User with space"
```

<a name='config'></a>

---

## !config

Muestra y cambia la configuraci??n del servidor.

### Usage

```text
!config [key] [value]
```

### Aliases

- `!c`

### Arguments

| Argument | Type            | Required | Description                                             | Details                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| -------- | --------------- | -------- | ------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| key      | [Enum](#Enum)   | No       | El ajuste de configuraci??n que quieres mostrar/cambiar. | Use one of the following values: `announcementVoice`, `announceNextSong`, `autoModAllCapsEnabled`, `autoModAllCapsMinCharacters`, `autoModAllCapsPercentageCaps`, `autoModDeleteBotMessage`, `autoModDeleteBotMessageTimeoutInSeconds`, `autoModDisabledForOldMembers`, `autoModDisabledForOldMembersThreshold`, `autoModDuplicateTextEnabled`, `autoModDuplicateTextTimeframeInSeconds`, `autoModEmojisEnabled`, `autoModEmojisMaxNumberOfEmojis`, `autoModEnabled`, `autoModHoistEnabled`, `autoModIgnoredChannels`, `autoModIgnoredRoles`, `autoModInvitesEnabled`, `autoModLinksBlacklist`, `autoModLinksEnabled`, `autoModLinksFollowRedirects`, `autoModLinksWhitelist`, `autoModLogEnabled`, `autoModMentionRolesEnabled`, `autoModMentionRolesMaxNumberOfMentions`, `autoModMentionUsersEnabled`, `autoModMentionUsersMaxNumberOfMentions`, `autoModModeratedChannels`, `autoModModeratedRoles`, `autoModQuickMessagesEnabled`, `autoModQuickMessagesNumberOfMessages`, `autoModQuickMessagesTimeframeInSeconds`, `autoModWordsBlacklist`, `autoModWordsEnabled`, `autoSubtractFakes`, `autoSubtractLeaves`, `autoSubtractLeaveThreshold`, `captchaVerificationFailedMessage`, `captchaVerificationLogEnabled`, `captchaVerificationOnJoin`, `captchaVerificationSuccessMessage`, `captchaVerificationTimeout`, `captchaVerificationWelcomeMessage`, `channels`, `defaultMusicPlatform`, `disabledMusicPlatforms`, `fadeMusicEndDelay`, `fadeMusicOnTalk`, `getUpdates`, `hideLeftMembersFromLeaderboard`, `ignoredChannels`, `joinMessage`, `joinMessageChannel`, `joinRoles`, `lang`, `leaderboardStyle`, `leaveMessage`, `leaveMessageChannel`, `logChannel`, `modLogChannel`, `modPunishmentBanDeleteMessage`, `modPunishmentKickDeleteMessage`, `modPunishmentMuteDeleteMessage`, `modPunishmentSoftbanDeleteMessage`, `modPunishmentWarnDeleteMessage`, `musicVolume`, `mutedRole`, `prefix`, `rankAnnouncementChannel`, `rankAnnouncementMessage`, `rankAssignmentStyle` |
| value    | [Value](#Value) | No       | El nuevo valor del ajuste.                              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

### Examples

```text
!config
```

<a name='createInvite'></a>

---

## !createInvite

Crea c??digos de invitaci??n ??nicos.

### Usage

```text
!createInvite <name> [channel]
```

### Aliases

- `!create-invite`

### Arguments

| Argument | Type            | Required | Description                                                                               | Details |
| -------- | --------------- | -------- | ----------------------------------------------------------------------------------------- | ------- |
| name     | [Text](#Text)   | Yes      | El nombre del c??digo de invitaci??n.                                                       |         |
| channel  | [Canal](#Canal) | No       | El canal para el cual el c??digo de invitaci??n es creado. Usa el canal actual por defecto. |         |

### Examples

```text
!createInvite reddit
```

```text
!createInvite website #welcome
```

<a name='credits'></a>

---

## !credits

Mostrar desarrolladores y colaboradores del bot.

### Usage

```text
!credits
```

### Examples

```text
!credits
```

<a name='disconnect'></a>

---

## !disconnect

Disconnect the bot from the current voice channel.

### Usage

```text
!disconnect
```

### Examples

```text
!disconnect
```

<a name='export'></a>

---

## !export

Exporta informaci??n de Invite Succubi a una hoja csv.

### Usage

```text
!export <type>
```

### Arguments

| Argument | Type          | Required | Description                      | Details                                        |
| -------- | ------------- | -------- | -------------------------------- | ---------------------------------------------- |
| type     | [Enum](#Enum) | Yes      | El tipo de exportar que quieres. | Use one of the following values: `leaderboard` |

### Examples

```text
!export leaderboard
```

<a name='fixRanks'></a>

---

## !fixRanks

Deletes any ranks where the role was deleted.

### Usage

```text
!fixRanks
```

### Aliases

- `!fix-ranks`

### Examples

```text
!fixRanks
```

<a name='getBot'></a>

---

## !getBot

Consigue un link de invitaci??n para el bot.

### Usage

```text
!getBot
```

### Aliases

- `!get-bot`
- `!invite-bot`
- `!invitebot`

### Examples

```text
!getBot
```

<a name='graph'></a>

---

## !graph

Muestra gr??ficos sobre varias estad??sticas en este servidor.

### Usage

```text
!graph <type> [from] [to]
```

### Aliases

- `!g`
- `!chart`

### Arguments

| Argument | Type          | Required | Description                   | Details                                                              |
| -------- | ------------- | -------- | ----------------------------- | -------------------------------------------------------------------- |
| type     | [Enum](#Enum) | Yes      | El tipo de gr??fico a mostrar. | Use one of the following values: `joins`, `joinsAndLeaves`, `leaves` |
| from     | [Date](#Date) | No       | cmd.graph.self.args.from      |                                                                      |
| to       | [Date](#Date) | No       | cmd.graph.self.args.to        |                                                                      |

### Examples

```text
!graph joins
```

```text
!graph leaves
```

```text
!graph usage
```

<a name='help'></a>

---

## !help

Mostrar ayuda.

### Usage

```text
!help [command]
```

### Arguments

| Argument | Type                | Required | Description                                     | Details                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| -------- | ------------------- | -------- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| command  | [Comando](#Comando) | No       | El comando a obtener m??s informaci??n detallada. | Use one of the following values: `addInvites`, `addRank`, `ban`, `botConfig`, `botInfo`, `caseDelete`, `caseView`, `check`, `clean`, `cleanShort`, `cleanText`, `clearInvites`, `config`, `createInvite`, `credits`, `disconnect`, `export`, `fixRanks`, `getBot`, `graph`, `help`, `info`, `interactiveConfig`, `inviteCodeConfig`, `inviteCodes`, `inviteDetails`, `invites`, `kick`, `leaderboard`, `lockdown`, `lyrics`, `mashup`, `memberConfig`, `members`, `mute`, `nowPlaying`, `pause`, `permissions`, `ping`, `play`, `prefix`, `premium`, `punishmentConfig`, `purge`, `purgeUntil`, `queue`, `ranks`, `removeInvites`, `removeRank`, `repeat`, `restoreInvites`, `resume`, `rewind`, `search`, `seek`, `setup`, `skip`, `softBan`, `strike`, `strikeConfig`, `subtractFakes`, `subtractLeaves`, `support`, `tryPremium`, `unban`, `unhoist`, `unmute`, `volume`, `warn` |

### Examples

```text
!help
```

```text
!help addRank
```

<a name='info'></a>

---

## !info

Muestra informaci??n de un miembro en especifico.

### Usage

```text
!info <user> [details] [page]
```

### Aliases

- `!showinfo`

### Arguments

| Argument | Type              | Required | Description                                                                                | Details                                             |
| -------- | ----------------- | -------- | ------------------------------------------------------------------------------------------ | --------------------------------------------------- |
| user     | [User](#User)     | Yes      | El usuario del que quieres ver m??s informaci??n.                                            |                                                     |
| details  | [Enum](#Enum)     | No       | Solicitar solo datos espec??ficos sobre un miembro.                                         | Use one of the following values: `bonus`, `members` |
| page     | [Number](#Number) | No       | Que pagina de los detalles ser?? mostrada. Tambi??n puedes usar las reacciones para navegar. |                                                     |

### Examples

```text
!info @User
```

```text
!info "User with space"
```

```text
!info @User members
```

```text
!info @User bonus
```

```text
!info @User members 4
```

<a name='interactiveConfig'></a>

---

## !interactiveConfig

Configuraci??n interactiva

### Usage

```text
!interactiveConfig
```

### Aliases

- `!ic`

### Examples

```text
!interactiveConfig
```

<a name='inviteCodeConfig'></a>

---

## !inviteCodeConfig

Muestra y cambia la configuraci??n de los c??digos de invitaci??n del servidor.

### Usage

```text
!inviteCodeConfig [key] [inviteCode] [value]
```

### Aliases

- `!invite-code-config`
- `!icc`

### Arguments

| Argument   | Type                       | Required | Description                                                         | Details                                          |
| ---------- | -------------------------- | -------- | ------------------------------------------------------------------- | ------------------------------------------------ |
| key        | [Enum](#Enum)              | No       | El ajuste de configuraci??n que quieres mostrar/cambiar.             | Use one of the following values: `name`, `roles` |
| inviteCode | [Invite Code](#InviteCode) | No       | El c??digo de invitaci??n para el que desea cambiar la configuraci??n. |                                                  |
| value      | [Value](#Value)            | No       | El nuevo valor del ajuste.                                          |                                                  |

### Examples

```text
!inviteCodeConfig
```

<a name='inviteCodes'></a>

---

## !inviteCodes

Obt??n una lista de todos tus c??digos de invitaci??n.

### Usage

```text
!inviteCodes
```

### Aliases

- `!invitecode`
- `!invite-code`
- `!invite-codes`
- `!getinvitecode`
- `!get-invite-code`
- `!get-invite-codes`
- `!showinvitecode`
- `!show-invite-code`

### Examples

```text
!inviteCodes
```

<a name='inviteDetails'></a>

---

## !inviteDetails

Muestra detalles sobre donde son tus invitaciones.

### Usage

```text
!inviteDetails [user]
```

### Aliases

- `!invite-details`

### Arguments

| Argument | Type          | Required | Description                                                 | Details |
| -------- | ------------- | -------- | ----------------------------------------------------------- | ------- |
| user     | [User](#User) | No       | El usuario del que quieres mostrar invitaciones detalladas. |         |

### Examples

```text
!inviteDetails
```

```text
!inviteDetails @User
```

```text
!inviteDetails "User with space"
```

<a name='invites'></a>

---

## !invites

Muestra invitaciones personales.

### Usage

```text
!invites [user]
```

### Aliases

- `!invite`
- `!rank`

### Arguments

| Argument | Type          | Required | Description                                      | Details |
| -------- | ------------- | -------- | ------------------------------------------------ | ------- |
| user     | [User](#User) | No       | El usuario del que quieres mostrar invitaciones. |         |

### Examples

```text
!invites
```

```text
!invites @User
```

```text
!invites "User with space"
```

<a name='kick'></a>

---

## !kick

Expulsa a un miembro del servidor.

### Usage

```text
!kick <member> [reason]
```

### Arguments

| Argument | Type              | Required | Description                       | Details |
| -------- | ----------------- | -------- | --------------------------------- | ------- |
| member   | [Member](#Member) | Yes      | Usuario a expulsar.               |         |
| reason   | [Text](#Text)     | No       | Por qu?? el usuario fue expulsado. |         |

### Examples

<a name='leaderboard'></a>

---

## !leaderboard

Mostrar a los miembros con m??s invitaciones.

### Usage

```text
!leaderboard [page]
```

### Aliases

- `!top`

### Arguments

| Argument | Type              | Required | Description                                   | Details |
| -------- | ----------------- | -------- | --------------------------------------------- | ------- |
| page     | [Number](#Number) | No       | Que pagina de la tabla de puntuaci??n obtener. |         |

### Examples

```text
!leaderboard
```

```text
!leaderboard 1mo
```

```text
!leaderboard 30d 6
```

<a name='lockdown'></a>

---

## !lockdown

Lockdown a specific channel (Prevents anyone without special roles from sending messages)

### Usage

```text
!lockdown [-t value|--timeout=value] [channel]
```

### Arguments

| Argument | Type            | Required | Description                             | Details |
| -------- | --------------- | -------- | --------------------------------------- | ------- |
| channel  | [Canal](#Canal) | No       | The channel that you want to lock down. |         |

### Flags

| Flag                    | Short     | Type                  | Description                                                                                                  |
| ----------------------- | --------- | --------------------- | ------------------------------------------------------------------------------------------------------------ |
| &#x2011;&#x2011;timeout | &#x2011;t | [Duration](#Duration) | The timeout after which the lockdown automatically ends. Run the command again to end the lockdown manually. |

### Examples

```text
!lockdown
```

<a name='lyrics'></a>

---

## !lyrics

Show lyrics of the currently playing song.

### Usage

```text
!lyrics [-l|--live]
```

### Flags

| Flag                 | Short     | Type                | Description                                                                                         |
| -------------------- | --------- | ------------------- | --------------------------------------------------------------------------------------------------- |
| &#x2011;&#x2011;live | &#x2011;l | [Boolean](#Boolean) | Si esta establecido, la letra de la canci??n se va a sincronizar con la reproducci??n actual de esta. |

### Examples

```text
!lyrics
```

<a name='mashup'></a>

---

## !mashup

Create a mashup of 2 songs.

### Usage

```text
!mashup <videos>
```

### Arguments

| Argument | Type          | Required | Description                                | Details |
| -------- | ------------- | -------- | ------------------------------------------ | ------- |
| videos   | [Text](#Text) | Yes      | The videos that should be mashed together. |         |

### Examples

<a name='memberConfig'></a>

---

## !memberConfig

Muestra y cambia la configuraci??n de los miembros del servidor.

### Usage

```text
!memberConfig [key] [user] [value]
```

### Aliases

- `!member-config`
- `!memconf`
- `!mc`

### Arguments

| Argument | Type            | Required | Description                                                               | Details                                                |
| -------- | --------------- | -------- | ------------------------------------------------------------------------- | ------------------------------------------------------ |
| key      | [Enum](#Enum)   | No       | La configuraci??n de configuraci??n de miembro que desea mostrar / cambiar. | Use one of the following values: `hideFromLeaderboard` |
| user     | [User](#User)   | No       | El miembro para el que se muestra/cambia la configuraci??n.                |                                                        |
| value    | [Value](#Value) | No       | El nuevo valor del ajuste.                                                |                                                        |

### Examples

```text
!memberConfig
```

<a name='members'></a>

---

## !members

Muestra el conteo de miembros del servidor actual.

### Usage

```text
!members
```

### Aliases

- `!member`
- `!memberscount`

### Examples

```text
!members
```

<a name='mute'></a>

---

## !mute

Mute a user

### Usage

```text
!mute [-d value|--duration=value] <user> [reason]
```

### Arguments

| Argument | Type              | Required | Description                                        | Details |
| -------- | ----------------- | -------- | -------------------------------------------------- | ------- |
| user     | [Member](#Member) | Yes      | El usuario que debe estar silenciado.              |         |
| reason   | [Text](#Text)     | No       | La raz??n por la cual este usuario est?? silenciado. |         |

### Flags

| Flag                     | Short     | Type                  | Description                       |
| ------------------------ | --------- | --------------------- | --------------------------------- |
| &#x2011;&#x2011;duration | &#x2011;d | [Duration](#Duration) | The duration to mute the user for |

### Examples

<a name='nowPlaying'></a>

---

## !nowPlaying

Shows information about the currently playing song

### Usage

```text
!nowPlaying [-p|--pin]
```

### Aliases

- `!np`
- `!now-playing`

### Flags

| Flag                | Short     | Type                | Description                                                                        |
| ------------------- | --------- | ------------------- | ---------------------------------------------------------------------------------- |
| &#x2011;&#x2011;pin | &#x2011;p | [Boolean](#Boolean) | Pin the now playing message and update it automatically whenever a new song plays. |

### Examples

```text
!nowPlaying
```

<a name='pause'></a>

---

## !pause

Pause the current song.

### Usage

```text
!pause
```

### Aliases

- `!stop`

### Examples

```text
!pause
```

<a name='permissions'></a>

---

## !permissions

Configura permisos para usar comandos.

### Usage

```text
!permissions [cmd] [role]
```

### Aliases

- `!perms`

### Arguments

| Argument | Type                | Required | Description                                                 | Details                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| -------- | ------------------- | -------- | ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| cmd      | [Comando](#Comando) | No       | El comando al cual configurar permisos.                     | Use one of the following values: `addInvites`, `addRank`, `ban`, `botConfig`, `botInfo`, `caseDelete`, `caseView`, `check`, `clean`, `cleanShort`, `cleanText`, `clearInvites`, `config`, `createInvite`, `credits`, `disconnect`, `export`, `fixRanks`, `getBot`, `graph`, `help`, `info`, `interactiveConfig`, `inviteCodeConfig`, `inviteCodes`, `inviteDetails`, `invites`, `kick`, `leaderboard`, `lockdown`, `lyrics`, `mashup`, `memberConfig`, `members`, `mute`, `nowPlaying`, `pause`, `permissions`, `ping`, `play`, `prefix`, `premium`, `punishmentConfig`, `purge`, `purgeUntil`, `queue`, `ranks`, `removeInvites`, `removeRank`, `repeat`, `restoreInvites`, `resume`, `rewind`, `search`, `seek`, `setup`, `skip`, `softBan`, `strike`, `strikeConfig`, `subtractFakes`, `subtractLeaves`, `support`, `tryPremium`, `unban`, `unhoist`, `unmute`, `volume`, `warn` |
| role     | [Rol](#Rol)         | No       | El rol al cual se le deber??a dar ornegar acceso al comando. |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

### Examples

```text
!permissions
```

<a name='ping'></a>

---

## !ping

Mencionar al Bot

### Usage

```text
!ping
```

### Examples

```text
!ping
```

<a name='play'></a>

---

## !play

Reproducir la canci??n si la cola esta vac??a, en caso contrario la canci??n ser?? a??adida al final de la cola.

### Usage

```text
!play [-p value|--platform=value] [-n|--next] <link>
```

### Aliases

- `!p`

### Arguments

| Argument | Type          | Required | Description                                   | Details |
| -------- | ------------- | -------- | --------------------------------------------- | ------- |
| link     | [Text](#Text) | Yes      | The link to a specific song or a search term. |         |

### Flags

| Flag                     | Short     | Type                | Description                                                                       |
| ------------------------ | --------- | ------------------- | --------------------------------------------------------------------------------- |
| &#x2011;&#x2011;platform | &#x2011;p | [Enum](#Enum)       | Select the platform where you want the song to be played.                         |
| &#x2011;&#x2011;next     | &#x2011;n | [Boolean](#Boolean) | If set, it will play this song next instead of adding it to the end of the queue. |

### Examples

<a name='prefix'></a>

---

## !prefix

Muestra el prefijo actual del bot.

### Usage

```text
!prefix
```

### Examples

```text
!prefix
```

<a name='premium'></a>

---

## !premium

Informaci??n sobre la versi??n premium de Invite Succubi.

### Usage

```text
!premium [action]
```

### Aliases

- `!paypal`
- `!donate`

### Arguments

| Argument | Type          | Required | Description                                                                                                                                                                    | Details                                                            |
| -------- | ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------ |
| action   | [Enum](#Enum) | No       | La acci??n a realizar. Nada para la informaci??n de Premium. `check` para ver el estado de tu suscripci??n Premium. `activate` para usar tu suscripci??n Premium en este servidor. | Use one of the following values: `Activate`, `Check`, `Deactivate` |

### Examples

```text
!premium
```

```text
!premium check
```

```text
!premium activate
```

```text
!premium deactivate
```

<a name='punishmentConfig'></a>

---

## !punishmentConfig

Configura castigos cuando una cierta cantidad de strikes es alcanzada.

### Usage

```text
!punishmentConfig [punishment] [strikes] [args]
```

### Aliases

- `!punishment-config`

### Arguments

| Argument   | Type              | Required | Description                                    | Details                                                                   |
| ---------- | ----------------- | -------- | ---------------------------------------------- | ------------------------------------------------------------------------- |
| punishment | [Enum](#Enum)     | No       | Tipo de castigo a usar.                        | Use one of the following values: `ban`, `kick`, `mute`, `softban`, `warn` |
| strikes    | [Number](#Number) | No       | Numero de strikes para ser usado este castigo. |                                                                           |
| args       | [Text](#Text)     | No       | Argumentos pasados al castigo.                 |                                                                           |

### Examples

```text
!punishmentConfig
```

<a name='purge'></a>

---

## !purge

Elimina mensajes en un canal.

### Usage

```text
!purge <quantity> [user]
```

### Aliases

- `!prune`

### Arguments

| Argument | Type              | Required | Description                               | Details |
| -------- | ----------------- | -------- | ----------------------------------------- | ------- |
| quantity | [Number](#Number) | Yes      | Cuantos mensajes deber??an ser eliminados. |         |
| user     | [User](#User)     | No       | User whose messages are deleted.          |         |

### Examples

<a name='purgeUntil'></a>

---

## !purgeUntil

Elimina mensajes en un canal hasta un mensaje especifico.

### Usage

```text
!purgeUntil <messageID>
```

### Aliases

- `!purge-until`
- `!prune-until`
- `!pruneu`
- `!purgeu`

### Arguments

| Argument  | Type          | Required | Description                       | Details |
| --------- | ------------- | -------- | --------------------------------- | ------- |
| messageID | [Text](#Text) | Yes      | ID del ultimo mensaje a eliminar. |         |

### Examples

<a name='queue'></a>

---

## !queue

Display the songs in the queue.

### Usage

```text
!queue
```

### Examples

```text
!queue
```

<a name='ranks'></a>

---

## !ranks

Mostrar todos los rangos.

### Usage

```text
!ranks [page]
```

### Aliases

- `!show-ranks`
- `!showranks`

### Arguments

| Argument | Type              | Required | Description                         | Details |
| -------- | ----------------- | -------- | ----------------------------------- | ------- |
| page     | [Number](#Number) | No       | The page of the ranks list to show. |         |

### Examples

```text
!ranks
```

<a name='removeInvites'></a>

---

## !removeInvites

Removes a specified amount of invites from a user.

### Usage

```text
!removeInvites <user> <amount> [reason]
```

### Aliases

- `!remove-invites`

### Arguments

| Argument | Type              | Required | Description                          | Details |
| -------- | ----------------- | -------- | ------------------------------------ | ------- |
| user     | [User](#User)     | Yes      | The user to remove the invites from. |         |
| amount   | [Number](#Number) | Yes      | The amount of invites to remove.     |         |
| reason   | [Text](#Text)     | No       | The reason for removing the invites. |         |

### Examples

```text
!removeInvites @User 5
```

```text
!removeInvites "User with space" 23 Removed for cheating
```

```text
!removeInvites @User -6 Added for apologizing
```

<a name='removeRank'></a>

---

## !removeRank

Remueve un rango.

### Usage

```text
!removeRank <rank>
```

### Aliases

- `!remove-rank`

### Arguments

| Argument | Type        | Required | Description                          | Details |
| -------- | ----------- | -------- | ------------------------------------ | ------- |
| rank     | [Rol](#Rol) | Yes      | Para el que desea eliminar el rango. |         |

### Examples

```text
!removeRank @Role
```

```text
!removeRank "Role with space"
```

<a name='repeat'></a>

---

## !repeat

Set the song to be played on repeat.

### Usage

```text
!repeat
```

### Aliases

- `!loop`

### Examples

```text
!repeat
```

<a name='restoreInvites'></a>

---

## !restoreInvites

Restaura todas las invitaciones previamente limpiadas.

### Usage

```text
!restoreInvites [user]
```

### Aliases

- `!restore-invites`
- `!unclear-invites`
- `!unclearinvites`

### Arguments

| Argument | Type          | Required | Description                                                                                             | Details |
| -------- | ------------- | -------- | ------------------------------------------------------------------------------------------------------- | ------- |
| user     | [User](#User) | No       | El usuario a restaurar todas las invitaciones. Si se omite, restaura invitaciones a todos los usuarios. |         |

### Examples

```text
!restoreInvites
```

```text
!restoreInvites @User
```

```text
!restoreInvites "User with space"
```

<a name='resume'></a>

---

## !resume

Resume the current song.

### Usage

```text
!resume
```

### Aliases

- `!start`

### Examples

```text
!resume
```

<a name='rewind'></a>

---

## !rewind

Rewind the song and start from the beginning.

### Usage

```text
!rewind
```

### Aliases

- `!replay`

### Examples

```text
!rewind
```

<a name='search'></a>

---

## !search

Search for the search term and let you chose one of the results.

### Usage

```text
!search [-p value|--platform=value] <search>
```

### Arguments

| Argument | Type          | Required | Description     | Details |
| -------- | ------------- | -------- | --------------- | ------- |
| search   | [Text](#Text) | Yes      | The search term |         |

### Flags

| Flag                     | Short     | Type          | Description                                               |
| ------------------------ | --------- | ------------- | --------------------------------------------------------- |
| &#x2011;&#x2011;platform | &#x2011;p | [Enum](#Enum) | Select the platform where you want the song to be played. |

### Examples

<a name='seek'></a>

---

## !seek

Skip to a specific part of the song.

### Usage

```text
!seek [duration]
```

### Arguments

| Argument | Type              | Required | Description                                                                | Details |
| -------- | ----------------- | -------- | -------------------------------------------------------------------------- | ------- |
| duration | [Number](#Number) | No       | The position the song will be skipped to (from the beginning, in seconds). |         |

### Examples

```text
!seek
```

<a name='setup'></a>

---

## !setup

Ayuda con la configuraci??n del bot y la comprobaci??n de problemas (por ejemplo, falta de permisos)

### Usage

```text
!setup
```

### Aliases

- `!guide`
- `!test`
- `!testbot`
- `!test-bot`

### Examples

```text
!setup
```

<a name='skip'></a>

---

## !skip

Skip the current song and play the next song in the queue.

### Usage

```text
!skip [amount]
```

### Aliases

- `!next`

### Arguments

| Argument | Type              | Required | Description                     | Details |
| -------- | ----------------- | -------- | ------------------------------- | ------- |
| amount   | [Number](#Number) | No       | How many songs will be skipped. |         |

### Examples

```text
!skip
```

<a name='softBan'></a>

---

## !softBan

Banea y despu??s autom??ticamente desbanea a un miembro del servidor.

### Usage

```text
!softBan [-d value|--deleteMessageDays=value] <user> [reason]
```

### Aliases

- `!soft-ban`

### Arguments

| Argument | Type              | Required | Description                     | Details |
| -------- | ----------------- | -------- | ------------------------------- | ------- |
| user     | [Member](#Member) | Yes      | Usuario a banear.               |         |
| reason   | [Text](#Text)     | No       | Por qu?? fue baneado el usuario. |         |

### Flags

| Flag                              | Short     | Type              | Description                                        |
| --------------------------------- | --------- | ----------------- | -------------------------------------------------- |
| &#x2011;&#x2011;deleteMessageDays | &#x2011;d | [Number](#Number) | Delete messages from the user this many days back. |

### Examples

<a name='strike'></a>

---

## !strike

Add strikes to a user

### Usage

```text
!strike <member> <type> <amount>
```

### Arguments

| Argument | Type              | Required | Description                       | Details                                                                                                                                                      |
| -------- | ----------------- | -------- | --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| member   | [Member](#Member) | Yes      | The member receiving the strikes  |                                                                                                                                                              |
| type     | [Enum](#Enum)     | Yes      | The type of the violation         | Use one of the following values: `allCaps`, `duplicateText`, `emojis`, `hoist`, `invites`, `links`, `mentionRoles`, `mentionUsers`, `quickMessages`, `words` |
| amount   | [Number](#Number) | Yes      | The amount of strikes to be added |                                                                                                                                                              |

### Examples

<a name='strikeConfig'></a>

---

## !strikeConfig

Configura strikes recibidos por varias violaciones.

### Usage

```text
!strikeConfig [violation] [strikes]
```

### Aliases

- `!strike-config`

### Arguments

| Argument  | Type              | Required | Description        | Details                                                                                                                                                      |
| --------- | ----------------- | -------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| violation | [Enum](#Enum)     | No       | Tipo de violaci??n. | Use one of the following values: `allCaps`, `duplicateText`, `emojis`, `hoist`, `invites`, `links`, `mentionRoles`, `mentionUsers`, `quickMessages`, `words` |
| strikes   | [Number](#Number) | No       | Numero de strikes. |                                                                                                                                                              |

### Examples

```text
!strikeConfig
```

<a name='subtractFakes'></a>

---

## !subtractFakes

Remueve invitaciones falsas de todos los usuarios.

### Usage

```text
!subtractFakes
```

### Aliases

- `!subtract-fakes`
- `!subfakes`
- `!sf`

### Examples

```text
!subtractFakes
```

<a name='subtractLeaves'></a>

---

## !subtractLeaves

Remueve salidas de todos los usuarios.

### Usage

```text
!subtractLeaves
```

### Aliases

- `!subtract-leaves`
- `!subleaves`
- `!sl`

### Examples

```text
!subtractLeaves
```

<a name='support'></a>

---

## !support

Consigue un link de invitaci??n a nuestro servidor de soporte.

### Usage

```text
!support
```

### Examples

```text
!support
```

<a name='tryPremium'></a>

---

## !tryPremium

Prueba la versi??n premium de Invite Succubi gratis por un limitado periodo de tiempo.

### Usage

```text
!tryPremium
```

### Aliases

- `!try`
- `!try-premium`

### Examples

```text
!tryPremium
```

<a name='unban'></a>

---

## !unban

Unban a user

### Usage

```text
!unban <user> [reason]
```

### Arguments

| Argument | Type          | Required | Description                                         | Details |
| -------- | ------------- | -------- | --------------------------------------------------- | ------- |
| user     | [User](#User) | Yes      | The user that should be unbanned.                   |         |
| reason   | [Text](#Text) | No       | La raz??n por la cual este usuario no est?? excluido. |         |

### Examples

<a name='unhoist'></a>

---

## !unhoist

Add a character in front of all members with a special character in front of their name, so they will be shown at the end of the member list.

### Usage

```text
!unhoist
```

### Aliases

- `!dehoist`

### Examples

```text
!unhoist
```

<a name='unmute'></a>

---

## !unmute

Unmute a user

### Usage

```text
!unmute <user>
```

### Arguments

| Argument | Type              | Required | Description                              | Details |
| -------- | ----------------- | -------- | ---------------------------------------- | ------- |
| user     | [Member](#Member) | Yes      | El usuario que debe estar sin silenciar. |         |

### Examples

<a name='volume'></a>

---

## !volume

Set the volume if an argument is passed, or show the current volume.

### Usage

```text
!volume [volume]
```

### Arguments

| Argument | Type              | Required | Description                          | Details |
| -------- | ----------------- | -------- | ------------------------------------ | ------- |
| volume   | [Number](#Number) | No       | The value the volume will be set to. |         |

### Examples

```text
!volume
```

<a name='warn'></a>

---

## !warn

Advertir a un miembro

### Usage

```text
!warn <member> [reason]
```

### Arguments

| Argument | Type              | Required | Description                       | Details |
| -------- | ----------------- | -------- | --------------------------------- | ------- |
| member   | [Member](#Member) | Yes      | Usuario ha advertir.              |         |
| reason   | [Text](#Text)     | No       | Por qu?? el miembro fue advertido. |         |

### Examples
