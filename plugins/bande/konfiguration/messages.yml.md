# Messages.yml

{% hint style="info" %}
Alle beskeder bliver behandlet som en **List\<String>**, så du kan derfor lave flere linjer hvis du vil.
{% endhint %}

{% code title="messages.yml" %}
```yaml
prefix: "[bande]" # Skal være 1 linje.
no_bande: "Du har ingen bande."
player_only: "Denne kommando kan kun bruges af spillere."
console_only: "Denne kommando kan kun bruges af consolen."
no_permission: "Du har ikke adgang til denne kommando."
bande_not_found: "Der blev ikke fundet en bande med navnet {0}"
command_on_cooldown: "Du skal vente {0} før du kan bruge denne kommando igen."
error_occurred: "Der skete en fejl"
not_member_of_bande: "Du er ikke medlem af banden {0}"
no_access: "Du har ikke adgang til at gøre dette."
reload:
  starting: "%prefix% Starter reload af bande."
  success: "Bande er successfuldt blevet reloadet."
  error: "Der skete en fejl under reload af bande."
groups: # Skal være 1 linje.
  leader:
    title: Leder
    color: "&5"
  admin:
    title: Admin
    color: "&d"
  officer:
    title: Officer
    color: "&e"
  member:
    title: Medlem
    color: "&a"
  unknown:
    title: Ukendt
    color: "&7"
time: # Skal være 1 linje.
  day:
    singular: dag
    plural: dage
    abbreviation: d
  hour:
    singular: time
    plural: timer
    abbreviation: h
  minute:
    singular: minut
    plural: minutter
    abbreviation: m
  second:
    singular: sekund
    plural: sekunder
    abbreviation: s
  and: og
  since: siden
ally_chat:
  usage: 'Brug /allychat <besked>'
  message:
    - "[ALLYCHAT]"
    - "[{0}] {1}: {2}"
bande_chat:
  usage: 'Brug /bandechat <besked>'
  message:
    - "[BANDECHAT]"
    - "[{0}] {1}: {2}"
create_bande:
  not_enough_money: "En bande koster ${0} og du mangler ${1}"
  already_have_bande: "Du har allerede en bande: {0}"
  input_prompt:
    - "&7Skriv din kommende bandes navn i chatten."
    - "&7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "Du kan nu bruge chatten igen!"
    bande_exists: "Banden {0} findes allerede"
    name_too_short: "Navnet skal være mindst være {0} tegn"
    name_too_long: "Navnet må maksimalt været {0} tegn"
    only_alphabetical: "Navnet kan kun indeholde bogstaverne fra A til Z"
    banned_name: "Navnet kan ikke være: {0}"
    bande_created:
      - "Du har oprettet banden:"
      - "&a{0}"
delete_bande:
  player_deleted_bande: "{0} har slettet banden {1}"
  you_deleted_bande: "Du har slettet din bande {0}"
leave_bande:
  player_left_bande: "{0} har forladt banden"
  you_left_bande: "Du har forladt banden {0}"
player_invitations:
  invitation_not_available: "Denne invitation findes ikke mere."
  has_reached_max_members: "Banden {0} har ikke plads til flere medlemmer."
  you_joined_bande: "Du har joinet banden: {0}"
  player_joined_bande: "{0} har joinet banden."
bande_invitations:
  player_is_not_invited: "Spilleren {0} er ikke inviteret."
  remover_invitation_removed: "{0}'s invitation er blevet fjernet."
  invited_invitation_removed: "Din invitation fra banden {0} er blevet fjernet af {1}"
invite_member:
  input_prompt:
    - "&7Skriv spilleren i chatten."
    - "&7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "Du kan nu bruge chatten igen"
  player_is_not_found: "Spilleren {0} er ikke online"
  cant_invite_yourself: "Du kan ikke invitere dig selv"
  already_member_of_bande: "{0} er allerede medlem af din bande."
  already_invited: "{0} er allerede blevet inviteret."
  inviter_success: "Du har inviteret {0} til banden."
  invited_success: "Du er blevet inviteret til {1} af {0}"
deposit_money:
  input_prompt:
    - "&7Indtast beløber du ønsker at indsætte."
    - "&7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "Du kan nu bruge chatten igen!"
    only_numbers: "Du kan kun indsætte hele beløber"
    not_enough_money: "Du mangler ${0}"
    transaction_successful: "Du har indsat ${0} på din bandes konto, i har nu ${1}"
    player_transaction: "{0} har indsat ${1} på din bandes konto, i har nu ${1}"
rename_bande:
  input_prompt:
    - "&7Indtast dit ønskede bandenavn"
    - "&7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "Du kan nu bruge chatten igen!"
    not_enough_money: "Rename koster ${0} og banden mangler ${1}"
    bande_renamed:
      - "Din bande er blevet renamet fra {0} til {1}"
bande_members:
  cant_edit_yourself: "Du kan ikke ændre på dig selv."
  cant_edit_player: "Du kan ikke ændre på {0}"
edit_member:
  member_edited: "{0}'s rolle er blevet ændret til {1} af {2}"
  demoted_yourself: "Du har givet {0} Leder og er derfor blevet demoted til Admin"
kick_member:
  cant_kick_player: "Du kan ikke kicke {0}"
  you_kicked_player: "Du har kicket {0} fra banden"
  player_kicked_member: "{0} har kicket {1} fra banden."
  you_have_been_kicked: "Du er blevet kicket fra {0} af {1}"
add_ally:
  input_prompt:
    - "&7Indtast bandens navn."
    - "&7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "Du kan nu bruge chatten igen"
    ally_already_added: "Jeres bande har allerede spurgt {0} som allierede."
    bande_already_added: "Banden {0} har spurgt din bande som allierede, accepter den inden under invitationer"
    ally_added: "Du har spurgt banden {0} om allierede"
    bande_has_send_invitation: "Banden {0} har spurgt om allierede"
remove_ally:
  player_has_removed_ally: "{0} har fjernet banden {1} som allierede"
  you_have_remove_ally: "Du har fjernet banden {0} som allierede."
  has_removed_you_as_ally: "Banden {0} har fjernet jer som allierede."
accept_ally:
  bande_has_reached_max_allies: "Din bande har ikke plads til flere allierede."
  ally_has_reached_max_allies: "Banden {0} har ikke plads til flere allierede."
  has_accepted_ally: "Du har accepteret en alliance med banden {0}"
  has_become_ally_with: "Din bande er nu allierede med {0}"
  cant_add_your_own_bande: "Du kan ikke spørger din egen bande om allierede."
bande_shop:
  not_enough_money: "Din bande har ikke råd til dette."
  maximized_item: "I har opnået max i dette level."
  bought_item: "Du har købt {0} for ${1} til banden."
  player_has_bought_item: "{0} har købt {1} for ${1} til banden."
levelup:
  missing_requirements: "Din bande har ikke løst alle opgaverne."
  bande_levelup: "Din bande er steget i level {0}"
chat_format:
  no_gang: "{0}{1}{2}&8: &f{3}"
  has_gang:
    member: "&8[&a{0}&8][&a{1}&8]{2}{3}{4}&8: &f{5}"
    ally: "&8[&a{0}&8][&a{1}&8]{2}{3}{4}&8: &f{5}"
    rival: "&8[&c{0}&8][&c{1}&8]{2}{3}{4}&8: &f{5}"
    default: "&8[&7{0}&8][&7{1}&8]{2}{3}{4}&8: &f{5}"
gui: # Gui
  information:
    allies:
      ally: "&8 ● &a{0}"
      and_x_more: "&8 ● &7Og &a{0} &7flere."
      no_allies: "&8 ● &7I har ingen allierede."
    rivals:
      no_rivals: "&8 ● &7I har ingen rivaler."
      no_rivals_against:
      - "&8 ● &7I har ingen rivaler."
      - "&8   &7mod jer."
      rival: "&8 ● &c{0}"
      and_x_more: "&8 ● &7Og &c{0} &7flere."
    members:
      member: "&8 ● &8[&7{0}&8] &7{1}"
```
{% endcode %}
