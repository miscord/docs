# Quick start

## Installation

### Standard

🏁 **Windows**

Download the .exe [here](https://download.miscord.net/win.zip) \(32-bit version [here](https://download.miscord.net/win32.zip)\)

🐧 **Linux**

Download the executable [here](https://download.miscord.net/linux.zip) \(32-bit version [here](https://download.miscord.net/linux32.zip)\)

🍎 **macOS**

Install Miscord using [Homebrew](https://brew.sh/):

```text
bash /usr/bin/ruby -e "$(curl -fsSL` https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew tap miscord/miscord
brew cask install miscord
```

or download the app directly [here](https://download.miscord.net/macapp.zip)

### Advanced

🐳 **Docker**

Run command:

```text
docker run -d -v /home/bjorn/Documents/miscord:/config miscord/miscord
```

Example docker-compose.yml:  
\(_when replacing the path, keep_ ":/config" _at the end of it_\)

```yaml
version: '3'
services:
  miscord:
    image: miscord/miscord:latest
    volumes:
      - /home/bjorn/Documents/miscord:/config
```

**NPM \(all platforms\)**

* Install Node.js using instructions [here](https://github.com/miscord/docs/tree/869f6068a6791a3ea5626f000165348f4e6047b1/node.js)
* Install Miscord using `npm install -g miscord`

\(On Mac or Linux, prefix `sudo` is needed if you are not root user, i.e. `sudo npm install -g miscord`\)  
You can follow the guide [here](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo.md) to install global packages without admin permissions

## Setup

* Create a Discord bot \(see [here](https://github.com/miscord/docs/tree/869f6068a6791a3ea5626f000165348f4e6047b1/installation/Creating-a-Discord-bot/README.md)\)
* Create a dedicated Facebook account
  * make it look believable
  * try to come up or generate a fake name \(you can set the nickname for it in the chat\)
  * you can use a profile picture from [https://thispersondoesnotexist.com/](https://thispersondoesnotexist.com/)
  * log into it on a phone \(Messenger app\)
* Generate config [here](https://miscord.net/config-generator.html) - config options explained [here](https://github.com/miscord/docs/tree/869f6068a6791a3ea5626f000165348f4e6047b1/installation/Configuration/README.md)
* Build your connections \(see [here](https://github.com/miscord/docs/tree/869f6068a6791a3ea5626f000165348f4e6047b1/installation/Connections.yml), you have to do it by hand for now\)

