# Actions

## Action Suffix

* All actions support add suffix.
* `~<Interger>` means the chance the action will be excuted, up to 100. 50 means this action has 50% chance to excute. Like:

```yaml
    actions:
      - 'console_command: say hello, {player}~50'
```

## Sound

Send sound to player.

```yaml
- 'sound: ui.button.click;;1;;1' 
# "sound: SOUND;;volume;;pitch"
```

## Message

Send a message to the player, support color code.

```yaml
- 'message: Hello!'
```

## Announcement

Send a message to all online players, support color code.&#x20;

```yaml
- 'announcement: Hello!'
```

## Effect

Give players potion effect.

```yaml
- 'effect: BLINDNESS;;1;;60'
```

**BLINDNESS** is SpigotAPI effect ID, its different form minecraft effect namespace, you can find them here: [https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/potion/PotionEffectType.html](https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/potion/PotionEffectType.html).

**1** is effect level.

**60** is effect duration.

## Teleport

Teleport player to specified location.

```yaml
- 'teleport: LobbyWorld;;0;;128;;10'
```

**LobbyWorld** is world name.

**0** is X pos.

**128** is Y pos.

**10** is Z pos.

You can also add yaw and pitch at the end of action string, like:

```yaml
- 'teleport: DungeonWorld;;100;;30;;300;;90;;0'
```

## Player Command

Make the player excutes a command.

```yaml
- 'player_command: tell i am a boy!'
```

## Op Command

Make the player excutes a command as OP.

```yaml
- 'op_command: tell i am a boy!'
```

## Console Command

Make the console excutes a command.

```yaml
- 'console_command: op %player%'
```

## Spawn vanilla mobs

Spawn vanilla mobs, mob ID follow this page:

[https://hub.spigotmc.org/javadocs/spigot/org/bukkit/entity/package-summary.html](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/entity/package-summary.html)

```
- 'eneity_spawn: ZOMBIE'
```

## MythicMobs spawn

### MythicMobs Spawn at block location

Require MythicMobs.

<pre class="language-yaml"><code class="lang-yaml"><strong>- 'mythicmobs_spawn: test;;1'
</strong></code></pre>

`test` is **Mob ID**, `1` is the **level**. Mob ID and level use `;;` spite.

Level can remove, this means you can set:

```yaml
- 'mythicmobs_spawn: test'
```

### MythicMobs Spawn at remote location

Require MythicMobs.

Simailr to MythicMobs Spawn at block location, but you need add `;;world name;;x;;y;;z` at the end of action string, for example:

```yaml
- 'mythicmobs_spawn: testMonster;;LobbyWorld;;11;;64;;12'
```
