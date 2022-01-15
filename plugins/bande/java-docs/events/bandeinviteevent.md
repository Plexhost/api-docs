---
description: Eventet bliver callet når en spiller bliver inviteret til en bande.
---

# BandeInviteEvent

**Import:** dk.plexhost.bande.events.BandeInviteEvent

|              |                              |                                 |
| ------------ | ---------------------------- | ------------------------------- |
| **Method**   | **Return Type**              | **Beskrivelse**                 |
| getInviter() | Player                       | Spilleren der invitere.         |
| getInvited() | Player                       | Spilleren der bliver inviteret. |
| getBande()   | [Bande](../classes/bande.md) | Spillernes bande.               |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
