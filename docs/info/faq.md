# ❓FAQ

## Q: How to set other item plugins's item as reward?

A:

```yaml
rewards:
  reward_1:
    reward:
      hook-plugin: MMOItems
      hook-item: 'AXE;;MAGIC_AXE'
    amount: 1
    chance: 1
```

## Q: How to generate archeology block at world?

A: Please use `/ca arch` command to start generation.

## Q: Does this plugin generate archeology block at loaded chunk?

A: Yes. But chunk that already generated archeology blocks won't try generate again.

## Q: This plugin make my server lag when genetating archeology blocks.

A: This maybe lead to by you didn't use vanilla world generater, try remove all your archeology block config's `gaussian` section maybe solve your problem.

## Q: Does this plugin require resource pack?

A: Yes, and if your server has ItemsAdder or Oraxen, plugin will auto merge resource pack and you don't need do anything!

## Q: I can't see the archeology block, why?

A: Try update the plugin to latest or your resource pack has some issues.
