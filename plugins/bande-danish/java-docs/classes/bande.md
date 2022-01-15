# Bande

**Import:** dk.plexhost.bande.bande.Bande

|                                                            |                               |                                                                                       |
| ---------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------- |
| **Method**                                                 | **Return Type**               | **Beskrivelse**                                                                       |
| addBank(long)                                              | void                          | Tilføj penge til banden.                                                              |
| addMember(Player)                                          | void                          | Tilføj en spiller til banden.                                                         |
| addStat(String, int)                                       | void                          | Tilføj **int** til bandens stat **String**                                            |
| changeMember(UUID, int)                                    | void                          | Ændre et medlems rank i banden.                                                       |
| decrementAllySkade()                                       | void                          | Nedsæt bandens allyskade med 1.                                                       |
| decrementBandeSkade()                                      | void                          | Nedsæt bandens bandeskade med 1.                                                      |
| delete()                                                   | void                          | Sletter banden.                                                                       |
| getAmountOfAllies()                                        | int                           | Få antallet af allierede.                                                             |
| getAmountOfMembers()                                       | int                           | Få antallet af medlemmer.                                                             |
| getAmountOfRivals([RivalsType](../enums/rivalstype.md))    | int                           | Få antallet af rivaler.                                                               |
| getCreated()                                               | Date                          | Hvornår banden blev oprettet.                                                         |
| getCustomVariableString(String, String)                    | String                        | Returner en custom **String** variable, og ellers en default.                         |
| getCustomVariableInt(String, int)                          | int                           | Returner en custom **int** variable, og ellers en default.                            |
| getCustomVariableBoolean(String, boolean)                  | boolean                       | Returner en custom **boolean** variable, og ellers en default.                        |
| getLastSeen()                                              | Date                          | Hvornår en medlem fra banden sidst blev set.                                          |
| getLevel()                                                 | int                           | Bandens level.                                                                        |
| getMaxAllies()                                             | int                           | Bandens maksimale antal allierede.                                                    |
| getMaxMembers()                                            | int                           | Bandens maksimale antal medlemmer.                                                    |
| getMaxRivals()                                             | int                           | Bandens maksimale antal rivaler.                                                      |
| getMemberName(UUID)                                        | String                        | Få navnet af en fra banden ved brug af medlemmets UUID.                               |
| getName()                                                  | String                        | Bandens navn.                                                                         |
| getPermission(String permission)                           | int                           | Få hvilken rank medlemmet skal have i banden for bruge denne permission.              |
| getSortedMembers()                                         | LinkedHashMap\<UUID, Integer) | Få medlemmerne sorteret efter rank.                                                   |
| getStat(String)                                            | int                           | Få bandens stat ud fra en string.                                                     |
| incrementMaxAllies()                                       | void                          | Øg bandens maksimale allierede med 1.                                                 |
| incrementMaxMembers()                                      | void                          | Øg bandens maksimale medlemmer med 1.                                                 |
| incrementMaxRivals()                                       | void                          | Øg bandens maksimale rivaler med 1.                                                   |
| isMember(UUID)                                             | boolean                       | Check om bestemt UUID er medlem af banden.                                            |
| isOwner(UUID)                                              | boolean                       | Check om bestemt UUID er ejer af banden.                                              |
| removeBank(long)                                           | long                          | Fjern penge fra bandens bank, og returner **getBank()**                               |
| removeMember(UUID)                                         | void                          | Fjerner et medlem fra banden.                                                         |
| setBank(long)                                              | void                          | Sæt bandens bank til **long**                                                         |
| setCustomVariable(String, Object, boolean)                 | void                          | Sæt en custom variabel for banden, og angiv om den skal save til filen med det samme. |
| sendMessageToAllMembers(String\[])                         | void                          | Send en besked til alle medlemmer.                                                    |
| sendMessageToAllMembers(String)                            | void                          | Send en besked til alle medlemmer.                                                    |
| <p>sendMessageToMembersExcept(Player, </p><p>String[])</p> | void                          | Send en besked til alle medlemmerne i banden på nær en.                               |
| <p>sendMessageToMembersExcept(Player, </p><p>String)</p>   | void                          | Send en besked til alle medlemmerne i banden på nær en.                               |
| setLevel(int)                                              | void                          | Sæt bandens level.                                                                    |
| setPermission(String, int)                                 | void                          | Sæt bandens permission rank til noget bestemt.                                        |
| setStat(String, int)                                       | void                          | Sæt en stat til **int**                                                               |
