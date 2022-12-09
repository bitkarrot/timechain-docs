---
title: Markdown Syntax
description: Examples of how to use Markdown
publishedAt: 12-08-2022
updatedAt: 12-08-2022
tags: [Markdown]
layout: ../../layouts/MainLayout.astro

---

This document is a demo for those new to Markdown. 

If you are unfamiliar with Markdown, you can also visit the [Getting Started
guide in Markdown](https://www.markdownguide.org/getting-started/) to learn
more. 

To view the original markdown file, visit the `Edit this page` link in the 
right hand navigation under the `More` section.


## Paragraphs

Lorem ipsum dolor sit amet, consectetur adipiscing elit 🤣, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Id donec ultrices tincidunt arcu non sodales neque sodales. Adipiscing diam donec adipiscing tristique risus nec feugiat in.

## Line Break

> auto line break by [`remark-breaks`](https://github.com/remarkjs/remark-breaks 'remarkjs/remark-breaks')

Lorem ipsum dolor sit amet,
consectetur adipiscing elit 🤣,
sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Id donec ultrices tincidunt arcu non sodales neque sodales.
Adipiscing diam donec adipiscing tristique risus nec feugiat in.

## Emphasis

### Bold

Love **is** bold

### Italic

A _cat_ meow

### Bold and Italic

This is really **_very_** important text.

## Blockquotes

> Blockquotes can also be nested...
>
> > ...by using additional greater-than signs right next to each other...
> >
> > > ...or with spaces between arrows.

## Lists

### Unordered

- Create a list by starting a line with `+`, `-`, or `*`
- Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    - Ac tristique libero volutpat at
    * Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
- Very easy!

### Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa

Start numbering with offset:

57. foo
1. bar

## Code

> Syntax highlighting by [`Rehype Pretty Code`](https://rehype-pretty-code.netlify.app/ "Rehype Pretty Code's documentation")

<Callout type='warning'>Inline syntax highlighting is unstable in development mode.</Callout>

### Inline Code

This is an array `[1, 2, 3]` of numbers 1 through 3.

### Code Block

```
Sample text here...
```

```bash title="Terminal"
pnpm build
```

```jsx title="Counter.tsx" showLineNumbers {4}
import { createSignal } from 'solid-js'

export default function Counter() {
  const [count, setCount] = createSignal(0)

  const add = () => setCount((i) => i + 1)

  return (
    <div class='flex gap-x-4'>
      <button type='button' onClick={add}>
        the count is {count()}
      </button>
    </div>
  )
}
```

## Horizontal Rules

---

## Link

[YouTube](https://youtube.com)

[Google]

[google]: https://google.com

### Adding Titles

[YouTube](https://youtube.com 'Go to YouTube')

## Image

> Image compress by [`@astrojs/image`](https://docs.astro.build/en/guides/integrations-guide/image/ "@astrojs/image's guide")

**Below we embed a Local image**

![a cat called Lulu](../../../public/images/lulu.jpg)

**and this is a Remote image from https://i.pinimg.com**

![a cat called Lulu](https://i.pinimg.com/originals/f3/43/73/f343733b4bcb341c2faecfb62fe1d9ca.jpg)

## Escaping Characters

\* Without the backslash, this would be a bullet in an unordered list.


## rehype-twemoji

😀 😃 😄 😁 😆 😅 😂 🤣 🥲 🥹 ☺️ 😊 😇 🙂 🙃 😉 😌 😍 🥰 😘 😗 😙 😚 😋 😛 😝 😜 🤪 🤨 🧐 🤓 😎 🥸 🤩 🥳 😏 😒 😞 😔 😟 😕 🙁 ☹️ 😣 😖 😫 😩 🥺 😢 😭 😮‍💨 😤 😠 😡 🤬 🤯 😳 🥵 🥶 😱 😨 😰 😥 😓 🫣 🤗 🫡 🤔 🫢 🤭 🤫 🤥 😶 😶‍🌫️ 😐 😑 😬 🫠 🙄 😯 😦 😧 😮 😲 🥱 😴 🤤 😪 😵 😵‍💫 🫥 🤐 🥴 🤢 🤮 🤧 😷 🤒 🤕 🤑 🤠 😈 👿 👹 👺 🤡 💩 👻 💀 ☠️ 👽 👾 🤖 🎃 😺 😸 😹 😻 😼 😽 🙀 😿 😾
