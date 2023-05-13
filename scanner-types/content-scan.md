---
description: >-
  A data scraping feature that scans any websites html content in order to match
  against server owners blacklisted keywords.
---

# Content Scanner

## How Content scan works

Introducing Content Scanner, a powerful feature of my bot! With Content Scanner enabled, every message containing a link in a Discord channel is instantly scanned. The bot extracts the HTML content from the linked website and compares it against your server owner's blacklisted keyword phrases.

Content Scanner flags any domains based on their HTML content and matches them against your specified blacklisted keywords. This means you don't even need to know the exact URL to block undesirable links. For example, you can easily block specific YouTube links with video titles such as "How to get free Discord Nitro," "Get free Steam games," or "How to become rich with mining."

## Important to know

If executing this command with "orange, apple, banana", this will count as 1 phrase!

The bot will use these 3 separate words and try match against the html content from a domain. It doesn't matter which order these words are posted. As long as the html content contains all of these 3 words, the bot will flag that domain and sanction the user accordingly.

You can configure additional phrase such as "gold, red, yellow, pink, purple" which means the bot will then scan websites content for any of these phrases.

Note that the bot will not flag the website if the content does not contain all words from the same phrase. Example if the html content contains these words only:

Phrase 1 gold, red Phrase 2 apple

Then the bot will not flag the url. It must contain all words from the specific phrases to flag a domain.

## Default: <mark style="color:red;">Disabled</mark>

To configurate this scanner, follow these steps:

> **Step 1:** /settings\
> **Step 2:** _Select_ Server scanners\
> **Step 3:** Content scanner
