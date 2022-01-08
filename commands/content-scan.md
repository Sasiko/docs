---
description: >-
  A feature that allows the server owner to detect any website based on server
  owners own preference by adding their own keywords. By acessing website html
  content and match against keywords.
---

# Content Scan

| Commands                            | Explanation                                                                  |
| ----------------------------------- | ---------------------------------------------------------------------------- |
| /contentscan add-keywords keywords: | You can add multiple keywords, just ensure to add comma between each words.  |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FptnlqXieqil9xh6J32eI%2Fcontent-scan-add.gif?alt=media&token=b8a74452-110a-4442-96fd-a8472408e497" %}


{% endtab %}
{% endtabs %}

{% hint style="info" %}
**Useful tip:** You can choose to have the bot scan for a single word consecutively if you add a comma between each keyword or you can add several words in one single keyword.&#x20;

<mark style="background-color:purple;">Example usage:</mark>\
/contentscan add-keywords keywords: i like eating apple, but i dislike orange, lemon taste great\
_"i like eating apple"_ **would count as 1 keyword.**\
****\
****If you add multiple words in one keywords then the bot will search for that specific keywords. This can be useful for matching specific sentence which usually yields more accurate domain detection.&#x20;
{% endhint %}

{% hint style="info" %}
Content scan is disabled by default. To activate it, simply add keywords
{% endhint %}



| Commands                   | Explanation                                                              |
| -------------------------- | ------------------------------------------------------------------------ |
| /contentscan list-keywords | This command will list all the keywords you have added for content scan. |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FB5rljnwl4BtCdolgsszL%2Fcontentscan-view.gif?alt=media&token=04812f4c-66a4-469a-9f27-4242aba7d3d5" %}


{% endtab %}
{% endtabs %}



| Commands                               | Explanation                                                                |
| -------------------------------------- | -------------------------------------------------------------------------- |
| /contentscan remove-keywords keywords: | Delete your keywords. Has to be identical in order to remove the keywords. |

{% tabs %}
{% tab title="Command demonstration" %}
{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FExRFSiGGE6uXpYA2tMPv%2Fuploads%2FLJmN97mImVgNBDoTaRWm%2Fcontent-scan-remove.gif?alt=media&token=6147dd17-dda3-45f0-8632-7664d132af94" %}
{% endtab %}
{% endtabs %}
