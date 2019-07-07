# How to create a Discord bot

* Go [here](https://discordapp.com/developers/applications/me)
* Click "Create an application"

![screenshot of the big button with a plus sign](https://static.bjorn.ml/miscord-wiki-screenshots/1.png)

* Give your bot a name \(it can be anything, it won't be visible to others\)
* Also, copy the Client ID. We'll need it later

![screenshot of the name field](https://static.bjorn.ml/miscord-wiki-screenshots/2.png)

* Don't forget to save the changes!

![screenshot of the save changes button](https://static.bjorn.ml/miscord-wiki-screenshots/3.png)

* Go to the "Bot" tab

![screenshot of the bot tab](https://static.bjorn.ml/miscord-wiki-screenshots/4.png)

* Add a new bot

![screenshot of the add bot button](https://static.bjorn.ml/miscord-wiki-screenshots/5.png)

* Give your bot a username \(it'll be public\)

![screenshot of bot&apos;s name](https://static.bjorn.ml/miscord-wiki-screenshots/6.png)

* Copy the link below and replace \(your id here\) with your Client ID you copied before  

  ```text
  https://discordapp.com/api/oauth2/authorize?client_id=(your id here)&permissions=805829712&scope=bot
  ```

  Example link:

  ```text
  https://discordapp.com/api/oauth2/authorize?client_id=4803666206452613&permissions=805829712&scope=bot
  ```

**Permissions:**

![screenshot of the list of permissions](https://static.bjorn.ml/miscord-wiki-screenshots/9.png)

* Open that link, choose your server and click "authorize"

![screenshot of the authorize button](https://static.bjorn.ml/miscord-wiki-screenshots/7.png)

* Go back and enter the "bot" tab once again

![screenshot of the bot tab](https://static.bjorn.ml/miscord-wiki-screenshots/4.png)

* Copy the token and paste it into your config/config generator

![screenshot of the bot tab](https://static.bjorn.ml/miscord-wiki-screenshots/8.png)

