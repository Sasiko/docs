# Youtube

## How Youtube works

Youtube scanner type have 2 functions. 1 is for scanning content of youtube videos. 2 is for blocking specific youtube channel.

1. Helps you block any youtube videos based on youtube video contents. This function works similar to "Content scan" but specialized in youtube videos only. If you add keywords then Phish Grabber will scan any youtube video in order to match against your keywords.&#x20;
2. Block a specific youtube channel at your choosing. If any videos, newly uploaded or old, originates from the blacklisted channel, Phish Grabber will detect it and sanction the users accordingly, if enabled.&#x20;

## Important to know

If executing this command with "orange, apple, banana", this will count as 1 phrase!

The bot will use these 3 separate words and try match against the html content from a domain. It doesn't matter which order these words are posted. As long as the html content contains all of these 3 words, the bot will flag that domain and sanction the user accordingly.

You can configure additional phrase such as "gold, red, yellow, pink, purple" which means the bot will then scan websites content for any of these phrases.

Note that the bot will not flag the website if the content does not contain all words from the same phrase. Example if the html content contains these words only:

Phrase 1 gold, red Phrase 2 apple

Then the bot will not flag the url. It must contain all words from the specific phrases to flag a domain.

## Default: <mark style="color:red;">Disabled</mark>

To configurate this scanner, follow these steps:

> **/youtube add-keywords keywords:**
