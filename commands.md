# Commands

If you set `commandChannel` in your config \(it can be Channel ID or your User ID\), you can execute commands to configure Miscord while running. \(note: when using channel ID, you have to @ miscord for the command to be recognized\)

Commands available:

* `set <key> <value>` - sets value in the config
* `get <key>` - gets value from the config
* `link <Discord channel name or ID> <Facebook thread ID> [...more Facebook thread IDs]` - links one or more Facebook threads to a Discord channel
* `unlink <Facebook thread ID>` - removes existing link from the channel map
* `list` - shows existing connections
* `showConfig` - shows the entire config \(without username/password/token\)
* `help` - shows this message
* `quit` - exits Miscord

## 3.10.x and newer

Commands available:

* `set` - sets value in the config
* `get` - gets value from the config
* `add` - adds a new connection
* `remove` - removes an existing connection
* `list` - shows existing connections
* `info` - shows endpoints of an existing connection
* `link` - adds an endpoint to an existing connection
* `unlink` - removes an endpoint from an existing connection
* `showConfig` - shows the entire config
* `help` - shows this message
* `quit` - exits Miscord

