---
description: Eventet bliver callet når et medlems rank i banden bliver ændret.
---

# BandeMemberRoleChangedEvent

**Import:** dk.plexhost.bande.events.BandeMemberRoleChangedEvent

|                        |                                          |                             |
| ---------------------- | ---------------------------------------- | --------------------------- |
| **Method**             | **Return Type**                          | **Beskrivelse**             |
| getBande()             | [Bande](../classes/bande.md)             | Banden.                     |
| getPlayer()            | Player                                   | Spilleren der ændre.        |
| getEditedBandePlayer() | [BandePlayer](../classes/bandeplayer.md) | Medlemet der bliver ændret. |
| getOldRole()           | [Role](../enums/role.md)                 | Medlemmets gamle rolle.     |
| getNewRole()           | [Role](../enums/role.md)                 | Medlemmets nye rolle.       |
