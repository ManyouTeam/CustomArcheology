# ⚙️Install

## Plugin Install <a href="#install" id="install"></a>

* Put the `.jar` file into your server's `plugins` folder.
* Correct `settings.block-material` option in `config.yml` file, for more info, please view [this page](configuration-files.md). <mark style="color:red;">**This option can only changed before use this plugin!**</mark>
* Stop your server and then restart it. <mark style="color:red;">Cannot load plugins in any other way while the server is starting</mark>.
* When updating plugins, please be sure to remove old versions.
* When downgrading from **a new game version** to **an old version** on the server where the plugin is located, it is important to remove the `pack` folder from the configuration file.
* When using the [Localized Item Name](../features/localized-item-name.md) feature, it is important to note that when switching server game versions, the previously generated localized files need to be deleted.
* Since `1.20.1` and `1.20.1+` has some changes about game packets, so if you are upgrading server from `1.20` or `1.20.1` version to `1.20.1+` version, you need regenerate resource pack to make all things work well.
* This plugin will generate resource pack at `pack` folder, you need install the resource pack to your client or using plugins like **ItemsAdder** or **Oraxen** to send the resource pack to client.

## Resource Pack Install <a href="#custom-card-and-ui-texture" id="custom-card-and-ui-texture"></a>

CustomArcheology requires your player use specifeid resource pack to display custom archeology block and tools, so:

* If your server don't have resource pack yet, just zip your pack folder and ask your players install it in their Minecraft client. For more info, please view below.
* If your server use other resource pack plugin, you need merge these two resource packs first. For ItemsAdder and Oraxen plugin, we have auto merge feature. (Require enable `auto-copy-resourcepack.enabled` option in config.yml and set correct value at auto-copy-resourcepack config section)

### How to install resource pack? <a href="#how-to-install-resource-pack" id="how-to-install-resource-pack"></a>

First, you have to answer me a question: **Are you using resource pack plugins like ItemsAdder?**

If no, you must install the resource pack at Minecraft client.

* Open the game.
* At main menu, click **Options...** button.
* At options menu, click **Resource Packs...** button.
* Zip plugin's `/pack/` folder, then drag and drop it to this window.
* Click the new resource pack to add it to game.
* All is done, join your server and now you will see custom card textures!

If yes, you have to merge the two resource pack. For ItemsAdder and Oraxen plugin, we have [auto merge](../features/auto-copy-resource-pack.md) feature. (Require enable `auto-copy-resourcepack.enabled` option in config.yml and set correct value at auto-copy-resourcepack config section)

* We use **Blue\_dye** as material, if your other resource pack plugin does not use it as material, you just need copy and paste FlipCard's resource pack to the other plugin's resource pack.
* If your other resource pack plugin use it **White\_dye** as material, you have to merge the two resource pack. This is a little complex, maybe [this site ](https://merge.elmakers.com/)can help you. What's more, you can also contact our staff to help you merge!
* **CustomArcheology does not send the resource pack to players**, so you need use the other resource pack plugin to send the merged resource pack to players.
