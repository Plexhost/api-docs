# Config.yml

{% code title="config.yml" %}
```yaml
# Prisen for at oprette en bande, sæt til 0 for gratis.
bande_price: 2500
rename_price: 10000
debug: false
bande_minimum_length: 3
bande_maximum_length: 12

default_max_members: 3
default_max_allies: 1
default_max_rivals: 1

# Tid der skal gå mellem at folk "søger" efter bander med /bande <navn> kommandoen - behold over 3 for at undgå lag.
command_cooldown: 3

# Hvor mange minutter der går mellem alle bander bliver gemt.
# Vigtige data bliver gemt med det samme.
save_minutes: 10

# Hvor mange minutter der går mellem hver gang leaderboardsne opdatere.
leaderboard_minutes: 15

no_bande: "Ingen"

# Bander kan ikke hedde disse navne.
# Skal skrives med lowerCase (små bogstaver)
banned_names:
  - neger

# Om pluginet skal styre chat, eller du selv vil implementere noget.
handle_chat: true
```
{% endcode %}
