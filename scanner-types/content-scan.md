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

## Configurational options

| Regex    | Accept only ECMAscript/Javascript regex language. Visit this [site](https://regex101.com/) to test your regex expressions.                                  |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Keywords | You can configure additional phrase such as "gold, red, yellow, pink, purple" which means the bot will then scan websites content for any of these phrases. |

&#x20;

{% hint style="info" %}
It is highly recommended you visit following pages [How-to Content Scanner](../commands/content-scan.md) <mark style="color:red;">**and**</mark> [Usage/Tips](../commands/content-scan/usage-tips.md) on how to effectively use this datascraping feature.
{% endhint %}



## Default: <mark style="color:red;">Disabled</mark>

To configurate this scanner, follow these steps:

> **Step 1:** /settings\
> **Step 2:** _Select_ Server scanners\
> **Step 3:** Content scanner
