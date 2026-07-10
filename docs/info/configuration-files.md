# 🛠️Configuration files

After the plugin is successfully loaded for the first time, several folders and files will be generated in the `plugins/CustomArcheology` directory in the server's root directory. These are the configuration files for **CustomArcheology**. Here is an introduction to the purpose of each folder and file:

* `blocks` folder: A folder containing the configuration files for archaeology blocks. It stores the configuration files for all the archaeology blocks in the plugin.
* `languages` folder: A folder containing the configuration files for plugin languages. It stores the language files for the plugin. You can set the language file used by the plugin in `config.yml`.
* `loottables` folder: A folder containing the configuration files for loot tables. It stores the configuration files for all the loot tables in the plugin. Loot tables are often used in the configuration files for archaeology blocks to specify the rewards that players can obtain after archaeological excavation.
* `pack` folder: The directory where the plugin generates the resource pack. **CustomArcheology** needs to be used in conjunction with a resource pack, and you need to distribute this resource pack to players.
* `textures` folder: The directory where the textures for plugin archaeology blocks and archaeological tools are stored.
* `tools` folder: A folder containing the configuration files for archaeological tools. It stores the configuration files for all the archaeological tools in the plugin.
* `config.yml`: The main configuration file for the plugin. Common configuration options are usually provided here.
* `generated-item-format.yml` file: When using the `/ca generateeitemformat` command, we will parse the item you are holding into an **ItemFormat** and store the parsed **ItemFormat** content in this file.
* `XX_xx.json` file: Localized files automatically generated through [Localized Item Name](https://mythicchanger.superiormc.cn/features/localized-item-name-premium) feature. The name of this file is determined based on the localized language you have set for this feature, but it usually ends in `. json`.

## Config.yml file content <a href="#config.yml-file-content" id="config.yml-file-content"></a>

```yaml
# CustomArcheology by @rzt1020 & @PQguanfang
#
# Read the Wiki here: customarcheology.superiormc.cn
# Purchase the plugin, and you can get free texture expansion pack with 5 tools, 6 blocks included!

log-generated-block: false

config-files:
  generate-default-files: true
  language: en_US
  minecraft-locate-file:
    # After enable, we will autoload Minecraft locate file when we need know an item's locate name.
    # It will make server little lag when loading this file because this file is very large.
    enabled: true
    generate-new-one: false
    file: 'zh_cn.json'

auto-copy-resourcepack:
  enabled: true
  # If you are using Oraxen, please change this to Oraxen.
  # Other plugins is OK, you just need put correct path in path option.
  plugin: "ItemsAdder"
  # If you are using Oraxen, please change this to "/pack/assets".
  path: "/contents/customarcheology/resourcepack/"

database:
  use-mysql: false
  mysql:
    host: localhost
    port: 3306
    user: root
    password: root
    database: minecraft

settings:
  # Support value: UUID or RANDOM
  block-save: UUID
  block-material: STONE
  start-custom-model-data:
    block: 10000
    tool: 10000
  visible-distance: 8
  item-scale: 0.5
  block-scale: 0.25
  hook:
    betterstructures: true
```

## Block Material

You can use this option to set the original block on which the archaeological block is based, with a default value of **STONE**.&#x20;

You have to correct this option before use the plugin, if you have changed this option, all archeology block generated before will all <mark style="color:red;">**BROKEN**</mark>!

It is recommend you set the material to be one block, like STONE, otherwise sometimes transparent edges of archaeological blocks.
