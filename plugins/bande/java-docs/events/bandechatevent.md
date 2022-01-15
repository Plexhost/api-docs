---
description: >-
  Eventet bliver callet når en spiller sender en besked i ALL, ALLY eller BANDE
  chatten.
---

# BandeChatEvent

**Import:** dk.plexhost.bande.events.BandeChatEvent

|              |                                  |                                |
| ------------ | -------------------------------- | ------------------------------ |
| **Method**   | **Return Type**                  | **Beskrivelse**                |
| getPlayer()  | Player                           | Spilleren der sendte beskeden. |
| getMessage() | String                           | Beskeden der bliver sendt.     |
| getType()    | [ChatType](../enums/chattype.md) | Chat typen der bliver sendt.   |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
