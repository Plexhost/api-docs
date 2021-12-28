---
description: Eventet bliver callet før en bande bliver slettet.
---

# BandePreDeleteEvent

**Import:** dk.plexhost.bande.events.BandePreDeleteEvent

|                 |                                      |                               |
| --------------- | ------------------------------------ | ----------------------------- |
| **Method**      | **Return Type**                      | **Beskrivelse**               |
| getPlayer()     | Player                               | Spilleren der sletter banden. |
| getBande()      | [Bande](../classes/bande.md)         | Banden der bliver slettet.    |
| getDeleteType() | [DeleteType](../enums/deletetype.md) | -                             |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
