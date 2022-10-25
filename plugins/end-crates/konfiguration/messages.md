# Messages

{% code title="messages.yml" %}
```yaml
preview:
  title: "&2&lEndCrate"
  prize-lore:
    - "&7Chance&8: &a{0}%"
reward-hologram:
  title: "&2&l&nEnd Crate"
commands:
  help:
    - '&8[&aEndCrates&8] &7Commands&8:'
    - '&8 » &a/endcrate givecrate <crate>'
    - '&8 » &a/endcrate givekey <player> <crate> [<antal>]'
    - '&8 » &a/endcrate reload'
  givekey:
    usage: "&8[&aEndCrates&8] &7Korrekt brug&8: &f/endcrate givekey <player> <crate> [<antal>]"
    success: "&8[&aEndCrates&8] &7Du har givet &f{2}x {1} &7til &a{0}"
  givecrate:
    usage: "&8[&aEndCrates&8] &7Korrekt brug&8: &f/endcrate givecrate <crate>"
    success:
      - "&8[&aEndCrates&8] &7Du har givet dig selv en &f{0} &7crate."
      - "&8[&aEndCrates&8] &7Placer den for at man kan åbne den."
  reload:
    start: "&8[&aEndCrates&8] &7Reloader pluginet"
    success: "&8[&aEndCrates&8] &aReload gennemført."
    failed: "&8[&cEndCrates&8] &cReload fejlede. Tjek venligst konsolen."
events:
  crate-place:
    crate-no-exist: "&8[&cEndCrates&8] &cCraten &f{0} &cfindes ikke længere."
    crate-placed: "&8[&aEndCrates&8] &aDu har placeret en &f{0} &acrate!"
  crate-break:
    sneak: "&8[&cEndCrates&8] &7Du skal sneake for at fjerne craten."
    crate-removed: "&8[&aEndCrates&8] &aDu har fjernet en crate!"

player-only: "&8[&cEndCrates&8] &cDu skal være en spiller for at bruge denne kommando."
no-permission: "&8[&cEndCrates&8] &cDu har ikke adgang til denne kommando."
crate-not-found: "&8[&cEndCrates&8] &cCraten &f{0} &cblev ikke fundet."
invalid-amount: "&8[&cEndCrates&8] &cUgyldigt antal&8: &f{0}"
player-not-found: "&8[&cEndCrates&8] &cSpilleren &f{0} &cblev ikke fundet."
no-keys: "&8[&cEndCrates&8] &cDu har ikke nogen nøgler til denne crate."
crate-already-opened: "&8[&cEndCrates&8] &cDenne crate er allerede igang med at blive åbnet."
```
{% endcode %}
