---
description: >-
  A feature that allows the server owner to detect any website based on server
  owners own preference by adding their own keywords. By acessing website html
  content and match against keywords.
---

# Content Scanner

| Steps                                                                                                                       | Explanation                                                                  |
| --------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| <p>Step 1:  /settings<br>Step 2: Select Local Scanners<br>Step 3: Select Content scanner<br>Step 4: Manage Keyword List</p> | You can add multiple keywords, just ensure to add comma between each words.  |

| Steps                                                                                                                                | Explanation                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------- |
| <p>Step 1:  /settings<br>Step 2: Select Local Scanners<br>Step 3: Select Content scanner<br>Step 4: Manage Patterns (Regex) List</p> | You can add javascript regex expression with this configuration.  |

{% hint style="info" %}
**Useful tip:** You can choose to have the bot scan for a single word consecutively if you add a comma between each keyword or you can add several words in one single keyword.&#x20;

<mark style="background-color:purple;">Example usage:</mark>\
/contentscan add-keywords keywords: i like eating apple, but i dislike orange, lemon taste great\
_"i like eating apple"_ **This would count as 1 keyword.**\
****\
****If you add more words per keywords, the more specialized the bot will be when flagging against domains. This can be useful for matching specific sentences that some site uses, which usually yields a more surgicial target against a very specific website content.
{% endhint %}

{% hint style="info" %}
Content scan is disabled by default. To activate it, simply add keywords
{% endhint %}



