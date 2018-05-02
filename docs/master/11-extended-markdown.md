---
permalink: extended-markdown
category: root
---

# Extended markdown
The beauity of markdown is that it's readable to human eyes, but that also becomes a short-coming, since we cannot define rich content in Markdown. Dimer tries to find the best of both worlds using macros.

Macros are as readable as markdown, but extends the markdown so that we can embed **videos**, **codepen pens** or even define **notification blocks**.

## note
The `note` macro displays a blue color note, as shown below.

```md
[note]
Hello this is a note
[/note]
```

##### Output

[note]
Hello this is a note
[/note]

## tip and warning
The `tip` macro uses the green color and `warning` uses the yellow color.

```md
[tip]
Every second box contains a magic stick
[/tip]

[warn]
Fire in the hole
[/warn]
```

##### Output

[tip]
Every second box contains a magic stick
[/tip]

[warn]
Fire in the hole
[/warn]

## youtube
Also you can embed a youtube video using the `youtube` macro.

```md
[youtube url="https://youtu.be/dWO9uP_VJV8"]
```

## codepen
Codepen pens can be embedded using the pen URL.

```md
[codepen url="https://codepen.io/ge1doot/pen/vRJyVG"]
```

##### Output
[codepen url="https://codepen.io/ge1doot/pen/vRJyVG"]
