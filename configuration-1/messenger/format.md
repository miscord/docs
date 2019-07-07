# Format

If you want to format your messages on Messenger differently, you can change format value \(`config.messenger.format`\)

Supported variables:

* `{username}`
* `{message}` or `{content}`
* `{source}` \(`Discord` or `Messenger: group name` in case of Messenger linking\)

**Example:**  
Config:

```javascript
{
  "format": "[{username}] {source} {message}",
  "sourceFormat": {
    "discord": "(D)",
    "messenger": "(M - {name})"
  }
}
```

| Username | Input message | Source | Output message |
| :--- | :--- | :--- | :--- |
| Bjornskjald | Hello world! | Discord | \[Bjornskjald\] \(D\) Hello world! |
| Bjornskjald | Hello from Messenger | Messenger \(Group name: "Testing"\) | \[Bjornskjald\] \(M - Testing\) Hello from Messenger |

Source formats are also configurable:

* Discord \(`config.messenger.sourceFormat.discord`\): default `(Discord)`
* Messenger \(`config.messenger.sourceFormat.messenger`\): default `(Messenger: {name})`

