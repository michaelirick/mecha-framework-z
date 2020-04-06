
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

```
{"mechas": {
  # each key is the unique id for the mecha in question, this allows overrides via mods
  "gundam": {
    "name": "Gundam",
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
