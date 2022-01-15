# RivalAddedEvent

**Import:** dk.plexhost.bande.events.RivalAddedEvent

|             |                              |                                 |
| ----------- | ---------------------------- | ------------------------------- |
| **Method**  | **Return Type**              | **Beskrivelse**                 |
| getBande()  | [Bande](../classes/bande.md) | Banden som tilføjede rivalen    |
| getRival()  | [Bande](../classes/bande.md) | Bandens rival.                  |
| getPlayer() | Player                       | Spilleren som tilføjede rivalen |

{% hint style="info" %}
Eventet extender **CancellableEvent,** og kan blive cancelled med **setCancelled(true)**
{% endhint %}
