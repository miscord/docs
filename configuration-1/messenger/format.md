# Format examples

**From Discord:**

![Original message](../../.gitbook/assets/image.png)

![\*{username}\*: {content}](../../.gitbook/assets/image%20%281%29.png)

The default format, keep in mind that the bold text doesn't appear as bold on mobile Messenger yet.

![\[{username}\]: {content}](../../.gitbook/assets/image%20%282%29.png)

![\[{username}\] {source}: {newline} {content}](../../.gitbook/assets/image%20%283%29.png)

`messenger.sourceFormat.discord` is set here to `(#{name})`.  
Useful if you have multiple channels connected to one Messenger chat and want to know from which channel the message was.

\*\*\*\*

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

