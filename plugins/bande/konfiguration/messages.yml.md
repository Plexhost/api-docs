# Messages.yml

{% hint style="info" %}
Alle beskeder bliver behandlet som en **List\<String>**, så du kan derfor lave flere linjer hvis du vil.
{% endhint %}

{% code title="messages.yml" %}
```yaml
prefix: "&8&l┃ &b&lBande &8&l┃" # Skal være 1 linje.
no_bande: "&8&l┃ &c&lBande &8&l┃ &7Du er ikke medlem af nogen bande.."
player_only: "&8&l┃ &c&lBande &8&l┃ &7Denne kommando kan kun bruges af spillere."
console_only: "&8&l┃ &c&lBande &8&l┃ &7Denne kommando kan kun bruges af consolen."
no_permission: "&8&l┃ &c&lBande &8&l┃ &7Du har ikke adgang til denne kommando."
bande_not_found: "&8&l┃ &c&lBande &8&l┃ &7Der blev ikke fundet en bande med navnet &c{0}"
command_on_cooldown: "&8&l┃ &c&lBande &8&l┃ &7Du skal vente &c{0} &7før du kan bruge denne kommando igen."
error_occurred: "&8&l┃ &c&lBande &8&l┃ &cDer skete en fejl, kontakt en administrator."
not_member_of_bande: "&8&l┃ &c&lBande &8&l┃ &7Du er ikke medlem af banden &c{0}"
no_access: "&8&l┃ &c&lBande &8&l┃ &7Du har ikke adgang til at gøre dette."
reload:
  starting: "&8&l┃ &b&lBande &8&l┃ &7Starter reload af bande."
  success: "&8&l┃ &a&lBande &8&l┃ &aBande er successfuldt blevet reloadet."
  error: "&8&l┃ &c&lBande &8&l┃ &cDer skete en fejl under reload af bande."
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
  not_enough_money: "&8&l┃ &c&lBande &8&l┃ &7En bande koster &c${0} &7og du mangler &c${1}"
  already_have_bande: "&8&l┃ &c&lBande &8&l┃ &7Du er allerede medlem af banden &c{0}"
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Skriv din kommende bandes navn i chatten."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen!"
    bande_exists: "&8&l┃ &c&lBande &8&l┃ &7Der findes allerede en bande med dette navn."
    name_too_short: "&8&l┃ &c&lBande &8&l┃ &7Bandens navn skal mindst indeholde &c{0} tegn."
    name_too_long: "&8&l┃ &c&lBande &8&l┃ &7Bandens navn kan højst indeholde &c{0} tegn."
    only_alphabetical: "&8&l┃ &c&lBande &8&l┃ &7Navnet kan kun indeholde bogstaverne fra &cA &7til &cZ."
    banned_name: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke oprette en bande med dette navn."
    bande_created:
      - "&8&l┃ &b&lBande &8&l┃ &7Du har oprettet banden &b{0}"
delete_bande:
  player_deleted_bande: "&8&l┃ &c&lBande &8&l┃ &c{0} &7har slettet banden &c{1}"
  you_deleted_bande: "&8&l┃ &b&lBande &8&l┃ &7Du har slettet din bande &b{0}"
leave_bande:
  player_left_bande: "&8&l┃ &c&lBande &8&l┃ &c{0} &7har forladt din bande."
  you_left_bande: "&8&l┃ &b&lBande &8&l┃ &7Du har forladt banden &b{0}"
player_invitations:
  invitation_not_available: "&8&l┃ &c&lBande &8&l┃ &7Denne invitation findes ikke mere."
  has_reached_max_members: "&8&l┃ &c&lBande &8&l┃ &7Banden &c{0} &7har ikke plads til flere medlemmer."
  you_joined_bande: "&8&l┃ &b&lBande &8&l┃ &7Du har joinet banden &b{0}"
  player_joined_bande: "&8&l┃ &b&lBande &8&l┃ &b{0} &7har joinet banden."
bande_invitations:
  player_is_not_invited: "&8&l┃ &c&lBande &8&l┃ &7Spilleren &c{0} &7er ikke inviteret til banden."
  remover_invitation_removed: "&8&l┃ &c&lBande &8&l┃ &c{0}'s &7invitation er blevet fjernet."
  invited_invitation_removed: "&8&l┃ &b&lBande &8&l┃ &7Din invitation fra banden &c{0} &7er blevet fjernet af &c{1}"
invite_member:
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Skriv navnet på spilleren du vil invitere."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen!"
  player_is_not_found: "&8&l┃ &c&lBande &8&l┃ &7Spilleren &c{0} &7er ikke online."
  cant_invite_yourself: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke invitere dig selv til banden."
  already_member_of_bande: "&8&l┃ &c&lBande &8&l┃ &c{0} &7er allerede medlem af din bande."
  already_invited: "&8&l┃ &c&lBande &8&l┃ &c{0} &7er allerede blevet inviteret."
  inviter_success: "&8&l┃ &b&lBande &8&l┃ &7Du har inviteret &b{0} &7til banden."
  invited_success: "&8&l┃ &b&lBande &8&l┃ &7Du er blevet inviteret til &b{1} &7af &b{0}"
deposit_money:
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Indtast beløber du ønsker at indsætte."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen!"
    only_numbers: "&8&l┃ &c&lBande &8&l┃ &cDu kan kun indsætte hele beløber."
    not_enough_money: "&8&l┃ &c&lBande &8&l┃ &7Du mangler &c${0} &7for at indsætte dette beløb."
    transaction_successful: "&8&l┃ &b&lBande &8&l┃ &7Du har indsat &b${0} &7på din bandes konto, i har nu &b${1}"
    player_transaction: "&8&l┃ &b&lBande &8&l┃ &b{0} &7har indsat &b${1} &7på din bandes konto, i har nu &b${2}"
rename_bande:
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Indtast dit ønskede bandenavn."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen!"
    not_enough_money: "&8&l┃ &c&lBande &8&l┃ &7Det koster &b${0} &7at rename, og banden mangler &b${1}"
    bande_renamed:
      - "&8&l┃ &b&lBande &8&l┃ &7Din bande er blevet renamet fra &b{0} &7til &b{1}"
bande_members:
  cant_edit_yourself: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke ændre på dig selv."
  cant_edit_player: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke ændre på &c{0}."
edit_member:
  member_edited: "&8&l┃ &b&lBande &8&l┃ &b{0}'s &7rolle er blevet ændret til &b{1} &7af &b{2}"
  demoted_yourself: "&8&l┃ &b&lBande &8&l┃ &7Du har givet &b{0} &7Leder og er derfor blevet demoted til Admin."
kick_member:
  cant_kick_player: "&8&l┃ &c&lBande &8&l┃ &7Du har ikke adgang til at ikke kicke &b{0}."
  you_kicked_player: "&8&l┃ &b&lBande &8&l┃ &7Du har kicket &b{0} &7fra banden."
  player_kicked_member: "&8&l┃ &b&lBande &8&l┃ &b{0} &7har kicket &b{1} &7fra banden."
  you_have_been_kicked: "&8&l┃ &c&lBande &8&l┃ &7Du er blevet kicket fra &c{0} &7af &c{1}"
add_ally:
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Skriv navnet på banden du vil blive allierede med."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen"
    ally_already_added: "&8&l┃ &b&lBande &8&l┃ &7Du har spurgt &b{0} &7om allierede."
    bande_already_added: "&8&l┃ &b&lBande &8&l┃ &7Banden &b{0} &7har spurgt din bande som allierede, accepter den inden under invitationer."
    ally_added: "&8&l┃ &b&lBande &8&l┃ &7Du har spurgt banden &b{0} &7om allierede."
    bande_has_send_invitation: "&8&l┃ &b&lBande &8&l┃ &7Banden &b{0} &7har spurgt din bande om allierede."
remove_ally:
  player_has_removed_ally: "&8&l┃ &b&lBande &8&l┃ &b{0} &7har fjernet banden &b{1} &7som allierede"
  you_have_remove_ally: "&8&l┃ &b&lBande &8&l┃ &7Du har fjernet banden &b{0} &7som allierede."
  has_removed_you_as_ally: "&8&l┃ &c&lBande &8&l┃ &7Banden &c{0} &7har fjernet jer som allierede."
accept_ally:
  bande_has_reached_max_allies: "&8&l┃ &c&lBande &8&l┃ &7Din bande har ikke plads til flere allierede."
  ally_has_reached_max_allies: "&8&l┃ &c&lBande &8&l┃ &7Banden &c{0} &7har ikke plads til flere allierede."
  has_accepted_ally: "&8&l┃ &b&lBande &8&l┃ &7Du har startet en alliance med banden &b{0}"
  has_become_ally_with: "&8&l┃ &b&lBande &8&l┃ &7Din bande er nu allierede med &b{0}"
  cant_add_your_own_bande: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke spørger din egen bande om allierede."

add_rival:
  input_prompt:
    - "&8&l┃ &b&lBande &8&l┃ &7Skriv navnet på banden du vil blive rivaler med."
    - "&8&l┃ &b&lBande &8&l┃ &7Du kan skrive &b'!cancel'&7 for at annullere."
  response:
    cancel: "&8&l┃ &b&lBande &8&l┃ &7Du kan nu bruge chatten igen."
    already_rival: "&8&l┃ &c&lBande &8&l┃ &7Din bande er allerede rivaler med &c{0}"
    you_have_rival_added: "&8&l┃ &b&lBande &8&l┃ &7Du har tilføjet banden &b{0} &7som rivaler."
    player_have_rival_added: "&8&l┃ &b&lBande &8&l┃ &b{0} har tilføjet banden &b{1} &7som rival."
    cant_rival_your_own_bande: "&8&l┃ &c&lBande &8&l┃ &7Du kan ikke gøre din egen bande til rival."
    reached_max_rivals: "&8&l┃ &c&lBande &8&l┃ &7Din bande har ikke plads til flere rivaler."
remove_rival:
  player_has_removed_rival: "&8&l┃ &b&lBande &8&l┃ &c{0} &7har fjernet banden &c{1} &7som rival."
  you_have_remove_rival: "&8&l┃ &b&lBande &8&l┃ &7Du har fjernet banden &b{0} &7som rival."
bande_shop:
  not_enough_money: "&8&l┃ &c&lBande &8&l┃ &7Din bande har ikke råd til dette."
  maximized_item: "&8&l┃ &c&lBande &8&l┃ &cDin bande har opnået max i dette level."
  bought_item: "&8&l┃ &b&lBande &8&l┃ &7Du har købt &b{0} &7for &b${1} &7til banden."
  player_has_bought_item: "&8&l┃ &b&lBande &8&l┃ &b{0} &7har købt &b{1} &7for &b${2} &7til banden."
levelup:
  missing_requirements: "&8&l┃ &c&lBande &8&l┃ &7Din bande har ikke løst alle opgaverne."
  bande_levelup: "&8&l┃ &a&lBande &8&l┃ &7Din bande er steget i &alevel &2{0}"
  max_level: "&8&l┃ &c&lBande &8&l┃ &7Din bande et i max level."
chat_format:
  no_gang: "{0}{1}{2}&8: &f{3}"
  in_gang:
    member: "&8[&a{0}{1}&8][&a{2}&8]{3}{4}{5}&8: &f{6}"
    ally: "&8[&a{0}{1}&8][&a{2}&8]{3}{4}{5}&8: &f{6}"
    rival: "&8[&c{0}{1}&8][&c{2}&8]{3}{4}{5}&8: &f{6}"
    default: "&8[&7{0}{1}&8][&7{2}&8]{3}{4}{5}&8: &f%2$s"
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
  information_other:
    allies:
      ally: "&8 ● &a{0}"
      and_x_more: "&8 ● &7Og &a{0} &7flere."
      no_allies: "&8 ● &7Banden har ingen allierede."
    rivals:
      no_rivals: "&8 ● &7Banden har ingen rivaler."
      no_rivals_against:
        - "&8 ● &7Banden har ingen."
        - "&8   &7rivaler mod sig."
      rival: "&8 ● &c{0}"
      and_x_more: "&8 ● &7Og &c{0} &7flere."
    members:
      member: "&8 ● &8[&7{0}&8] &7{1}"
```
{% endcode %}
