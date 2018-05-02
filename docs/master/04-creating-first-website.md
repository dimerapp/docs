---
permalink: creating-first-website
category: root
---

# Creating first website

We have released Dimer beta with the Command line binaries for all major operating systems. This guide handholds you in using the CLI interface and publish your markdown files.

[tip]
Dimer only needs markdown files to generate a documentation website. Say goodbye to complex build tools 👋
[/tip]

## Useful links

- [Dimer for Mac](dimer-for-mac)
- [Dimer For Linux](dimer-for-linux)
- [Dimer For Windows](dimer-for-windows)

Before getting started, make sure you have the CLI installed and running `dimer` results similar to the following output.

![](http://res.cloudinary.com/adonisjs/image/upload/q_100/v1525059195/dimer-help_gwctqj.png)

#### Step 1

Create an empty directory and run the following command inside it to create a JSON formatted config file.

```bash
dimer init

# created dimer.json
```

#### Step 2

Now open `dimer.json` and update the website settings.

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

| Key | Description |
|-----|--------------|
| subdomain | Subdomain is the website address suffixed with `.dimerapp.com`. Subdomain must be URL friendly and should not contain `http` or `https`.
| cname |  Cname is the custom domain that you want to point to `subdomain.dimerapp.com`. [Learn more](custom-domain) about cnames. |
| defaultVersion | The default version for your documentation. Users will land on this version when URL doesn't point to a specific version. |
| versions | A map of documentation versions. If your docs only have one version, then let leave it as `master`. |
| theme | Documentation website theme. We currently support `default` theme only. |
| themeSettings | A key value pair of options you can define for the selected theme.[Here's the list of all the available options](theme-options) |

### Step 3

As per the default configuration. The documentation for the `master` version will be inside a subdirectory called `docs/master`. Let's create/copy your markdown files inside this directory.

Once done, run the following command to publish it.

```bash
dimer publish
```

Congratulations! You have just published your documentation on dimer.

## Troubleshooting
Not every time, things go as per the plan. In case of any confusion, make sure to read the [troubleshooting](define-a-subdomain) section, ask for help on [Slack](https://dimerapp.slack.com)  or reach us directly from the [help page](https://dimerapp.com/help)
