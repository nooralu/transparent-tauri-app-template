A simple demo of creating a transparent tauri window.

# Steps

1. add `"decorations": false` to `tauri.conf.json`, so that the window is borderless.

```JSON
{
  "tauri": {
    "windows": [
      {
        "decorations": false
      }
    ]
  }
}
```

before:

![decorations](./screenshots/decorations.png)

after:

![no-decorations](./screenshots/no-decorations.png)

