# Police Job inventory assets

Copy the supplied PNG files into the image directory used by the configured
inventory. Item catalog entries remain framework/inventory specific; the
Police Job registers their usable callbacks through `Sky.FW` at runtime.

## Crime scene tape

- Item name: `crime_scene_tape`
- Label: `Crime Scene Tape`
- Suggested weight: `750`
- Stackable: yes
- Close inventory on use: yes
- Image: `crime_scene_tape.png`

The usable callback is registered automatically while
`Config.CrimeSceneTape.enabled` is `true`. The default setup consumes one item
when a tape barrier is placed and returns it when an authorized officer removes
the barrier. Jobs, duty state, model, distances and inventory behavior are all
configurable in `Config.CrimeSceneTape` and `/jobconfig`.

Example catalog entries:

```lua
-- ox_inventory data/items.lua
['crime_scene_tape'] = {
    label = 'Crime Scene Tape',
    weight = 750,
    stack = true,
    close = true,
},

-- QBCore shared/items.lua
crime_scene_tape = {
    name = 'crime_scene_tape',
    label = 'Crime Scene Tape',
    weight = 750,
    type = 'item',
    image = 'crime_scene_tape.png',
    unique = false,
    useable = true,
    shouldClose = true,
    description = 'Portable crime scene barrier tape',
},
```

For ESX inventories, add the same item name and label to the inventory's item
catalog. No custom usable event is required; `sky_policejob` owns that part.
