# 🔗Compatibility

This plugin mainly adds **direct compatibility** for some item plugins.

## **Direct compatibility** <a href="#direct-compatibility" id="direct-compatibility"></a>

### <mark style="color:red;">Directly</mark> supported item plugins list

You can use items from these plugins in [ItemFormat](https://ultimateshop.superiormc.cn/format/itemformat-tm).

* ItemsAdder
* Oraxen
* EcoItems
* EcoArmor
* MMOItems
* MythicMobs
* eco
* NeigeItems
* ExecutableItems
* Nexo
* CraftEngine

### <mark style="color:red;">Directly</mark> supported protection plugins list <a href="#directly-supported-protection-plugins-list-premium" id="directly-supported-protection-plugins-list-premium"></a>

If players do not have permission to place or break blocks within these protection plugins areas, CustomArcheology can prevent players place or break archeology blocks in these areas.

* BentoBox
* Dominion
* GriefPrevention
* HuskTowns
* HuskClaims
* Lands
* PlotSquared
* Residence
* Towny
* WorldGuard

## MythicDungeons: Extra function <a href="#neigeitems-item-name-translation-hook" id="neigeitems-item-name-translation-hook"></a>

A addon plugin called **ManyouMDExtension** add new function to MythicDungeons.

* Place archeology block

Download Link: [https://www.spigotmc.org/resources/manyoumdextension-add-more-functions-for-mythicdungeons-for-our-plugins-1-14-1-21-4.99816/](https://www.spigotmc.org/resources/manyoumdextension-add-more-functions-for-mythicdungeons-for-our-plugins-1-14-1-21-4.99816/)

## BetterStrucutres: Custom Genearete Rule

* Support genearate archeology block at specified BetterStrucutres's strucutre.

## NBTAPI: Extra Item Format option <a href="#nbtapi-extra-item-format-option-premium" id="nbtapi-extra-item-format-option-premium"></a>

For info about ItemFormat, please view UltimateShop wiki [here](https://ultimateshop.superiormc.cn/format/itemformat-tm).

The format of this option is:

```yaml
nbt:
  <NBT Type>:
    <NBT Key>: <NBT Value>
```

Supported NBT Type:&#x20;

* byte
* short
* int
* long
* float
* double
* string

For example:

```yaml
nbt:
  string: 
    customNBT: 'Hello!'
  int:
    anotherNBTComponent.theNBTKey: 5
```
