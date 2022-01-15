---
description: Eventet bliver callet når en bande stiger i level.
---

# BandeLevelupEvent

**Import:** dk.plexhost.bande.events.BandeJoinEvent

|               |                              |                                      |
| ------------- | ---------------------------- | ------------------------------------ |
| **Method**    | **Return Type**              | **Beskrivelse**                      |
| getPlayer()   | Player                       | Spilleren der stiger banden i level. |
| getBande()    | [Bande](../classes/bande.md) | Banden.                              |
| getLevel()    | int                          | Bandens nye level.                   |
| setLevel(int) | void                         | Sæt bandens nye level.               |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
