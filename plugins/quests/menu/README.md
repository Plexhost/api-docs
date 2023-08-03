# Menu

{% hint style="info" %}
Alle quest menuer skal oprettes i mappen \`/menus\`

Det er muligt at lave sub-folders derinde for at organisere sig.
{% endhint %}

Alle quest menuer består af 3 dele:\
\- Indstillinger\
\* `max-activated-quests` afgør hvor mange quests fra denne menu som man kan have aktiveret på en gang.\
\* `permission` er den permission som en spiller skal have for at kunne åbne menuen.\
\
\- Gui ([læs mere om det her](gui.md))\
\* `quests` her skal du skrive id'et på dine quests og det slot som du vil have de skal fremgå i menuen.\
\
\- Template:\
\* Du kan som udgangspunkt nøjes med at konfigurere `default-template.yml` for hvordan quest items skal fremgå i menuen - dog kan du også gøre dette på et individuelt plan i hver quest menu som vil override default template.

&#x20;

### **Eksempel på en quest menu.**

{% code title="menus/default.yml" lineNumbers="true" %}
```yaml
max-activited-quests: 3 # The maximum amount of quests a player can have activated at once from this menu.
permission: "quests.menu.default" # The permission required to open this menu.

gui:
  title: "Example Quests"
  rows: 1
  items:
    glass:
      material: STAINED_GLASS_PANE
      data: 15
      slots: [ 0, 1, 2, 3, 4, 5, 6, 7, 8]
  quests:
    BlockBreakExample: 2
    BlockPlaceExample: 3
    ChatExample: 4
    ConsumeExample: 5
    FindRegionExample: 6

template:
  completed:
    material: EMERALD_BLOCK
    title: "&a&lKlaret!"
    lore:
      - "&7Du har klaret denne mission."
  cooldown:
    material: COAL_BLOCK
    title: "&e&l{title}"
    lore:
      - "&7Du har klaret denne mission."
      - "&7Kom igen om&8: &f{cooldown}"
  activated:
    material: STONE # Can be overridden in the individual Mission Files.
    title: "&b&l{title}"
    enchanted: true
    lore:
      - "&8&l» &7Opgave&8: &a{quest}"
      - "&8&l» &7Belønninger&8:"
      - "{rewards}"
      - ""
      - "&8&l» &7Fremskridt&8: &a{progress}/{required}"
      - ""
      - "&aDenne mission er aktiveret."
      - "&8&l » &7Klik for at afbryde den."
  default:
    material: STONE # Can be overridden in the individual Mission Files.
    title: "&b&l{title}"
    lore:
      - "&8&l» &7Opgave&8: &a{quest}"
      - "&8&l» &7Belønninger&8:"
      - "{rewards}"
      - ""
      - "&8&l» &7Klik for at starte missionen."
```
{% endcode %}
