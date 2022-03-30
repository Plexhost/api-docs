---
description: Hvordan laver man levels?
---

# Levels



1. Vi starter med at oprette en `level1.yml` fil i mappen `/levels`
2. Så tilføjer vi hvilket level det tilhører.\
   `level: 1`
3. Og nu kommer vi til det sjove, nemlig at lave kravene.\
   Vi tilføjer først `requirements:` til filen.

Hvert et krav indeholder 3 dele.

1. **Kravet.**\
   Selve kravet bruger en relativ nem struktur. \
   Du opstiller den som en condition i en String.\
   Her er det nemmest at bruge de indbyggede placeholders til at opnå\
   det ønskede resultat.\
   \
   Vi tager et eksempel hvor vi vil have et krav, hvor ens Bande Skade skal være \
   mindre eller lig med 95.\
   \
   Det første del af **conditionen** er så vores bande skade, \*\
   som har placeholderen: `<shop_bandeskade>`\
   ``\
   ``Den anden del er **operatoren**, altså at det skal mindre eller lig med.\
   Følgende operators kan bruges:\
   \- **`=`** og **`==`** (lig med)\
   \- **`<=`** og **`=<`** (mindre eller lig med)\
   \- **`>=`** og **`=>`** (større eller lig med)\
   \- **`>`** (større end)\
   \- **`<`** (mindre end)\
   \
   Vi kan så se at **mindre eller lig med** operatoren er **`<=` ** \
   ****\
   ****Den sidste del er så tallet, vi skal bruge tallet **95.**\
   ****\
   ****Så skal vi bare sætte den sammen.\
   Så den ender med at se ud som: `requirement: "<shop_bandeskade><=95"`\

2. **Tekst der vises når man har klaret det.**\
   Det opstilles som: `completed: "&a&l✔ &aKøb bandeskade ned til &295%"`\

3. **Tekst der vises når man ikke har klaret det.**\
   Det opstilles som: `not-completed: "&c&l✘ &7Køb bandeskade ned til &c95%"`\


Jeg har lige været så venlig at færdiggøre den for jer, så i kan se hvordan det første default level ser ud.

{% code title="level1.yml" %}
```yaml
level: 1 # Bandens level for at det er disse krav der gælder.
requirements:
  1:
    requirement: "<shop_bandeskade><=95"
    text:
      completed: "&a&l✔ &aKøb bandeskade ned til &295%"
      not-completed: "&c&l✘ &7Køb bandeskade ned til &c95%"
  2:
    requirement: "<amount_members>>=2"
    text:
      completed: "&a&l✔ &aOpnå &22 medlemmer&a i banden."
      not-completed: "&c&l✘ &7Opnå &c2 medlemmer&7 i banden."
  3:
    requirement: "<amount_allies>>=1"
    text:
      completed: "&a&l✔ &aOpnå &21 allieret&a i banden."
      not-completed: "&c&l✘ &7Opnå &c1 allieret&7 i banden."
```
{% endcode %}
