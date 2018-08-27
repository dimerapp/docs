# Zones and Versions not allowed together

When writing documentation, you can make use of `zones` and `versions` to cleanly manage and present your content. However, they both are not allowed as top level keys inside the config file.

#### Incorrect config
```json
{
  "zones": {
    "guides": "guides"
  },
  "versions": {
    "master": "master"
  }
}
```

#### Correct config
```json
{
  "zones": {
    "guides": {
      "master": "guides/master"
    }
  }
}
```

When using zones and versions together, the versions must be nested inside zones. 
