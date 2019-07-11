# Connections

**Important links**

* [How to get Discord IDs](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-)
* [How to get Messenger IDs](../faq.md#where-to-find-thread-id)

Your connection list is stored in a file named `connections.yml`. Example format:

{% code-tabs %}
{% code-tabs-item title="connections.yml" %}
```yaml
connection-name:
  - type: discord
    id: '1234'
  - type: messenger
    id: '5678'
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Each connection entry consists of "endpoint" blocks, which usually have 2 properties: **type** \(`discord`/`messenger`\) and **id**, both required when creating a connection.  
You can add as many endpoints to one connections as you want.  
Additionally, an endpoint can have a `readonly` property, which when set to `true` can make that endpoint read-only

On every launch Miscord will parse `connections.yml` to get a list of connections and will notify you if something's wrong.  
For each connection endpoint there will be added a name, so it will be more readable.

You can also configure connections with commands.  
The example above can be recreated using following commands:

```text
@Miscord add connection-name
@Miscord link connection-name discord 1234
@Miscord link connection-name messenger 5678
```

Example connections file \(~~used live on~~ [~~Miscord's Discord server~~](https://discord.gg/DkmTvVz) ~~in `#testing`~~Facebook banned my accounts\) :

{% code-tabs %}
{% code-tabs-item title="connections.yml" %}
```yaml
__comment: >-
  This is your connections.yml file. More info at
  https://github.com/miscord/miscord/wiki/Connections.yml
testing:
  - type: discord
    id: '433683136115900421'
  - type: messenger
    id: '1616656375118166'
dev:
  - type: discord
    id: '461611312196091321'
  - type: messenger
    id: '1709943095783086'
  - type: messenger
    id: '1458225837612649'
    readonly: true
```
{% endcode-tabs-item %}
{% endcode-tabs %}

Command representation:

```text
@Miscord add testing
@Miscord link testing discord 433683136115900421
@Miscord link testing messenger 1616656375118166
```

```text
@Miscord add dev
@Miscord link dev discord 461611312196091321
@Miscord link dev messenger 1709943095783086
@Miscord link dev messenger 1458225837612649
@Miscord readonly dev 1458225837612649 true
```

