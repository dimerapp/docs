---
permalink: yaml-front-matter
category: root
---

# YAML front matter

YAML front matter helps you in defining meta data for your markdown file. In this guide we learn about it's syntax and available meta data options.

The meta data is always defined at the top of the markdown file fenced between `---` 3 dashes.

```markdown
---
permalink: hello-world
category: greetings
---

Here goes the markdown content
```

As you can see, the very first block is wrapped within opening and closing 3 dashes. This is how we define the meta data within the markdown file.

## permalink
By default, dimer generates the document URL from the filename. This works great as a starting point, but limits you from changing the filename, since it will result in a broken URL.

The permalink propery helps you in defining the permanent URL for your docs. Always make sure the value is URL friendly and doesn't contain any spaces or special characters.

```md
---
permalink: overview
---
```

## category
The `category` option defines the category for a doc. All docs with the same category value, will be grouped together in the sidebar.

```md
---
category: getting-started
---
```

## title
The `title` of the document is like a movie name. Since a movie can never be released without a name, in the same way a document can never be published without a title.

You can omit the `title` field, if your document defines a **top level h1**.

##### Defining explicitly
```md
---
title: Hello world
---
```

##### Used h1 implicitly
```md
# Heading 1 can also be a valid title
```
