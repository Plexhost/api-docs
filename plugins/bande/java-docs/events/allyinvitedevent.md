---
description: Eventet bliver callet når en bande spørger en anden bande om alliance.
---

# AllyInvitedEvent

**Import:** dk.plexhost.bande.events.AllyInvitedEvent

|             |                              |                                      |
| ----------- | ---------------------------- | ------------------------------------ |
| **Method**  | **Return Type**              | **Beskrivelse**                      |
| getBande()  | [Bande](../classes/bande.md) | Banden som spurgte om allierede.     |
| getAlly()   | [Bande](../classes/bande.md) | Banden som blev spurgt om allierede. |
| getPlayer() | Player                       | Spilleren som spurgte.               |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
