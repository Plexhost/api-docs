---
description: Eventet bliver callet når en bande acceptere en alliance.
---

# AllyAcceptedEvent

**Import:** dk.plexhost.bande.events.AllyAcceptedEvent

|                    |                              |                                  |
| ------------------ | ---------------------------- | -------------------------------- |
| **Method**         | **Return Type**              | **Beskrivelse**                  |
| getBandeWhoAsked() | [Bande](../classes/bande.md) | Banden som spurgte om allierede. |
| getAskedBande()    | [Bande](../classes/bande.md) | Banden som accepterede.          |
| getPlayer()        | Player                       | Spilleren som accepterede.       |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
