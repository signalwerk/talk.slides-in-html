---
theme: signalwerk
title: Building Slides
---

```fm
style: negative
background: true
```

## Hello _👋_

# Building **Slides**

_Libre Graphics Meeting_

<footer>

2026 · Zurich · Stefan Huber

</footer>

--s--

## Pros

# Why in HTML?

- Text-based format (Markdown, HTML)
- Version control with Git
- Easy to include media (images, videos, iframes)

--s--

## Frameworks

# HTML-based presentations

- [Reveal.js](https://revealjs.com/)
- [Spectacle](https://formidable.com/open-source/spectacle/)
- [Impress.js](https://impress.js.org/)
- [Deck.js](http://imakewebthings.com/deck.js/)
- [Shower](https://shwr.me/)


--s--

```fm
style: negative
background: true
```

## Longevity

# _My_ understanding of a presentation framework that _long-term evolves_ with me

--s--

```fm
style: negative
background: true
```

## My Slides

# _Learnings_ from the last 5 years

--s--

## Basic Setup

# Keep it simple, stupid

```
slides/
  ├── index.html
  ├── slides.md
  └── assets/
```

--s--

## index.html

<div style="font-size: .7rem;">

```html
<html lang="en">
  <head>
    …
    <!-- styles -->
    <link
      rel="stylesheet"
      href="https://rawcdn.githack.com/signalwerk/slides/23bc5c4/base.css"
    />
  </head>
  <body>
    <!-- slides -->
    <signalwerk-slides href="slides.md"></signalwerk-slides>
    <!-- logic -->
    <script
      src="https://rawcdn.githack.com/signalwerk/slides/23bc5c4/index.js"
      async
    ></script>
  </body>
</html>
```

</div>

--s--

## slides.md

<div style="font-size: .8rem;">

```markdown
## Little Title

# Big Title

- content
- content
- content

––s––

## Little Title

# Big Title

- content
- content
- content
```

</div>

--s--



## slides.md · Frontmatter

<div style="font-size: .8rem;">

````markdown
```fm
style: negative
background: true
```

## Little Title

# Big Title

- content
- content
- content

––s––
...
````

</div>

--s--

## Slide Title _emphasis_ and **strong**

# Slide Title _emphasis_ and **strong**

### H3 Subtitle

- Text [Link](https://github.com)
- Text _emphasis_ and **strong**

<footer>

Footer: Text [Link](https://github.com) with _emphasis_ and **strong**

</footer>

--s--

```fm
style: negative
background: true
```

## Slide Title _emphasis_ and **strong**

# Slide Title _emphasis_ and **strong**

### H3 Subtitle

- Text [Link](https://github.com)
- Text _emphasis_ and **strong**

<footer>

Footer: Text [Link](https://github.com) with _emphasis_ and **strong**

</footer>

--s--

## Backgrounds

<div style="font-size: .8rem;">

````markdown
```fm
style: image
background:
  iframe: https://signalwerk.github.io/visual.spiral-3d.typo/
```
````

</div>

--s--

```fm
style: image
background:
  iframe: https://signalwerk.github.io/visual.spiral-3d.typo/
```

## iFrame as background

--s--

## Backgrounds

<div style="font-size: .7rem;">

````markdown
```fm
style: image
background:
  image: https://portrait.signalwerk.ch/illustration/2020/rgb/w4000/stefan-huber.jpg
  position: 50% 40%
```
````

</div>

--s--

```fm
style: image
background:
  image: https://portrait.signalwerk.ch/illustration/2020/rgb/w4000/stefan-huber.jpg
  position: 50% 40%
```

## Stefan

<div class="box box--w40p box--bottom box--white box--padding small">

- Developer
- ❦ Typography

</div>

<footer class="footer--right">

Illustration by [Benjamin Güdel](http://www.guedel.biz/) · 2020

</footer>

--s--

## Code syntax highlighting

```html
<html lang="en">
  <head>
    <title>title</title>
  </head>
  <body>
    <!-- page content -->
  </body>
</html>
```

--s--

## Custom syntax highlighting

```fea
# Ligature formation
feature liga {
    substitute f i by f_i;
    substitute f l by f_l;
} liga;
```

Including `fea` support for OpenType feature code.

--s--

## Print

# Everyone wants pdf, right?

--s--

## Print

```css
@media print {
  /* All your print styles go here */
  .noPrint {
    display: none !important;
  }
}
```

--s--

```fm
style: negative
background: true
```

## Custom elements in HTML

# Make it _extendable_

--s--

## Modules

<div style="font-size: .65rem;">

```html
<body>
  <!-- slides -->
  <signalwerk-slides href="slides.md"></signalwerk-slides>
  <!-- logic -->
  <script
    src="https://rawcdn.githack.com/signalwerk/slides/23bc5c4/index.js"
    async
  ></script>
  <!-- modules -->
  <script
    src="https://rawcdn.githack.com/signalwerk/slides/23bc5c4/modules/timer.js"
    async
  ></script>
</body>
```

</div>

--s--

## Modules

# Slides

```html
<signalwerk-slides href="slides.md"></signalwerk-slides>
```

--s--

## Modules

# Timer

```md
<timer-countdown time="00:01:00"></timer-countdown>
```

<div style="position: absolute; top: 0; right: 0;">
<timer-countdown time="00:01:00"></timer-countdown>
</div>

--s--

## Modules 

# Random Selection


<random-selection data-set="oblique-strategies"></random-selection>

<footer>

1975 – Oblique Strategies – Brian Eno und Peter Schmidt

</footer>

--s--

## Modules

# Speaker Video


<speaker-video></speaker-video>

--s--

### QR Code

<br>
<br>

<div class="box--w40p">
<qr-code data="https://libregraphicsmeeting.org/"></qr-code>
</div>

```html
<qr-code data="https://libregraphicsmeeting.org/"></qr-code>
```

--s--

```fm
style: negative
background: true
```

## Longevity

# It's great *to do things* <br>on my own and have them **evolve as I do.**

--s--

```fm
style: negative
background: true
```

## exit 0; thx

# _Questions?_

<style>
  .contact-links {
    padding-bottom: 1rem;
    font-size: .8rem;
  }
  .contact-links a {
    color: white;
  }
  .contact-links a:after {
    display: none;
  }
</style>

<footer class="contact-links">

**Stefan Huber** · sh@signalwerk.ch  
[mastodon.social/@signalwerk](https://mastodon.social/@signalwerk)  
[instagram.com/signalwerk](https://instagram.com/signalwerk)  
[linkedin.com/in/signalwerk](https://linkedin.com/in/signalwerk)  
[github.com/signalwerk](https://github.com/signalwerk)

</footer>
