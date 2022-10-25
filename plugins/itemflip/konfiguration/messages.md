# Messages

{% code title="messages.yml" %}
```yaml
errors:
  no-permission: "&8[&4ItemFlip&8] &7Du har ikke adgang til dette."
  error-occurred: "&8[&4ItemFlip&8] &7Der skete en fejl. Prøv venligst igen!"
  not-loaded: "&8[&4ItemFlip&8] &7Pluginet er ikke loadet færdigt endnu. Vent venligst!"
  player-only: "&8[&4ItemFlip&8] &7Du skal være en spiller for at kunne bruge denne kommando!"
  player-not-found: "&8[&4ItemFlip&8] &7Spilleren &f{0} &7er ikke online."
  invalid-number: "&8[&4ItemFlip&8] &7Antallet &f{0} &7er ikke et tal."
bets:
  accept-error: "&8[&4ItemFlip&8] &7Modbuddet er blevet slettet. Vælg et andet."
  deny-bet:
    deleted-error: "&8[&4ItemFlip&8] &7Modbuddet er allerede blevet slettet."
    bet-got-denied: "&8[&cItemFlip&8] &c{0} &7har afvist dit modbud."
    you-denied-bet: "&8[&cItemFlip&8] &7Du har afvist &c{0}'s &7modbud."
  delete-bet:
    flip-deleted: "&8[&4ItemFlip&8] &7Flippet er allerede slettet og du har fået dine items igen."
    bet-deleted: "&8[&4ItemFlip&8] &7Dit modbud er blevet slettet."
    already-deleted: "&8[&4ItemFlip&8] &7Dette bud er allerede blevet slettet."
  create-bet:
    created: "&8[&aItemFlip&8] &7Du har nu oprettet et nyt modbud til &f{0}"
    no-items: "&8[&4ItemFlip&8] &7Du skal have mindst 1 item i dit modbud!"
    received-bet: "&8[&aItemFlip&8] &a{0} &7har oprettet et modbud på dit flip!"
    already-created: "&8[&aItemFlip&8] &7Du har allerede et modbud på dette flip!"
    invalid-items:
      start: "&8[&4ItemFlip&8] &7Du kan ikke oprette modbud med&8:"
      each-item: "&8- &c{0}"
flips:
  create-flip:
    created: "&8[&aItemFlip&8] &7Du har nu oprettet et nyt flip!"
    no-items: "&8[&4ItemFlip&8] &7Du skal have mindst 1 item i dit flip!"
    no-flip-tokens: "&8[&4ItemFlip&8] &7Du har ingen flip tokens."
    invalid-items:
      start: "&8[&4ItemFlip&8] &7Du kan ikke oprette flip med&8:"
      each-item: "&8- &c{0}"
  deletex  -flip: "&8[&aItemFlip&8] &7Du har slettet dit flip. Dine items kan claimes i menuen."
  already-deleted: "&8[&4ItemFlip&8] &7Dette flip er blevet slettet eller taget."
results:
  error-flip: "&8[&4ItemFlip&8] &7Der skete en fejl med at load flippet. Prøv venligst igen!"
  error-bet: "&8[&4ItemFlip&8] &7Der skete en fejl med at load modbuddet. Prøv venligst igen!"
spin:
  win: "&8[&aItemFlip&8] &7Du har vundet et flip over &a{0}"
  loss: "&8[&cItemFlip&8] &7Du har tabt et flip til &c{0}"
tokens:
  success: "&8[&aItemFlip&8] &7Du har købt &f{0} flip tokens &7for &d1 diamond."
  no-item: "&8[&4ItemFlip&8] &7Du har ikke nok diamanter."
commands:
  give:
    usage: "&8[&4ItemFlip&8] &7Korrekt brug&8: &f/itemflip give <spiller> <antal>"
    tokens-given: "&8[&2ItemFlip&8] &7Du har givet &f{0} &7{1} &7flip tokens."
    tokens-received: "&8[&2ItemFlip&8] &7Du har modtaget &f{0} &7flip tokens."
  reload:
    start: "&8[&aItemFlip&8] &7Reloader pluginet..."
    error: "&8[&4ItemFlip&8] &7Der skete en fejl med at reload pluginet. Prøv venligst igen!"
    success: "&8[&aItemFlip&8] &7Reload er gennemført."
```
{% endcode %}
