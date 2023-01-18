# Skript-Reflect Snippet

```vbnet
import:
    dk.plexhost.bande.BandePlugin

load:
    set {BANDE} to BandePlugin.getAPI()

offlineplayer property bande:
    return type: object
    get:
        return {BANDE}.getBande(expr-1)

offlineplayer property bande id:
    return type: number
    get:
        return (expr-1's bande).getId()

offlineplayer property bande name:
    return type: text
    get:
        return (expr-1's bande).getName()

expression b-stat %text% of %player%'s bande:
    return type: number
    get:
        set {_bande} to expr-2's bande
        if {_bande} is not set:
            stop
        return {_bande}.getStat(expr-1)
    set:
        set {_bande} to expr-2's bande
        if {_bande} is not set:
            stop
        {_bande}.setStat(expr-1, the change value)
    add:
        set {_bande} to expr-2's bande
        if {_bande} is not set:
            stop
        {_bande}.addStat(expr-1, the change value)
    remove:
        set {_bande} to expr-2's bande
        if {_bande} is not set:
            stop
        set {_current} to {_bande}.getStat(expr-1)
        {_bande}.setStat(expr-1, {_current}-the change value)
    reset:
        set {_bande} to expr-2's bande
        if {_bande} is not set:
            stop
        {_bande}.setStat(expr-1, 0)


condition %player% has bande:
    check:
        set {_bande} to expr-1's bande
        if {_bande} is set:
            continue

condition %player% has bande permission %string%:
    check:
        set {_bande} to expr-1's bande
        if {_bande} is not set:
            stop
        if {_bande}.getRank(expr-1.getUniqueId()) <= {_bande}.getPermission(expr-2):
            continue
```
