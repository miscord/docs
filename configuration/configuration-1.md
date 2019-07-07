# Configuration

**Everything's optional, except for Messenger username/password and Discord token**

## [Config Generator](https://miscord.net/config-generator.html)

Default location of config file:

* Windows: `%appdata%/Miscord/config.json`
* Mac: `~/Library/Application Support/Miscord/config.json`
* Linux: `~/.config/Miscord/config.json`
* Other: `~/.miscord/config.json`

## Miscord

**Top-level values in the config**

| Variable name | Description | Default value |
| :--- | :--- | :--- |
| `logLevel` | Log level \(see [here](https://github.com/npm/npmlog#loglevelprefix-message-)\) | `info` |
| `checkUpdates` | Enables checking updates on every launch | `false` |
| `timezone` | Timezone for plan time parsing | \(none\) |
| `ignoredSequences` | Sequences to ignore messages containing them | `[]` |

## Channels

**These values should be in the `"channels": {}` block**

| Variable name | Description | Default value |
| :--- | :--- | :--- |
| `error` | Channel\(s\) for reporting errors, can be string or array | \(none\) |
| `command` | Channel\(s\) for sending commands, can be string or array | \(none\) |

## Messenger

**These values should be in the `"messenger": {}` block**

| Variable name | Description | Default value |
| :--- | :--- | :--- |
| `username` | Messenger username | :heavy\_multiplication\_x: |
| `password` | Messenger password | :heavy\_multiplication\_x: |
| `format` | Format of the message \(see [here](configuration/format)\) | `*{username}*: {message}` |
| `sourceFormat` | Format of the source in a Facebook message \(see more [here](configuration/format)\) | `{ "discord": "(Discord)", "messenger": "(Messenger: {name})" }` |
| `ignoreEmbeds` | Disables embed parsing from Discord | `false` |
| `attachmentTooLargeError` | Shows "attachment too large" error when sending to Discord | `true` |

## Discord

**These values should be in the `"discord": {}` block**

| Variable name | Description | Default value |
| :--- | :--- | :--- |
| `token` | Discord token | :heavy\_multiplication\_x: |
| `guild` | Discord guild \(server\) | \(none\) |
| `category` | Discord category name/id on the server | \(none\) |
| `renameChannels` | Renames channels according to Messenger | `true` |
| `showEvents` | Shows Facebook events \(join, leave, chat rename\) on Discord | `false` |
| `showFullNames` | Shows Facebook users' full names alongside their nicknames on Discord | `false` |
| `createChannels` | Enables creating new channels if not found \(enable if you want Miscord to create channels automatically according to your Messenger chats\) | `false` |
| `massMentions` | Allows mentioning `@everyone` and `@here` | `true` |
| `userMentions` | Allows mentioning regular users/roles | `true` |
| `ignoreBots` | Ignore all messages from bots \(or webhooks\) | `false` |
| `ignoredUsers` | Ignored users \(by ID\) | `[]` |

