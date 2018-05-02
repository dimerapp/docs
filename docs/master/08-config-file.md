---
permalink: dimer-config-file
category: root
---

# Config file
The config file `dimer.json` is the heart of a dimer project. It contains all neccessary information to setup and customize your documentation website.

Each project/website will have it's own configuration file, which is created by running the following command.

```bash
dimer init

# Created dimer.json
```

The file is formatted in JSON and looks similar to the following snippet.

```json
{
  "subdomain": "",
  "cname": "",
  "defaultVersion": "master",
  "versions": {
    "master": "docs/master"
  },
  "theme": "default",
  "themeSettings": {}
}
```

## subdomain
Each website must have a unique subdomain suffixed with `.dimerapp.com`. For example:

- adonisjs
- or adonisjs.dimerapp.com

The subdomain is used to access your website on the internet.

## cname
The `cname` property is used to map a custom domain to your dimerapp.com URL. For this, you will also have to make some minor changes in your DNS server. Learn more about cnames [here](custom-domain).

## defaultVersion
If your website only maintains a single version of documentation, then let this value as it is. Otherwise, you can define the version number on which users must land by default.

## versions
Again, no changes are required if you only maintain a single version of documentation. Otherwise you can define a map of **key/value** pairs. 

The key defines the version number and value points to a directory in which markdown files for that version are stored.

```json
{
  "versions": {
    "1.0": "docs/v1",
    "1.1": "docs/v1"
  }
}
```

Also you can define human friendly display name for a version as follows.

```json
{
  "versions": {
    "1.0": {
      "name": "Version 1",
      "path": "docs/v1"
    }
  }
}
```

## theme
The `theme` property defines the output theme for your documentation. Currently we only support one theme i.e `default`, so please leave this option as it is.

## themeSettings
Each theme exposes a set of configuration options, that you can define in order to integrate some services or customize the outlook of your website.

Make sure to read the [theme settings](theme-settings) guide for same.
