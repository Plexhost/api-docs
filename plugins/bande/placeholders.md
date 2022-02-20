---
description: Disse er PlaceholderAPI placeholders til at vise information.
---

# Placeholders



| Placeholder                                                                               | Beskrivelse                                                                                                                               | Eksempel                        |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- |
| `%bande_config_<key>%`                                                                    | Vis config values.                                                                                                                        | `%bande_config_bande_price%`    |
| `%bande_player_invitations%`                                                              | Viser antallet af ens bande invitationer.                                                                                                 | -                               |
| `%bande_name%`                                                                            | Viser din bandes navn, eller `placeholders.no_bande` hvis du ikke er medlem af en.                                                        |  -                              |
| <p><code>%bande_id%</code><br><code>%bande_bank%</code><br><code>%bande_level%</code></p> | <p>Viser din bandes id.<br>Viser din bandes bank.<br>Viser din bandes level.</p>                                                          | -                               |
| `%bande_stat_<stat>%`                                                                     | Viser din bandes stat.                                                                                                                    | `%bande_stat_kills%`            |
| `%bande_permission_<type>%`                                                               | Viser den rank man skal være for at bruge denne permission.                                                                               | `%bande_permission_rename%`     |
| `%bande_has_bought_<id>%`                                                                 | <p>Viser om man har købt en ting i shoppen.<br>Returner henholdsvis <code>placeholders.true</code> og <code>placeholders.false</code></p> | `%bande_has_bought_hungerbuff%` |
|                                                                                           |                                                                                                                                           |                                 |

Du kan også bruge `%bande_get_bande_name:<navn>%` i sammenhæng med de andre values. \
Så tager placeholderen udgangspunkt i den bande.\
\
Eksempel: `%bande_get_bande_name:<navn>_stat_kills%`
