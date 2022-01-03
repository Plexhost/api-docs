# Bande

![](../../.gitbook/assets/bande-banner.png)

## Beskrivelse <a href="#description" id="description"></a>

**Bande** er et enormt konfigurerbart plugin til Prison servere.\
Pluginet er lavet med "addons" i hovedet, og indeholder en utrolig nem måde for andre at udvikle deres version af plugin, som de gerne vil have det.

## Features

* Indbygget GUI system.
* API til at lave dine egne addons.
  * Levels
  * Settings
  * GUI
  * Shop
* Utælleligt mange custom events til at styre pluginet.

## Permissions

| **Command**   | **Alias** | **Permission** | **Beskrivelse**                              |
| ------------- | --------- | -------------- | -------------------------------------------- |
| /bande        | /b        | bande.use      | Tilgå bande menuen.                          |
| /bande reload | /b reload | bande.reload   | Reloader alle filerne (ikke selve banderne). |
| /bande info   | /b info   | bande.info     | Viser information om pluginet.               |
| /bande addons | /b addons | bande.addons   | Viser installerede addons.                   |

{% hint style="info" %}
Permissions **bande.admin** og **bande.\*** giver adgang til alt i pluginet.
{% endhint %}

## Dependencies

* [Vault](https://www.spigotmc.org/resources/vault.34315/)
* [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)

## Todo

* [ ] API Maven Repository
* [ ] Overskuelig og simpel placeholder system.
* [ ] MongoDB & MariaDB Support.
