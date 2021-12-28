---
description: Event der bliver callet når et medlem slår et andet medlem.
---

# BandeDamageMemberEvent

**Import:** dk.plexhost.bande.events.BandeDamageMemberEvent

|               |                              |                              |
| ------------- | ---------------------------- | ---------------------------- |
| **Method**    | **Return Type**              | **Beskrivelse**              |
| getAttacker() | Player                       | Spilleren der angreb.        |
| getVictim()   | Player                       | Spilleren der blev angrebet. |
| getBande()    | [Bande](../classes/bande.md) | Spillernes bande.            |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
