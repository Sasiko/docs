# Whitelist

| Commands                      | Explanation                                                                                        |
| ----------------------------- | -------------------------------------------------------------------------------------------------- |
| /whitelist add-domain domain: | Add domains so your content scan keywords and youtube keywords will ignore the whitelisted domain. |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FGNzdat0GVegjQptYYW0Y%2Fwhitelist-add.gif?alt=media&token=60f32c1a-f8e5-4d27-9c68-4d6f5919ebb2" %}
{% endtab %}
{% endtabs %}

{% hint style="info" %}
If you want to whitelist 1 domain then you need to add the same domain twice. \
Example:&#x20;

www.google.com

google.com

The reason is because www. is considered a subdomain and the nature of how Munio is extracting domains, it only look for specific domain and ignores subdomains.&#x20;
{% endhint %}



| Commands        | Explanation                             |
| --------------- | --------------------------------------- |
| /whitelist view | Display list of all whitelisted domains |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FEW3eg8IpQ1GCRfRklboJ%2Fwhitelist-view.gif?alt=media&token=73f2f1de-9dbd-4aa8-8ab8-362cb8e5ec1c" %}
{% endtab %}
{% endtabs %}



| Commands                 | Explanation                          |
| ------------------------ | ------------------------------------ |
| /whitelist remove entry: | Remove a specific whitelisted domain |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FjvosFKAp8NdpcdZGqG7N%2Fwhitelist-remove.gif?alt=media&token=d73c6ccc-e7c1-4355-95f9-45710571ac1d" %}
{% endtab %}
{% endtabs %}
