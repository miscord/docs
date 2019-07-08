---
description: 'These values should be in the "messenger": {} block'
---

# Messenger config

* `username` _String_ Messenger username, email or phone number ****
* `password` _String_ Messenger password \(or [app password](../../faq.md)\) 
* `format` = `*{username}*: {message}` _String_  
  Format of the message sent to Messenger  
  See examples [here](format.md)  
  Supported "variables":

  * `{username}`
  * `{message}` or `{content}`
  * `{source}` - specified in `messenger.sourceFormat`

* `sourceFormat`  
  The `{source}` from `messenger.format` above  
  You can use `{name}` here which will be substituted for channel/chat name.

  * `messenger` = `(Messenger: {name})` _String_
  * `discord` = `(Discord)` _String_

  \_\_

* `ignoreEmbeds` = `false` _Boolean_ Whether to parse embeds from Discord \(Embeds are more extensible messages, e.g. link previews or some messages from bots which have a title\) 
* `attachmentTooLargeError` = `true` _Boolean_ Whether to show "attachment too large" error when sending to Discord

