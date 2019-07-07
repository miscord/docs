# FAQ

_What if I don't want to/can't run Miscord myself?_ You can donate $5 or more and get a gift code for up to 3 hosted instances for a month... basically, I do all the dirty work/host Miscord/keep it running for you. More info in \#announcements

**How do I find User/Server/Channel ID?** [https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-)

**Where to find "thread ID"?** _Group_

* Go to [messenger.com](https://messenger.com)
* Enter the chosen conversation
* In the URL bar you should have `https://messenger.com/t/(some numbers)`. Those numbers are this thread's ID.

  _One-to-one_

* Open that person's profile on Facebook and copy the link.
* Go to [Find my Facebook ID](https://findmyfbid.com/)
* Paste the link and click "Find Numeric ID"

**How to run Miscord in the background with auto-restart?** ~~You can use pm2~~ please don't Miscord has auto-restart embedded, just run it regularly \(you can use `tmux` on Linux to run it in the background\)

**I don't get messages, help??**

* Did you configure [connections list](Connections.yml)?
* Are you sending messages \(on FB\) from the same account as in the config? Miscord ignores its own messages to not repeat itself

**Why do edited messages on Discord not reflect on Facebook Messenger?** It's _impossible_. Facebook doesn't share any way to edit messages.

**Something is not working, help**

* Update to the latest version
* See Troubleshooting page [here](troubleshooting)
* Change logLevel to verbose
* Ask for help at \#support or \#bugs

  Error messages or logs are welcome

  If you're sure it's not your fault, create an issue [here](https://github.com/miscord/miscord/issues/new).

**Can I make Miscord ignore a single message?** Yes, you can use `m!keep` prefix at the beginning of your message to make Miscord ignore that message.

**Where to get an app password?** See here: [https://www.facebook.com/settings?tab=security&section=per\_app\_passwords](https://www.facebook.com/settings?tab=security&section=per_app_passwords)

**Facebook not working \(2-Factor Auth, login review\), help** Use app password \(see above\)

