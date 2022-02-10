---
description: Archive of all the updates that has been released
---

# Updates

**10 Feburary**

Todays update is only QOL meant to optimize Phish Grabber performance.

* Using discord hybrid sharding. It is a new library that leaves fewer RAM footprint than DJS internal sharding.
* Reduced 50% amount of database calls. This was unnecessary roundtrip as it delayed bot additionally from executing its punishment in good time.
* Changed the list comparison method in order to reduce as many IF loops as possible. Too many loops created unnecessary overhead when executing its primary function.
* Added listeners for shard and client to monitor closely on errors.
* Rewriting Scanner types files used to have many regex type which creates pointlessly amount of overhead. The regex was gradually added as more scanner types were introduced in early phase of the bot development. Removed all internal regex to improve faster code execution.
* Cleanup slash command handlers and use built on required functionality over manual checking
* Slash commands are getting registered multiple times due to current approach when sharding. This does not create duplicate commands but highly ineffective and wasteful.

**7 Feburary**

* Added error catching so it shows logs when bot restart. This should allow me to analyse the logs, why bot auto restarts

There is still persisting issue with youtube-dl process always exiting with non 0 return code. Temporary fix is applied until a permanent has been found.

* Ignores large json dumps. Should improve the youtube feature where it can search faster now

\
\
**6 February**&#x20;

Major Update released Heuristic Protection is now enabled by default FOR ALL SERVERS. This bot will basically scan ALL domains and match against global registrar ban or local registrar ban.

Global registrar check

1. registrar of domain names reg.ru llc \[Domain age 20 days or younger]
2. regru-ru \[Domain age 20 days or younger]
3. regional network information center, jsc dba ru-center \[Domain age 20 days or younger]
4. hosting concepts b.v. d/b/a registrar.eu \[Domain age 10 days or younger]
5. hosting concepts b.v. d/b/a \[Domain age 10 days or younger]

How does registrar check protect my server? Global list has 2 condition for it to trigger the punishment. If the domain was registered under the company called registrar from the "Global registrar" list and check for domain creation date.

But why would this protection be useful? Based on my personal experience checking thousands of reported discord phishing domains, I can conclude that MAJORITY of these domains are registered under those 5 listed companies/registrar. These phishing domains are usually created under the same day as it get mass spammed in thousands of discord servers to reach more audience.

Why Heuristic protection and Phishing API compliments each other Phishing API are based on a community among bot developers where we report new phishing domains. Basically, API is based on reactive meassure, of mass spam that has already taken place. It usually take 20 minutes for new phishing domain to be added to API database. But those 20 minutes might have already reached to tens of thousands of users already, which is the weakpoint of only using phishing API.

Enters Heuristic protection, where it can flag newly registered domains and block it before it gets known by phishing apis. Because it only check based on domain age and from specific registrar, it weakpoint is that it cant cover a specific domain which has been flagged by heuristic protection forever as it check for domain age. Which is where Phishing API will cover that weakpoint since by the time 10 days have passed, that phishing domain would already been listed to phishing API, thus giving you a more robust protection against phishing domains.

Note Content scan act heuristically as well if you configure keywords that instruct the bot to check when scanning for websites html contents.

New function added

* Heuristic protection You can adjust the punishment types via this command: /punishment set-punishment scanner:

Add a domain registrar for bot to check against. Use /whois command to find the registrar name in order for bot to check the name. After adding the name, simply select AGE

If you don't add domain age, you will completely ban a domain registrar. BE CAREFUL WITH THIS. /heuristicprotection add-registrar registrar:

/heuristicprotection view-registrars

/heuristicprotection remove-registrars

* Content scan has been separated from Phish Grabber. It is now a separated local API due to the nature how content scan works, it can be resource demanding. By isolating the resource intensive tasks this should optimize the bot performance additionally

****

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
