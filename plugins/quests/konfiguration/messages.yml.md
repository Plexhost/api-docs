# Messages.yml

{% hint style="info" %}
Alle beskeder bliver behandlet som en **List\<String>**, så du kan derfor lave flere linjer hvis du vil.
{% endhint %}

{% code title="messages.yml" %}
```yaml
user-not-loaded: "&8&l┃ &c&lQuests &8&l┃ &cDer skete en fejl. Data er ikke hentet endnu."
no-permission: "&8&l┃ &c&lQuests &8&l┃ &cDu har ikke adgang til denne kommando."
player-only: "&8&l┃ &c&lQuests &8&l┃ &cDenne kommando er player-only."
no-menu-access: "&8&l┃ &c&lQuests &8&l┃ &7Du har ikke adgang til denne menu."
menu-not-found: "&8&l┃ &c&lQuests &8&l┃ &cMenuen &f{0} &cblev ikke fundet."
commands:
  reload:
    start: "&8&l┃ &a&lQuests &8&l┃ &aStarter reload af Quests."
    error: "&8&l┃ &c&lQuests &8&l┃ &cDer skete en fejl under reload."
    success: "&8&l┃ &2&lQuests &8&l┃ &2Reload var succesfuld."
  help:
    - "&8&m===================================================="
    - "  &2&lQuests"
    - ""
    - "  &8&l» &f/quests help &8- &7Viser denne besked"
    - "  &8&l» &f/quests open &7[MENU] &8- &7Åbner en quest menu."
    - "  &8&l» &f/quests reload &8- &7Reload konfigurationen."
    - "  &8&l» &f/quests show &7[PLAYER] [MENU] &8- &7Åbner menu for spiller."
    - ""
    - "&8&m===================================================="
  show:
    usage: "&8&l┃ &c&lQuests &8&l┃ &7Korrekt brug&8: &f/quests show [PLAYER] [MENU]"
    player-not-found: "&8&l┃ &c&lQuests &8&l┃ &cSpilleren &f{0} &cblev ikke fundet."
mission:
  started: "&8&l┃ &a&lQuests &8&l┃ &7Du har startet questen &a{0}"
  cancelled: "&8&l┃ &c&lQuests &8&l┃ &7Du har annulleret questen &c{0}"
  concurrent-error: "&8&l┃ &c&lQuests &8&l┃ &7Du kan kun have &c{0} quests &7aktiveret på en gang."
  concurrent-menu-error: "&8&l┃ &c&lQuests &8&l┃ &7Du kan kun have &c{0} quests &7aktiveret fra denne menu."
  complete:
    message: "&8&l┃ &a&lQuests &8&l┃ &7Du har klaret questen &a{0}"
    title: "&a&lQuest Klaret!"
    subtitle: "&7Du har klaret en quest!"
```
{% endcode %}
