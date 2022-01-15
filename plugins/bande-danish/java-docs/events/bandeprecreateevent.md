---
description: Eventet bliver callet før en bande bliver oprettet.
---

# BandePreCreateEvent

**Import:** dk.plexhost.bande.events.BandePreCreateEvent

|             |                 |                                           |
| ----------- | --------------- | ----------------------------------------- |
| **Method**  | **Return Type** | **Beskrivelse**                           |
| getPlayer() | Player          | Spilleren der prøver at oprette en bande. |
| getName()   | String          | Den kommende bandes navn.                 |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
