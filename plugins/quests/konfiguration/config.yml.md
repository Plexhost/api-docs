# Config.yml

{% code title="config.yml" %}
```yaml
license: Your license key
save-time: 5 # Hvor ofte serveren gemmer data.
concurrentQuests: 3 # Hvor mange quests en spiller maksimalt kan have.
storage: # Hvordan skal dataen gemmes.
  type: YAML # YAML or MongoDB
  username: username
  password: password
  host: host
  port: 27017
  srv: false
```
{% endcode %}
