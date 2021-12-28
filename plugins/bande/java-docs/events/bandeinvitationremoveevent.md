---
description: Eventet bliver callet når en player invitation bliver fjernet.
---

# BandeInvitationRemoveEvent

**Import:** dk.plexhost.bande.events.BandeInvitationRemoveEvent

|                      |                              |                                      |
| -------------------- | ---------------------------- | ------------------------------------ |
| **Method**           | **Return Type**              | **Beskrivelse**                      |
| getPlayer()          | Player                       | Spilleren der fjernede invitationen. |
| getBande()           | [Bande](../classes/bande.md) | Spillernes bande.                    |
| getInvitedUniqueId() | UUID                         | Inviteret spillers UUID              |
| getInvitedName()     | String                       | Inviteret spillers navn              |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
