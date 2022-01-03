# Create Addon

### Step 1 - Create Project

Start et almindeligt Java Projekt, som du ville gøre når du ville lave et plugin.

### Step 2 - Import with Maven

For at importere **Bande**, skal du blot tilføje denne kode til din **pom.xml.**

Erstat **{PATH}** med den absolutte sti til **Bande.jar** filen. Eksempel:

```
E:/IdeaProjects/Plexhost/Bande/target/Bande.jar
```

{% code title="pom.xml" %}
```xml
    <dependencies>
        <dependency>
            <groupId>dk.plexhost.bande</groupId>
            <artifactId>Bande</artifactId>
            <version>1.0</version>
            <systemPath>{PATH}</systemPath>
            <scope>system</scope>
        </dependency>
    </dependencies>
```
{% endcode %}

{% hint style="warning" %}
Der vil snart blive oprettet et **Maven Repository**, så man ikke skal import en lokal fil.
{% endhint %}

### Step 3 - Create Addon.yml file

For at pluginet kan registere dit Addon, skal du tilføje en **addon.yml** fil til din **resource-mappe**, som giver pluginet information om dit addon.

{% code title="addon.yml" %}
```
name: ExampleAddon
main: org.example.addon.ExampleAddon
version: 1.2
authors: [Plexhost.dk]
description: Beskrivelse
```
{% endcode %}

### Step 4 - Create Main Class

Du skal nu oprette en java class, som **"main"** refere til i addon.yml.\
I vores tilfælde er det en class med navnet **ExampleAddon** i packagen **org.example.addon**

Classen skal **extend** classen **BandeAddon**

{% code title="ExampleAddon.java" %}
```java
package org.example.addon;

import dk.plexhost.bande.addon.BandeAddon;
import dk.plexhost.bande.events.BandeCreateEvent;
import org.bukkit.Bukkit;
import org.bukkit.event.EventHandler;
import org.bukkit.event.Listener;

public class ExampleAddon extends BandeAddon implements Listener {

    @Override
    public void onEnable() {
        /*
         * We register the EventListener here.
         */
        Bukkit.getPluginManager().registerEvents(this, getMainPlugin());
    }

    @EventHandler
    public void onBandeCreate(BandeCreateEvent event){
        /*
         * We log to the console, that a new Bande has been created.
         */
        this.getMainPlugin().getLogger().info(event.getPlayer().getName() + " created bande " + event.getBande().getName());
    }


}

```
{% endcode %}

### Step 5 - Register Addon

Det eneste du skal gøre for at dit addon bliver registeret, er at smide det ind i **/plugins/Bande/addons** mappen.
