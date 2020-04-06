
# Resources

In order to provide easy to edit and modify parts and mecha, we'll be implementing a flatfile json format

File structure:

```
resources/
  parts/
  modules/
  mecha/
```

Mecha files:

```json
{"mechas": {
  // each key is the unique id for the mecha in question, this allows overrides via mods
  "gundam": {
    "name": "Gundam",
    "skeleton": "humanoid"
    "parts": [
      {
        "key": "gundam_head",
        "modules": [
          {"key": "60mm_head_vulcans"},
          {"key": "double_eye_sensors"},
          {"key": "gundanium_armor"}
        ]
      }
    ]
  }
}}
```

Part files:

```json
{
  "parts": {
    "gundam_head": {
      "name": "Gundam Head",
      "meshes": [
        {
          "file": "head.fbx",
          "bone:": "head",
          "translate": [0, 0, 0], // default
          "rotate": [0, 0, 0], // default
          "scale": [0, 0, 0] //default
        }
      ]
    }
  }
}
```
