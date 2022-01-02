# Blacklist

| Commands                      | Explanation                                                                                                     |
| ----------------------------- | --------------------------------------------------------------------------------------------------------------- |
| /blacklist add-domain domain: | By adding a blacklisted domain, content scan will be able to detect that domain and sanction users accordingly. |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FrJCwT21igGCXIiDFrL06%2Fblacklist-add.gif?alt=media&token=32f657da-6162-46e6-9126-f62fbce4dd86" %}
{% endtab %}
{% endtabs %}

{% hint style="info" %}
If you want to blacklist 1 domain then you need to add the same domain twice. \
Example:&#x20;

www.google.com

google.com

The reason is because www. is considered a subdomain and the nature of how phish grabber is extracting domains, it only look for specific domain and ignores subdomains.
{% endhint %}



| Commands        | Explanation                             |
| --------------- | --------------------------------------- |
| /blacklist view | Display list of all whitelisted domains |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2F6D6PgbAEh4ghkiNW8y3V%2Fblacklist-view.gif?alt=media&token=a8f246d3-848e-4c82-b5a2-5a300657a1a4" %}
{% endtab %}
{% endtabs %}



| Commands                 | Explanation                         |
| ------------------------ | ----------------------------------- |
| /blacklist remove entry: | Removes a domain from the blacklist |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FBzewj0ebDFFK7YqipQhD%2Fblacklist-remove.gif?alt=media&token=12896520-3ec0-455a-a68c-478145f0ae24" %}
{% endtab %}
{% endtabs %}
