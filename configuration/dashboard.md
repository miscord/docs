# Dashboard

Web dashboard is an easy way of managing your Miscord instance.

If you're running Miscord for the first time without a config, it will automatically set up the dashboard settings for you.  
Otherwise, you need to add an api block to your config \(port is optional\):

{% code title="config.json" %}
```javascript
"api": {
  "username": "ptrcnull",
  "password": "hunter2",
  "port": 1234
}
```
{% endcode %}

{% hint style="warning" %}
The `api` block should not be in other blocks like `messenger` or `discord`
{% endhint %}



