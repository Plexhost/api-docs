---
description: Eventet bliver callet når et medlem køber noget fra bande shoppen.
---

# BandeShopEvent

**Import:** dk.plexhost.bande.events.BandeShopEvent

|             |                              |                   |
| ----------- | ---------------------------- | ----------------- |
| **Method**  | **Return Type**              | **Beskrivelse**   |
| getPlayer() | Player                       | Spilleren.        |
| getBande()  | [Bande](../classes/bande.md) | Banden.           |
| getPrice()  | int                          | Prisen på itemet. |
| getItem()   | String                       | Itemets id.       |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
