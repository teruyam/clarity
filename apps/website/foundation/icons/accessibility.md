---
title: Accessibility
---

Icons have different accessibility requirements dependent on the context they are being used in.

### Presentational

Icons by default are presentational only meaning they do not provide any context to screen readers and will be purely cosmetic without additional markup.

<DocDemo toggle="false">

```html
<clr-icon shape="info-circle"></clr-icon>
```

</DocDemo>

### Interactive

When icons are used in buttons or links they should be used in conjunction with descriptive text.

Menu

<DocDemo toggle="false">

```html
<button class="btn"><clr-icon shape="bars"></clr-icon> Menu</button>
```

</DocDemo>

If the icon in an interactive item does not have text then the parent interactive item (typically a button or link) should have an appropriate `aria-label` describing the interaction.

<DocDemo toggle="false">

```html
<button class="btn btn-icon" aria-label="main menu">
  <clr-icon shape="bars"></clr-icon>
</button>
```

</DocDemo>

### Status/Indicator

If an icon is used to show a status/indicator or part of a larger body of text then the icon should have a title attribute so the icon can be properly read by the screen reader.

Usage Warning CPU usage is at 99% use.

<DocDemo toggle="false">

```html
<p>
  <clr-icon shape="exclamation-triangle" title="Usage Warning"></clr-icon>
  CPU usage is at 99% use.
</p>
```

</DocDemo>
