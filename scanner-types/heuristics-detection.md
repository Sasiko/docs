---
description: First line of defense against newly registered phishing/malicious domains!
---

# Heuristics detection

#### Background

Phish Grabber comes with several configureable heuristic features that gives servers first line of defense against unknown and not yet reported phishing domains. This is enabled by default.

By nature any discord related phishing domains  are registered and spammed under the same day. Majority of them register few domain registrar that gives them a safe haven against any reports against them. Because of these predictable patterns, it allows Phish Grabber to detect these pattern and block these new registered domains before it even has the chance to spam in your server.

#### Detection condition

The bot will scan all links and determine which registrar a domain is registered under and if the domain was created very recently then Phish Grabber will sanction the users by default.&#x20;

Punishment type is enabled by default that is called "Heurisitic Protection". This can however be disabled by individual server owners.&#x20;

{% hint style="info" %}
**Did you know?**

Content Scan also have heuristic feature in nature that can block newly registered domains before it gets known by Phish Grabber's phishing APIs.&#x20;
{% endhint %}

## &#x20;Default: <mark style="color:green;">Enabled</mark>

Bot will by default auto delete message and timeout users from all servers if the link match against globally or/and local blacklisted domain registrar.

**Default punishment type:** Delete & Timeout
