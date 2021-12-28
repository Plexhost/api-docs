---
description: Eventet bliver callet når en bande fjerner en bande som allierede.
---

# AllyRemoveEvent

**Import:** dk.plexhost.bande.events.AllyRemoveEvent

|             |                              |                                  |
| ----------- | ---------------------------- | -------------------------------- |
| **Method**  | **Return Type**              | **Beskrivelse**                  |
| getBande()  | [Bande](../classes/bande.md) | Banden som opløste alliancen.    |
| getAlly()   | [Bande](../classes/bande.md) | Den allierede bande.             |
| getPlayer() | Player                       | Spilleren som opløste alliancen. |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
