# Quests (missioner)

{% hint style="info" %}
Alle quests skal oprettes i mappen \`/quests\`

Det er muligt at lave sub-folders derinde for at organisere sig.
{% endhint %}

## Quest Typer:

* `BLOCK_BREAK`
  *   Smadre bestemt blok et bestemt antal gange&#x20;

      ```yaml
      type: BLOCK_BREAK
      variable: STONE # Material
      required: 128 # Antal
      ```
* `BLOCK_PLACE`
* `CHAT`
  *   Skriv bestemt besked i chatten

      ```yaml
      type: CHAT
      variable: Quests er et Awesome Plugin! # Besked
      ```
* `CONSUME`
* `PLAYER_FISH`
* `NPC_CLICK` _(kræver Citizens)_
  *   Find / Klik på en NPC

      ```yaml
      type: NPC_CLICK
      variable: 59 # id'et på NPC'en
      ```
  *   Aflever items til NPC

      ```yaml
      type: NPC_CLICK
      variable: 59 # id'et på NPC'en
      extra-variable: ROTTEN_FLESH # Material
      required: 64 # Antal
      ```
* `REGION_ENTER` _(kræver WorldGuard)_
  *   _Gå ind i bestemt region:_

      ```yaml
      type: REGION_ENTER
      variable: mines # The Region
      ```
* Opret en ticket for at få tilføjet flere events!

{% code title="quests/blockbreak.yml" lineNumbers="true" %}
```yaml
id: BlockPlaceExample
type: BLOCK_PLACE
variable: GLASS
required: 32 # default til 1
reward:
  commands:
    - "eco give {player} 560"
gui:
  title: "Placer - Example"
  material: GLASS
  description: "Placer 32x Glass"
  rewards:
    - " &8  - &a$560"
```
{% endcode %}

