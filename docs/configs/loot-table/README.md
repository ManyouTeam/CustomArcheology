# 💎Loot Table

All loot tables are stored in the `loottables` folder. The name of the configuration file is the ID of the loot table.

An example loot table configuration file is as follows:

<pre class="language-yaml"><code class="lang-yaml">rewards:
  reward_1:
    reward:
      material: emerald
    amount: 1
    chance: 1
  reward_2:
    reward:
      material: diamond
    amount: 1
    chance: 1
  reward_3:
    display-item:
      material: iron_ingot
    amount: 1~2
    chance: 10
    actions:
      - 'console_command: say hello, {player}'
  reward_4:
    display-item:
      material: dirt
    amount: 1~3
    chance: 20
    spawn-actions:
      - 'entity_spawn: ZOMBIE'
  reward_5:
    reward:
      material: suspicious_stone
<strong>    amount: 10~32
</strong>    chance: 10
</code></pre>

There are several sub-keys under the `rewards` key, such as `rewards_1, reward_2`. They are the IDs for each reward. Each reward has the following options to set:

* display-item: Items gradually emerging from archaeology blocks while players are excavating them. This option is optional. If it is not set, the item in the `reward` option will be used as the display item. **Need type** [**Item Format**](https://ultimateshop.superiormc.cn/format/itemformat-tm) **here.**
* reward: After the player excavates the archaeological block, the dropped item that pops up from the archaeology block serves as a reward for the player. **Need type** [**Item Format**](https://ultimateshop.superiormc.cn/format/itemformat-tm) **here.**

You can see from the above two options that there are two stages when players excavate archaeology blocks:

* State 1: The player is using a brush to excavate archaeological blocks, and potential reward items may appear on the archaeology blocks. Use Item Format.
* State 2: Archaeology blocks are excavated and drop items as rewards. Use Item Format.

A picture for State 1:

![](https://customarcheology.superiormc.cn/~gitbook/image?url=https%3A%2F%2F4281561411-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FIqo7Ab8fthDqhrg1mwtO%252Fuploads%252FDBJ8TbTFu3PuL6WogDjU%252F%25E5%25B1%258F%25E5%25B9%2595%25E6%2588%25AA%25E5%259B%25BE%25202023-12-27%2520132007.png%3Falt%3Dmedia%26token%3D6a9aeb96-dfd3-4254-a4df-97f0e06d280d\&width=768\&dpr=4\&quality=100\&sign=14b0c406\&sv=2)

When players excavate archaeology blocks, the items they see and the actual items they obtain can be deceived by setting different values for two options. Players think they are about to obtain a diamond, but in reality they have only obtained a bone!

Other options:

* amount: The number of items for this reward.
* chance: The weight of the reward is drawn, and the actual probability of winning the reward is the weight of the reward divided by the weight of all rewards.
* spawn-actions: The action performed by the player when excavating archaeological blocks.
* actions: The action performed by the player when picking up the reward item they have obtained.

After setting the spawn-actions and actions options, players will no longer be able to receive reward items obtained by excavating archaeology blocks.

## Action Format

Please view [this page](actions.md) for info.
