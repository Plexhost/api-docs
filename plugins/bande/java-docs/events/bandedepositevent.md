---
description: Eventet bliver callet når et medlem indsætter penge i banden.
---

# BandeDepositEvent

**Import:** dk.plexhost.bande.events.BandeDamageMemberEvent

|                 |                              |                                 |
| --------------- | ---------------------------- | ------------------------------- |
| **Method**      | **Return Type**              | **Beskrivelse**                 |
| getPlayer()     | Player                       | Spilleren der indsatte penge.   |
| getBande()      | [Bande](../classes/bande.md) | Spillernes bande.               |
| getAmount()     | long                         | Penge der bliver indsat.        |
| setAmount(long) | void                         | Sæt antallet der bliver indsat. |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
