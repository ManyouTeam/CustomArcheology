# 🔄Auto Copy Resource Pack

* Open `config.yml` file, and fine below contents:

```yaml
auto-copy-resourcepack:
  enabled: true
  # If you are using Oraxen, please change this to Oraxen.
  # Other plugins is OK, you just need put correct path in path option.
  plugin: "ItemsAdder"
  # If you are using Oraxen, please change this to "/pack/assets".
  path: "/contents/customarcheology/resourcepack/"
```

* Please set `auto-copy-resourcepack.enabled` option to true.
* Please set `auto-copy-resourcepack.plugin` option to the resource pack you are using. Support **ALL** resource pack plugin.
* Please set auto-copy-resourcepack.path option to the directory for storing texture for this resource package plugin, for example:
  * ItemsAdder: `/contents/customarcheology/resourcepack/`
  * Oraxen: `/pack/assets`
