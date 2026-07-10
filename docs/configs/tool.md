# 🛠️Tool

All archaeology tools are stored in the `tools` folder. The name of the configuration file is the ID of the tool.

The configuration file for an example tool is as follows:

```yaml
# The name of tool
display-name: "Archaeological Shovel"
# The lore of tool.
lore:
  - "&7A Archaeological Shovel"
# The texture of tool, should use texture ID.
texture: archaeological_shovel
# The recipes of tool, support register more than 1 recipe, replace ? with numbers starting from 1.
recipe_1:
  shape:
    - " AA"
    - " BA"
    - "B  "
  ingredients:
    A:
      # Type Item Format here.
      material: copper_ingot
    B:
      material: stick
```
