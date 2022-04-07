### Content-Based Styles with&nbsp;`:has()`

Style elements based on elements they contain

```css
.card {
  /* layout, without image */
}

.card:has(.card__image) {
  /* layout, with image */
}
```
