---
description: Archive of all the updates that has been released
---

# Updates

**30 January**

* Phishing database are now stores as RAM cache instead of sending request to a external api server to match the domain through external database. The local RAM cache is also synced with phishing apis database with help of websocket.&#x20;
* Help command added
* Whois command added&#x20;

**16 January**

* bugfix for logfixes again
* bugfix for whitelist/blacklist not properly checking the list.&#x20;
* Ignores blacklist/whitelist if several domains are posted under same message
* Now checks for edited messages
* Restructured punisher.ts and optimize the response time of the bot performance.

**3 January**

* logs not being posted properly

****

**26 December**

* Supporting additional phishing api.
* Added timeout feature
* Permission fix for commands

****

**25 December**

* Adding granular punishment options for scanner types: Antiphishing, Content scan, youtube and blacklist.

**Bug fixes**

* Content scan Punishment type didnt ignore youtube links.
* Fixed javascript regex types
* Critical fix that allowed bot to ignore some spam messages.
* logging fixes
* msgs get scanned twice when edited
* Youtube extraction issues for youtube shorts
* Change the way domains are extracted

**16 December**

**Bugfix:** Should fix the crashes when encountering errors such as unable to dm users, or permission issue such as manage delete

Bugfix: Ban/kick message not appearing

****

**15 December**

**Bugfix:** If one link is blacklisted by any factors while second link is whitelisted, bot ignores msg and ignore check This bugfix addresses that issue

****

**13 December**

**Bugfix:** Whitelist/Blacklist ineffective if a message contains 2 links that has blacklisted and whitelisted domain

****

**12 December**

* Guilds can now choose to delete, then kick or ban offending users
* Improved whitelist/blacklist checks. Bug fixed where bot still scans the domain if its posted with www and whitelist/blacklist contains without www. part Introduced global whitelist that applies to all guilds. Avoids doing unecessary checks such as google.com twitch.tv Saves additional server resources. Guild owners can choose to disable global whitelist though.

Guild owners own blacklist will override global whitelist.

* Bug fix where if one guild owner add a domain to whitelist/blacklist. then a different guild owner of differnt server try to do the same, it result with bot crash and unable to add the domain.

Improved commands. Some commands can now accept multiple values. IE ignore role @admin @moderator

```
main 
```

****

**11 December**

* Remove case sensitive when scanning domains.
* Restructured files for content scan and youtube

****

**11 December**

First public release with code refactoring. This bot was intially only used for my servers but changed to public as more servers encountered phishing spams.&#x20;
