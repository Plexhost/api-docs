---
description: Eventet bliver callet når en bande bliver slettet.
---

# BandeDeleteEvent

**Import:** dk.plexhost.bande.events.BandeDeleteEvent

|                 |                                      |                    |
| --------------- | ------------------------------------ | ------------------ |
| **Method**      | **Return Type**                      | **Beskrivelse**    |
| getName()       | String                               | Bandens navn.      |
| getId()         | int                                  | Bandens id.        |
| getMembers()    | List\<UUID>                          | Bandens medlemmer. |
| getDeleteType() | [DeleteType](../enums/deletetype.md) | -                  |
