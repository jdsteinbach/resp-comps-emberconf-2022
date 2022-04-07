#### Ember Modifier Workaround

```js
export default modifier((element, queries) => {
  const ro = new ResizeObserver(entries => {
    // use `queries` to manage classes/sizes
  });
  ro.observe(element);
  return () => ro.disconnect();
});
```
<br>

```html
{% raw %}
<div {{cq this.queries}}></div>
{% endraw %}
```
