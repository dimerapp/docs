---
permalink: customizing-sidebar
category: root
---

# Customizing sidebar

Documentation sidebar displays the hierarchy of documents optionally grouped inside categories. In this guide, we will learn how to customize the documents order or group them.

Before getting started, it is important to know that Dimer only supports one level deep category tree. This is an intentional limitation and in case of any questions, feel free to reach us.

## Defining category
The category for a document is defined using the YAML front matter.

```md
---
category: Tutorials
---
```

All the documents, that defines the same category will be grouped together in the sidebar.

Also it doesn't matter whether your documents are in a subfolder or not. Dimer simply relies on the category value defined as YAML frontmatter. 

## Managing order
The order in which topics are displayed in the sidebar is very important. Dimer follows the **same order in which files appears on your computer**. This approach gives you a visual clarity of the tree and also no overhead to maintain another config.

The simplest way to order files on your computer is to prefix them with a number.

![](http://res.cloudinary.com/adonisjs/image/upload/q_100/v1525180634/files_caxlqu.png)

## Subfolders

As mentioned earlier, Dimer doesn't rely on subfolders at all. However, you can group docs for a single category inside a subfolder to manage them easily.

The same formula of prefixing can also be applied to subfolders to manage the order of category headings. Let's see an example.

```
├── 01-tutorial
│   ├── 01-dimer-for-mac.md
│   ├── 02-dimer-for-linux.md
│   ├── 03-dimer-for-windows.md
│   └── 04-getting-started.md
└── 02-customizations
    ├── 01-customizing-sidebar.md
    └── 02-customizing-header.md
```

This will appear as follows in the sidebar.

![](http://res.cloudinary.com/adonisjs/image/upload/q_100/v1525180634/dimer-category-tree_zjbvrz.png)
