---
description: Lær hvordan du kan integere dine egne levels i pluginet.
---

# Add your own level

Alle Levels kræver sin egen class som extender **BandeLevel.**

{% code title="Level_2.java" %}
```java
package org.example.addon.levels;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;

import java.util.ArrayList;
import java.util.List;

// Vi extender BandeLevel for at vi kan registere levelet senere hen.
public class Level_2 extends BandeLevel {

    // Denne funktion bliver callet når nogle prøver at level op.
    @Override
    public boolean meetsRequirements(Bande bande) {
        
        // Går igennem kravene og returner false hvis de ikke bliver opfyldt.
        if(bande.getBandeSkade() > 95) return false;

        // Return true for at fortælle pluginet af banden kan level op.
        return true;
    }

    // Dette er en liste over tekst der bliver vist i ens Bande Information GUI.
    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        List<String> response = new ArrayList<>();
        
        // Banden opfylder ikke krav.
        if(bande.getBandeSkade() > 95) response.add("&c&l✘ &7Køb bandeskade ned til &c95%");
        
        // Banden opfylder kravet.
        else response.add("&a&l✔ &aKøb bandeskade ned til &295%");

        return response;
    }
}
```
{% endcode %}

Perfekt! Nu har vi lavet vores første level, så nu skal vi bare tilføje det til systemet.\
Det gør vi ved at brug af **BandeAPI** classen.

{% code title="ExampleAddon.java" %}
```java
package org.example.addon;

import dk.plexhost.bande.addon.BandeAddon;
import dk.plexhost.bande.BandePlugin;
import org.bukkit.Bukkit;
import org.bukkit.event.EventHandler;
import org.bukkit.event.Listener;

import org.example.addon.levels.*;

public class ExampleAddon extends BandeAddon {

    @Override
    public void onEnable() {
        
        // Vi kører methoden der hooker vores levels ind i systemet.
        this.enableLogins();
    }
    
    // Denne method bliver kørt hver gang at /bande reload bliver kørt.
    // Vi tilføjer levelsne igen, fordi at de bliver fjernet under en reload.
    @Override
    public void onReload() {
        
        // Vi kører methoden der hooker vores levels ind i systemet.
        this.enableLogins();
    }
    
    // Vi laver en method fordi at vi skal hook levels ind i pluginet flere gange.
    private void enableLogins(){
    
        // Vi tilføjer vores nye level til levelet 2.
        // Det betyder at en level 1 bande skal opfylde disse krav.
        BandePlugin.getAPI().addLevel(2, new Level_2());
    }

}

```
{% endcode %}
