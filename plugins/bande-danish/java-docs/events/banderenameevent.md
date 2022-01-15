---
description: Eventet bliver callet når en bande bliver renamet.
---

# BandeRenameEvent

**Import:** dk.plexhost.bande.events.BandeRenameEvent

|              |                              |                        |
| ------------ | ---------------------------- | ---------------------- |
| **Method**   | **Return Type**              | **Beskrivelse**        |
| getPlayer()  | Player                       | Spilleren der renamer. |
| getBande()   | [Bande](../classes/bande.md) | Banden.                |
| getOldName() | String                       | Bandens gamle navn.    |
| getNewName() | String                       | Bandens nye navn.      |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
