# Config

{% code title="config.yml" %}
```yaml
# License Key
license: Your License Key

# Debug mode?
debug: false

# Standard prisen, for alle nye celler, hvis prisen ikke er angivet.
defaultPrice: 300

# Standard maximum antal af dage, som man kan leje en celle i. Brug -1 for uendelig.
defaultMaxLength: 10

# Standard max medlemmer
defaultMaxMembers: 5

# Standard om ens celles blocks bliver sat til AIR, når du unrenter den.
defaultResetOnUnrent: false

# Om du modtager resterende dage i penge, når du sælger cellen.
refund: false

# Om der skal være cooldown på når man vil købe ny celle.
cooldown:
  enabled: false
  length: 3600 # Længden af cooldown

# Hvilket design som celle skilte har, når vdu bruger placeholderen %timeLeft%
# Tegnet '||' viser hvordan det vil se ud med forskellige længder af tid tilbage.
# Designs:
#  > 1: 2d19t21m || 4t21m
#  > 2: 7 dage || 5 timer || 21 minutter
timeLeftDesign: 2

# Skilt design
sign:
  rented:
    - '&c&lSOLGT'
    - '&c%cell%'
    - '&c%owner%'
    - '&c%timeleft%'
  available:
    - '&3&lTIL SALG'
    - '&b%cell%'
    - '&b$%price%'
    - '&b1 dag'
  removed:
    - ''
    - '&cCelle fjernet'
    - ''
    - ''
#
locale:
  days:
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
```
{% endcode %}
