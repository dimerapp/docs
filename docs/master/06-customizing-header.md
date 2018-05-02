---
permalink: customizing-header
category: root
---

# Customizing header

Dimer let you update the look and feel of the website header so that you can make it look closer to your brand.

In nutshell you will be able to update

- The header background color
- Logo
- Add navigation links

## Updating config

Let's open `dimer.json` file and add values inside the `themeSettings` block.

```json
{
  "themeSettings": {
    "headerBg": "#222222",
    "logoUrl": "",
    "navbar": {}
  }
}
```

#### headerBg
Header background color must be a valid color code. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)

#### logoUrl
A valid http or https url to your brand logo. For better rendering, make sure logo **height is under 48px**

#### navbar
A key/value pair of navigation links and their titles. Nested key/values will appear as a dropdown.  

```json
{
  "Home": "https://dimerapp.com",
  "Community": {
    "Github": "https://github.com/dimerapp",
    "Slack": "https://slack.dimerapp.com"
  }
}
```

