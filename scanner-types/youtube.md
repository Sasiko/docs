# Profile picture scan

## How Global avatar list works

Phish Grabber scans profile picture when new user join your server and when they are in your server and changes to a new profile picture. Bot will now match any profile pictures with the aforementioned conditions against the bots database of blacklisted profile pictures using similarity comparison that works like Google reverse image search.&#x20;

The blacklisted profile picture will only get added to the database if DM BOT spammers uses multiple accounts with the same profile picture. This feature will be extremely useful protecting your server against **DM SPAMMERS** that impersonate discord staff or any known dm spammers.



{% hint style="info" %}
Bot will by default auto kick users from all servers if the users profile picture match against the profile picture database.\
To disable the punishment simply use this command to disable it.



<mark style="background-color:blue;">**/punishment set-punishment scanner:Global Avatar List**</mark>
{% endhint %}

\






