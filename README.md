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

2. add `"transparent": true` to `tauri.conf.json`, so that the window is transparent.

```JSON
{
  "tauri": {
    "windows": [
      {
        "transparent": true
      }
    ]
  }
}
```

**NOTE**: according to [tauri docs](https://tauri.app/v1/api/config/#windowconfig)，you need to enable `macos-private-api` feature flag to use this feature on macOS.

> on macOS this requires the macos-private-api feature flag, enabled under tauri > macOSPrivateApi. 

