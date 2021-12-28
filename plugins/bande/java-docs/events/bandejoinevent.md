---
description: Eventet bliver callet når en spiller joiner en bande.
---

# BandeJoinEvent

**Import:** dk.plexhost.bande.events.BandeJoinEvent

|             |                              |                       |
| ----------- | ---------------------------- | --------------------- |
| **Method**  | **Return Type**              | **Beskrivelse**       |
| getPlayer() | Player                       | Spilleren der joiner. |
| getBande()  | [Bande](../classes/bande.md) | Den joinede bande.    |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
