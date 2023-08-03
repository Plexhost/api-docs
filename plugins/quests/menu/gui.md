# Gui

### GUI Layout

{% code title="default_gui.yml" %}
```yaml
gui:
    id: default_gui
    title: '&a&lDefault GUI'
    rows: 5
    slots:
        disabled_slot:
            enabled: false # Defaulter til true, så ikke nødvendig at skrive.
            item:
                ....
        enabled_slot:
            item:
                ....
```
{% endcode %}

### Item Layout

{% code title="default_gui.yml" %}
```yaml
gui:
    ...
    slots:
        head:
            item:
                name: '&l&lSejt Hovede?!'
                lore:
                - "Dette item har"
                - "en lore. OMG"
                material: SKULL
                value: "eeyJ0ZXh0dXJlcyI6eyJTS0lOIjp7InVybCI6Imh0dHA6Ly90ZXh0dXJlcy5taW5lY3JhZnQubmV0L3RleHR1cmUvNGRjY2IyNmExYjc1NWFkMjZkYTgwNWE0NmZhMmVhYjVjMWZkYmY1ZDU3Njg3YzkxMGRlNTY3N2MyMDBlYmM2MyJ9fX0"
                enchanted: true
                slot: 29
        dye:
            item:
                name: '&l&lFarve'
                material: INK_SACK
                data: 7
                slot: 29
                
```
{% endcode %}
