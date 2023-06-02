---
description: >-
  A feature that allows the server owner to detect any website based on server
  owners own preference by adding their own keywords. By acessing website html
  content and match against keywords.
---

# How-to Content Scanner

## How keywords works

![](<../.gitbook/assets/bild (1).png>)

When you add multiple keywords from the screenshot, Munio will match them in the specified order when scraping websites. For instance, if you add several keywords, you will have to add a comma to separate individual keywords example "Banana, Apple, Orange," \
\
Munio will flag a link if the HTML content contains these words in that exact order. However, it will not flag the link if the words are in a different order, such as "Apple, Orange, Banana."

If you want Munio to detect these three words without a specific order, you should add each keyword separately. In the "Add keywords" picture above, add only "banana" and click submit. Then, add a new keyword and repeat the process, adding only one keyword at a time. For example, add "orange," and so on.

<table><thead><tr><th>Steps</th><th width="394">Explanation</th></tr></thead><tbody><tr><td>Step 1:  /settings<br>Step 2: Select Local Scanners<br>Step 3: Select Content scanner<br>Step 4: Manage Keyword List</td><td>You can add multiple keywords, just ensure to add comma between each words. </td></tr></tbody></table>

<table><thead><tr><th width="353">Steps</th><th>Explanation</th></tr></thead><tbody><tr><td>Step 1:  /settings<br>Step 2: Select Local Scanners<br>Step 3: Select Content scanner<br>Step 4: Manage Patterns (Regex) List</td><td>You can add javascript regex expression with this configuration. </td></tr></tbody></table>

{% hint style="info" %}
**Useful tip:** You can choose to have the bot scan for a single word consecutively if you add a comma between each keyword or you can add several words in one single keyword.&#x20;

<mark style="background-color:purple;">Example usage:</mark>\
If a html content contains this sentence: \
<mark style="background-color:blue;">i like eating apple, but i dislike orange, lemon taste great</mark>\
and server owner add this keyword _"**i like eating apple**"_ \
**This would count as 1 keyword and will flag the link.**\
\
If you add more words per keywords, the more specialized the bot will be when flagging against domains. This can be useful for matching specific sentences that some site uses, which usually yields a more surgicial target against a very specific website content.
{% endhint %}

{% hint style="info" %}
Content scan is disabled by default. To activate it, simply add keywords
{% endhint %}



