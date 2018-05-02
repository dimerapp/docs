---
permalink: theme-settings
category: root
---

# Theme settings
In this guide we explore the available options to customize the theme outlook or integrate different services.

Following is the list of available `themeSettings`.

```json
{
  "themeSettings": {
    "headerBg": "#333",
    "logoUrl": "",
    "navbar": {},
    "gaId": ""
  }
}
```

## headerBg
The `headerBg` options accepts a [valid color code](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) to change the background color of the main header.

## logoUrl
Here you define an http or https URL of your brand logo. For better results, make sure the **logo height is under 48px**.

## navbar
The default theme let you show links in the header. You can use this option to display a navbar with links to your website or social accounts.

The key is link text and value is the URL it should point to.

```json
{
  "navbar": {
    "Home": "https://dimerapp.com",
    "Github": "https://github.com/dimerapp",
    "Twitter": "https://twitter.com/dimerapp"
  }
}
```

Also you can define one level nested navbar, which appears as a dropdown menu.

```json
{
  "navbar": {
    "Home": "https://dimerapp.com",
    "Community": {
      "Github": "https://github.com/dimerapp",
      "Twitter": "https://twitter.com/dimerapp"
    }
  }
}
```

## gaId
The `gaId` is the Google analytics id. You can get it from the analytics admin section, right **above the embed code**.
