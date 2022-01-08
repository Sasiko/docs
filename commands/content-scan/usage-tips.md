---
description: >-
  Content scan can be a very powerful tool if used correctly. In this page, we
  will attempt to showcase many ways how this function can serve in multiple
  type of purposes.
---

# Usage/Tips

## Multiple words per keyword

**Command example:**

/contentscan add-keywords keywords: discord nitro free, enjoy bigger file uploads

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2F18wGm1OMugXaV2W6JP9A%2Fexample%201.png?alt=media&token=49cce63b-a3c1-443e-8d76-be3d28bacc73" %}

From the image above, the bot will be able to scan these 2 keywords and flag the domain. \
By adding several words per keywords, it allows the bot to specifically target website that continues to use the same text content.&#x20;

Theres pros and cons by adding **multiple** words per keywords which will be listed below.

<mark style="color:green;">+ Highly specialized which will target specific type of website content.</mark>\ <mark style="color:green;">+ Less likely that legitimate domain will get flagged.</mark>\
<mark style="color:red;">-</mark> <mark style="color:red;">If a phishing website decides to change the entire text content then no match will be found.</mark>\ <mark style="color:red;">- Example Keyword 1 must match against identical words in the same order in order to get flagged. If website content has the following words in wrong order: nitro discord free then keyword 1 will not get matched.</mark>&#x20;

## Single word per keyword

**Command example:**

/contentscan add-keywords keywords: discord, nitro, free

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2Fe5jNIReBVtGB7b7ni2Ri%2Fexample%202.png?alt=media&token=3b1f155e-804d-4b56-a06f-e752a114e55e" %}

From the image above, it showcases that the bot will individually scan each word on the website content to match against your configured keyword.&#x20;

Theres pros and cons by adding **single** words per keywords which will be listed below.

<mark style="color:green;">+ Cover more variety of websites based on server owners preference, when configured correctly. More keywords you add, the less likely legitimate websites will get flagged.</mark> \
<mark style="color:red;">- Higher risk for flagging legitimate websites, as websites tend to use the same words. Requires more effort to configurate with accurate keywords.</mark>  \
<mark style="color:red;">- If you add fewer keywords, the chances are that the bot will flag more legitimate website because there's less specialization in your keyword configuration.</mark> \ <mark style="color:red;"></mark>
