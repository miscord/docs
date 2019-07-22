# Configuration

Configuration is split into 2 files: main config file named `config.json` and a list of connections named `connections.yml`.

All Miscord needs to run are Discord \(and Messenger\) credentials, but there's a bunch of options to customize to make Miscord suit your needs.

{% hint style="info" %}
If you haven't created a config file yet, just run Miscord and use the wizard to easily configure it.
{% endhint %}

Default location of config file:

* Windows: `%appdata%/Miscord/config.json`
* Mac: `~/Library/Application Support/Miscord/config.json`
* Linux: `~/.config/Miscord/config.json`
* Other: `~/.miscord/config.json`

### How to read

* Default values are specified after property name: `format` = `*{username}*: {content}`
* Type is specified in italics after property name: `Array<String> | String`. Union like this means that you can specify or string \(`"1234"`\), or array of strings \(`["1234", "5678"]`\).

### Config

* `logLevel` = `info` _String_  
  Levels:

  * `silent`
  * `fatal`
  * `error`
  * `warn`
  * `info`
  * `debug`
  * `trace`

 

* `api` Credentials used for API and dashboard See more here: [Dashboard](dashboard.md)
  * `username` _String_
  * `password` _String_ **or**
  * `key` _String_ 
* `checkUpdates` = `false` _Boolean_ Whether to check updates from GitHub on launch 
* `timezone` _String_ Used for time in the console, on plans and reminders from Messenger. List of timezones: [en.wikipedia.org](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) \(e.g., `Europe/Warsaw` or `America/New_York`\) 
* `ignoredSequences` _Array&lt;String&gt;_ I don't even know 
* `channels`
  * `error` _Array&lt;String&gt;_ \| _String_ Channel ID or list of channel IDs for reporting errors.  Highly recommended to set up. You can also use your user ID if you want to receive DMs.
  * `command` _Array&lt;String&gt;_ \| _String_ Channel ID or list of channel IDs for receiving commands. Check the list of commands by sending `@Miscord help`. As above, highly recommended and you can use your user ID. When using user ID, you don't need to ping the bot. 
* `discord` [DiscordConfiguration](discord.md) 
* `messenger` [MessengerConfiguration](messenger/)

