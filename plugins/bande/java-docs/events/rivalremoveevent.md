---
description: Eventet bliver callet når en rival bliver fjernet.
---

# RivalRemoveEvent

**Import:** dk.plexhost.bande.events.RivalRemoveEvent

|             |                              |                                |
| ----------- | ---------------------------- | ------------------------------ |
| **Method**  | **Return Type**              | **Beskrivelse**                |
| getBande()  | [Bande](../classes/bande.md) | Banden som fjernede rivalen.   |
| getRival()  | [Bande](../classes/bande.md) | Bandens rival.                 |
| getPlayer() | Player                       | Spilleren som fjernede rivalen |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
