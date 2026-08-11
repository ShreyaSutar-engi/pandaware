# Hero media

Drop your hero image or video here (e.g. `hero.jpg`, `hero.mp4`, or an
animated GIF of the hand gripping something).

Then in `docs/index.md`, replace the `.pw-hero__media` placeholder `<div>`
with an `<img>` or `<video>` tag pointing at this file, e.g.:

```html
<img src="assets/hero/hero.jpg" alt="PandaWare prosthetic hand" class="pw-hero__media-img">
```

or for video:

```html
<video class="pw-hero__media-img" autoplay muted loop playsinline>
  <source src="assets/hero/hero.mp4" type="video/mp4">
</video>
```

This file itself (`favicon.svg`) is a placeholder icon — swap it for a real
PandaWare logo whenever you have one, keeping the filename the same (or
update `theme.favicon` in `mkdocs.yml` if you rename it).
