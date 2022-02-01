---
description: First line of defense against newly registered phishing/malicious domains!
---

# Heuristics detection

#### Background

Phish Grabber comes with several configureable heuristic features that gives servers first line of defense against unknown and not yet reported phishing domains.&#x20;

By nature phishing any discord related phishing domains are registered under the same day as it get spammed to reach higher yield of target groups.

Due to a consistent pattern from these bad actors, majority of them register few domain registrar that gives them a safe haven against any report against them.&#x20;



#### Detection condition

The bot will scan all links and determine which registrar a domain is registered under and if the domain was created very recently then Phish Grabber will sanction the users by default.&#x20;

Punishment type is enabled by default that is called "Heurisitic Protection". This can however be disabled by individual server owners.&#x20;

&#x20;

{% hint style="info" %}
**Did you know?**

Content Scan also have heuristic feature in nature that can block newly registered domains before it gets known by phishing APIs.&#x20;
{% endhint %}
