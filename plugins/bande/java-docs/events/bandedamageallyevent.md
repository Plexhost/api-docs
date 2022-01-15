---
description: Event der bliver callet når en spiller slår en allieret.
---

# BandeDamageAllyEvent

**Import:** dk.plexhost.bande.events.BandeDamageAllyEvent

|                    |                              |                              |
| ------------------ | ---------------------------- | ---------------------------- |
| **Method**         | **Return Type**              | **Beskrivelse**              |
| getAttacker()      | Player                       | Spilleren der angreb.        |
| getVictim()        | Player                       | Spilleren der blev angrebet. |
| getAttackerBande() | [Bande](../classes/bande.md) | Attacker's bande.            |
| getAllyBande()     | [Bande](../classes/bande.md) | Victim's bande.              |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
