---
description: Dette kræver Skript-Reflect
---

# Citizens integration

{% hint style="info" %}
Husk at spilleren stadig skal have **itemflip.use** for at bruge menuen.
{% endhint %}

```vbnet
import:
  dk.plexhost.itemflip.userinterface.UIOptions
  dk.plexhost.itemflip.ItemFlipPlugin

rightclick on entity:
  if citizen id of event-entity = id på din npc:
    ItemFlipPlugin.getInstance().getUIManager().openGui(player, "start", new UIOptions())
```
