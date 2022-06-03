# Youtube

## How Youtube works

Phish Grabber scans profile picture when new user join your server and when they are in your server and changes to a new profile picture. Bot will now match any profile pictures with the aforementioned conditions against the bots database of blacklisted profile pictures using similarity comparison that works like Google reverse image search. The blackllisted profile picture will only get added to the database if DM BOT spammers uses multiple accounts with the same profile picture. This feature will be extremely useful protecting your server against **DM SPAMMERS** that impersonate discord staff or any known dm spammers.

\


## Important to know

If executing this command with "orange, apple, banana", this will count as 1 phrase!

The bot will use these 3 separate words and try match against the html content from a domain. It doesn't matter which order these words are posted. As long as the html content contains all of these 3 words, the bot will flag that domain and sanction the user accordingly.

You can configure additional phrase such as "gold, red, yellow, pink, purple" which means the bot will then scan websites content for any of these phrases.

Note that the bot will not flag the website if the content does not contain all words from the same phrase. Example if the html content contains these words only:

Phrase 1 gold, red Phrase 2 apple

Then the bot will not flag the url. It must contain all words from the specific phrases to flag a domain.

By default, content scan feature is disabled until server owners add any keywords using this command:

> /youtube add-keywords keywords:

## Default: <mark style="color:red;">Disabled</mark>

By default, youtube feature is disabled until server owners add any keywords using this command:

> /youtube add-keywords keywords:
