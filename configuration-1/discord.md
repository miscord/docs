---
description: 'These values should be in the "discord": {} block'
---

# Discord config

* `token` _String_ Discord bot token 
* `guild` _String_ Discord default server ID \(used only when `createChannels` is `true`\)  
* `category` _String_  
  Discord default category ID

  \(used only when `createChannels` is `true`\)   

* `renameChannels` = `true` _Boolean_ Whether to rename channels according to Messenger chat name updates Works only with one-to-one connections 
* `showFullNames` = `false` _Boolean_ Whether to show full names from Messenger messages instead of nicknames 
* `createChannels` = `false` _Boolean_ Whether to create channels on receiving a message in an unknown chat on Messenger Works best when using Miscord with a personal account 
* `massMentions` = `false` _Boolean_ Whether to allow `@everyone` and `@here` mentions 
* `userMentions` = `true` _Boolean_ Whether to allow mentioning Discord users 
* `roleMentions` = `true` _Boolean_ Whether to allow mentioning Discord roles 
* `ignoreBots` = `false` _Boolean_ Whether to ignore all messages from bots or webhooks 
* `ignoredUsers` _Array&lt;String&gt;_ IDs of users, whose messages will be ignored and not forwarded anywhere

