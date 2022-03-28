# Messages

{% code title="messages.yml" %}
```yaml
no-permission: '&8[&cCeller&8] &7Du har ikke adgang til denne kommando.'
player-only-cmd: '&8[&cCeller&8] &7Denne kommando er player-only.'
errors:
  unknown: '&8[&cCeller&8] &7Der skete en fejl med fejlkoden: &c{0}'
  alphanumeric: '&8[&cCeller&8] &7{0} kan kun indeholde bogstaver og tal.'
  numeric: '&8[&cCeller&8] &7Indtast venligst et tal.'
  plugin-not-found: '&8[&cCeller&8] &7Pluginet &c{0} &7blev ikke fundet.'
  cell-not-found: '&8[&cCeller&8] &7Ingen celle fundet med navnet&8: &c{0}'
  group-not-found: '&8[&cCeller&8] &7Ingen gruppe fundet med navnet&8: &c{0}'
  cell-location-not-found: '&8[&cCeller&8] &7Ingen lokation fundet for cellen&8: &c{0}'
  group-location-not-found: '&8[&cCeller&8] &7Intet skilt fundet for gruppen&8: &c{0}'
  already-being-edited: '&8[&cCeller&8] &7Denne &c{0} &7er allerede igang med at blive ændret.'
  player-not-online: '&8[&cCeller&8] &7Spillere &c{0}&7 er ikke online.'
  player-not-found: '&8[&cCeller&8] &7Ingen spiller fundet med navnet&8: &c{0}'
  command-on-cooldown: '&8[&cCeller&8] &7Du kan bruge kommandoen igen om&8: &c{0}'
success:
  teleport-cell: '&8[&aCeller&8] &7Du blev teleporteret til cellen&8: &a{0}'
  teleport-group: '&8[&aCeller&8] &7Du blev teleporteret til ''ledige'' skilt for gruppen&8: &a{0}'
  created-group: '&8[&aCeller&8] &7Gruppen &a{0}&7 er blevet lavet.'
  group-deleted: '&8[&aCeller&8] &7Gruppen &a{0}&7 er blevet slettet.'
  cell-forcesold: '&8[&aCeller&8] &7Cellen &a{0}&7 er blevet solgt.'
keywords:
  a-cell-name: "Et celle-navn"
  a-cell: 'En celle'
  cell: 'Celle'
  a-group-name: "Et gruppe-navn"
  a-group: 'En gruppe'
  group: 'Gruppe'
unrent:
  expired: '&8[&cCeller&8] &7Din celle er udløbet.'
  sold: '&8[&cCeller&8] &7Du har solgt din celle.'
  forcesold: '&8[&cCeller&8] &7Din celle er blevet solgt.'
  deleted: '&8[&cCeller&8] &7Din celle er blevet slettet.'
sign:
  no-more: "&lOg ikke flere"
  more: "&lOg {0} flere"
info:
  rented:
    - '&8&m----------&7 &aCELLE &8&m----------'
    - '&aEjer: &7{0}'
    - '&aTid tilbage: &7{1}'
    - '&aCelle: &7{2}'
    - '&aBlok: &7{3}'
    - '&aMedlemmere: &7{4}'
    - '&8&m----------&7 &aCELLE &8&m----------'
  available: '&8[&aCeller&8] &7Denne celle er ledig.'
  find:
    found-none:
      - '&8[&cCeller&8] &c{0}&7 ejer og er ikke tilføjet til nogen celle.'
    found-cells:
      - '&8[&aCeller&8] &a{0}&7 ejer cellerne&8: &a{1}'
    found-added:
      - '&8[&aCeller&8] &a{0}&7 er tilføjet til cellerne&8: &a{1}'
    found-both:
      - '&8&m----------&7 &aMEDLEM &8&m----------'
      - '&aNavn: &7{0}'
      - '&aEjer: &7{1}'
      - '&aTilføjet: &7{2}'
      - '&8&m----------&7 &aMEDLEM &8&m----------'
help:
  admin:
    top: '&8&m----------&7 &aADMIN KOMMANDOER &8&m----------'
    bottom: ''
    cmds:
      reload:
        help: '&a/cea reload &8- &7For at reload pluginet.'
        hover:
          - '&a/cea reload'
          - '&7Reloader config.yml og messages.DA.yml'
      admin:
        help: '&a/cea admin &8- &7For at åbne admin panelet.'
        hover:
          - '&a/cea admin <celle>'
          - '&7Åbner admin panelet, gives der et'
          - '&7celle som argument åbnes admin panelet,'
          - '&7for den celle.'
      create:
        help: '&a/cea create <celle> &8- &7For at lave ny celle.'
        hover:
          - '&a/cea create <celle>'
          - '&7Laver en ny celle, du kan tilføje et'
          - '&72. argument, som er gruppen, som cellen,'
          - '&7skal tilføjes til.'
      delete:
        help: '&a/cea delete <celle> &8- &7For at slette en celle.'
        hover:
          - '&a/cea delete <celle>'
          - '&7Sletter en celle'
      edit:
        help: '&a/cea edit <celle> &8- &7Åbner celle panelet.'
        hover:
          - '&a/cea edit <celle>'
          - '&7Åbner celle panelet for en celle.'
      teleport:
        help: '&a/cea tp <celle> &8- &7Teleporter til celle.'
        hover:
          - '&a/cea tp <celle>'
          - '&7Teleportere til celle.'
      setlocation:
        help: '&a/cea setloc <celle> &8- &7Sætter teleport lokationen.'
        hover:
          - '&a/cea setloc <celle>'
          - '&7Sætter teleport lokationen.'
      setsign:
        help: '&a/cea setsign <celle> &8- &7Sætter cellens skilt.'
        hover:
          - '&a/cea setsign <celle>'
          - '&7Sætter cellens skilt.'
      find:
        help: '&a/cea find <spiller> &8- &7Finder data om en spiller.'
        hover:
          - '&a/cea find <spiller>'
          - '&7Finder data om en spiller.'
  normal:
    top: '&8&m----------&7 &aCELLE KOMMANDOER &8&m----------'
    bottom: ''
    cmds:
      add:
        help: '&a/ce add <spiller> &8- &7For at tilføje medlemmer til din celle.'
        hover:
          - '&a/ce add <spiller>'
          - '&7Tilføjer en spiller til en af dine celler,'
          - '&7har du flere, vil du blive bedt om at angive,'
          - '&7hvilken celle, spilleren skal tilføjes til.'
      remove:
        help: '&a/ce remove <spiller> &8- &7For at fjerne medlemmer fra din celle.'
        hover:
          - '&a/ce remove <spiller>'
          - '&7Fjerner en spiller fra din celle,'
          - '&7har du flere, vil du blive bedt om at angive,'
          - '&7hvilken celle, spilleren skal fjernes fra.'
      info:
        help: '&a/ce info <celle/spiller> &8- &7For at få info om en celle/spiller'
        hover:
          - '&a/ce info <celle/spiller>'
          - '&7For at få info om en celle/spiller'
commands:
  reload:
    starting: '&8[&aCeller&8] &7Starter reload af Cells pluginet.'
    error: '&8[&cCeller&8] &7Der skete en fejl under reloaden.'
    success: '&8[&aCeller&8] &7Cells pluginet blev succesfuldt reloadet.'
  create:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea create <celle>'
    cell-already-exists: '&8[&cCeller&8] &7Cellen &a{0} &7findes allerede.'
    group-already-exists: '&8[&cCeller&8] &7Gruppen &a{0} &7findes allerede.'
    no-we-selection: '&8[&cCeller&8] &7Du har ingen WorldEdit selektion.'
    only-cuboid-selections: '&8[&cCeller&8] &7Celle regionen skal være kasseformet.'
    region-same-world: '&8[&cCeller&8] &7Din selektion er i 2 forskellige verdener.'
    cell-created: '&8[&aCeller&8] &7Cellen &a{0}&7 er blevet lavet, i gruppen &a{1}'
  delete:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea delete <celle>'
    cell-deleted: '&8[&aCeller&8] &7Cellen &a{0}&7 er blevet slettet.'
  edit:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea edit <celle>'
  teleport:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea tp <celle>'
  setlocation:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea setloc <celle>'
    location-changed: '&8[&aCeller&8] &7Du har sat lokationen for cellen&8: &a{0}'
  setsign:
    usage: '&8[&aCeller&8] &7Brug&8: &a/cea setsign <celle>'
    not-a-sign: '&8[&cCeller&8] &7Kig venligst på et skilt.'
    sign-changed: '&8[&aCeller&8] &7Du har sat skiltet for cellen&8: &a{0}'


  add:
    usage: '&8[&aCeller&8] &7Brug&8: &a/ce add <spiller>'
    no-cells: '&8[&cCeller&8] &7Du ejer ingen celle.'
    choose-cell:
      - '&8[&aCeller&8] &7Du ejer flere celler.'
      - '&8[&aCeller&8] &7Brug&8: &a/ce add <spiller> <celle>'
    max-members-reached: '&8[&cCeller&8] &7Der er ikke plads til flere medlemmer i cellen.'
    already-member: '&8[&cCeller&8] &c{0}&7 er allerede tilføjet til cellen.'
    member-added: '&8[&aCeller&8] &7Du har tilføjet &a{0}&7 til cellen.'
  remove:
    usage: '&8[&aCeller&8] &7Brug&8: &a/ce remove <spiller>'
    no-cells: '&8[&cCeller&8] &7Du ejer ingen celle.'
    choose-cell:
      - '&8[&aCeller&8] &7Du ejer flere celler.'
      - '&8[&aCeller&8] &7Brug&8: &a/ce remove <spiller> <celle>'
    not-member: '&8[&cCeller&8] &c{0}&7 er ikke tilføjet til cellen.'
    member-removed: '&8[&aCeller&8] &7Du har fjernet &a{0}&7 fra cellen.'
  info:
    no-cells: '&8[&cCeller&8] &7Du ejer ingen celle.'
    other-multiple-cells:
      - '&8[&aCeller&8] &a{0}&7 ejer cellerne&8: &a{1}'
      - '&8[&aCeller&8] &7Brug&8: &a/ce info <celle>'
    own-multiple-cells:
      - '&8[&aCeller&8] &7Du ejer cellerne&8: &a{0}'
      - '&8[&aCeller&8] &7Brug&8: &a/ce info <celle>'
events:
  add-duration:
    cant-afford: '&8[&cCeller&8] &7Du har ikke råd til at tilføje dage.'
    max-duration: '&8[&cCeller&8] &7Du kan ikke tilføje mere end &c{0} dage.'
    success: '&8[&aCeller&8] &7Du har tilføjet &a1 dag&7 for &a${0}'
  buy-cell:
    cant-afford: '&8[&cCeller&8] &7Du har ikke råd til denne celle.'
    no-permission: '&8[&cCeller&8] &7Du har ikke adgang til at leje denne celle.'
    max-cells: '&8[&cCeller&8] &7Du kan ikke leje flere celler.'
    success: '&8[&aCeller&8] &7Du har købt cellen &a{0} for &a${1}'
    cooldown: '&8[&cCeller&8] &7Du kan først købe en ny celle om&8: &c{0}'
  cellgroup-sign-placed:
    success: "&8[&aCeller&8] &7Du har sat 'ledige' skilt for gruppen&8 &a{0}"
    error: '&8[&cCeller&8] &7Der skete en fejl.'
```
{% endcode %}
