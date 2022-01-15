# Builtin Levels

Dette er classesne af alle de levels der kommer med pluginet.

{% tabs %}
{% tab title="Level 2" %}
Kravene for at komme i **level 2**.

{% code title="Level_2.java" %}
```java
package dk.plexhost.bande.levels.builtin;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;

import java.util.ArrayList;
import java.util.List;

public class Level_2 extends BandeLevel {


    @Override
    public boolean meetsRequirements(Bande bande) {
        if(bande.getBandeSkade() > 95) return false;
        if(bande.getAmountOfMembers() < 2) return false;
        if(bande.getAmountOfAllies() < 1) return false;
        return true;
    }

    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        List<String> response = new ArrayList<>();

        if(bande.getBandeSkade() > 95) response.add("&c&l✘ &7Køb bandeskade ned til &c95%");
        else response.add("&a&l✔ &aKøb bandeskade ned til &295%");

        if(bande.getAmountOfMembers() < 2) response.add("&c&l✘ &7Opnå &c2 medlemmer&7 i banden.");
        else response.add("&a&l✔ &aOpnå &22 medlemmer&a i banden.");

        if(bande.getAmountOfAllies() < 1) response.add("&c&l✘ &7Opnå &c1 allieret&7 i banden.");
        else response.add("&a&l✔ &aOpnå &21 allieret&a i banden.");

        return response;
    }
}
```
{% endcode %}
{% endtab %}

{% tab title="Level 3" %}
Kravene for at komme i **level 3**.

{% code title="Level_3.java" %}
```java
package dk.plexhost.bande.levels.builtin;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;

import java.util.ArrayList;
import java.util.List;

public class Level_3 extends BandeLevel {


    @Override
    public boolean meetsRequirements(Bande bande) {
        if(bande.getBandeSkade() > 90) return false;
        if(bande.getAmountOfMembers() < 4) return false;
        if(bande.getStat("kills") < 50) return false;
        return true;
    }

    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        List<String> response = new ArrayList<>();

        if(bande.getBandeSkade() > 90) response.add("&c&l✘ &7Køb bandeskade ned til &c90%");
        else response.add("&a&l✔ &aKøb bandeskade ned til &290%");

        if(bande.getAmountOfMembers() < 4) response.add("&c&l✘ &7Opnå &c4 medlemmer&7 i banden.");
        else response.add("&a&l✔ &aOpnå &24 medlemmer&a i banden.");

        if(bande.getStat("kills") < 50) response.add("&c&l✘ &7Dræb &c50&7 spillere.");
        else response.add("&a&l✔ &aOpnå &250&a spillere.");

        return response;
    }
}

```
{% endcode %}
{% endtab %}

{% tab title="Level 4" %}
Kravene for at komme i **level 4**.

{% code title="Level_4.java" %}
```java
package dk.plexhost.bande.levels.builtin;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;
import dk.plexhost.bande.enums.RivalsType;

import java.util.ArrayList;
import java.util.List;

public class Level_4 extends BandeLevel {


    @Override
    public boolean meetsRequirements(Bande bande) {
        if(bande.getAmountOfAllies() < 3) return false;
        if(bande.getAmountOfRivals(RivalsType.OWN) < 3) return false;
        if(bande.getStat("kills") < 175) return false;
        return true;
    }

    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        List<String> response = new ArrayList<>();

        if(bande.getAmountOfAllies() < 3) response.add("&c&l✘ &7Opnå &c3 allierede&7 i banden.");
        else response.add("&a&l✔ &aOpnå &23 allierede&a i banden.");

        if(bande.getAmountOfRivals(RivalsType.OWN) < 3) response.add("&c&l✘ &7Opnå &c3 rivaler&7 i banden.");
        else response.add("&a&l✔ &aOpnå &23 rivaler&a i banden.");

        if(bande.getStat("kills") < 175) response.add("&c&l✘ &7Dræb &c175&7 spillere.");
        else response.add("&a&l✔ &aOpnå &2175&a spillere.");

        return response;
    }
}

```
{% endcode %}
{% endtab %}

{% tab title="Level 5" %}
Kravene for at komme i **level 5**.

{% code title="Level_5.java" %}
```java
package dk.plexhost.bande.levels.builtin;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;
import dk.plexhost.bande.enums.RivalsType;

import java.util.ArrayList;
import java.util.List;

public class Level_5 extends BandeLevel {


    @Override
    public boolean meetsRequirements(Bande bande) {
        if(bande.getBandeSkade() > 75) return false;
        if(bande.getAmountOfRivals(RivalsType.OWN) < 3) return false;
        if(bande.getBank() < 12000) return false;
        return true;
    }

    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        List<String> response = new ArrayList<>();

        if(bande.getBandeSkade() > 75) response.add("&c&l✘ &7Køb bandeskade ned til &c75%");
        else response.add("&a&l✔ &aKøb bandeskade ned til &290%");

        if(bande.getStat("kills") < 350) response.add("&c&l✘ &7Dræb &c350&7 spillere.");
        else response.add("&a&l✔ &aOpnå &2350&a spillere.");

        if(bande.getBank() < 12000) response.add("&c&l✘ &7Have &c$12.000&7 i bandens bank.");
        else response.add("&a&l✔ &aHave &2$12.000&a i bandens bank.");
        return response;
    }
}

```
{% endcode %}
{% endtab %}

{% tab title="Level 6" %}
Et eksempel på **max level**. Du kan ikke level op til **level 6**, da den altså vil deny det i **linje 13**.

{% code title="Level_5.java" %}
```java
package dk.plexhost.bande.levels.builtin;

import dk.plexhost.bande.addons.BandeLevel;
import dk.plexhost.bande.bande.Bande;
import dk.plexhost.bande.utils.Color;

import java.util.Collections;
import java.util.List;

public class Level_6 extends BandeLevel {

    @Override
    public boolean meetsRequirements(Bande bande) {
        return false;
    }

    @Override
    public List<String> getRequirementsMessage(Bande bande) {
        return Collections.singletonList(Color.getColored("&cBanden er i maks level."));
    }
}

```
{% endcode %}
{% endtab %}
{% endtabs %}
