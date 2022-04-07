### Content-Based Styles with&nbsp;Templates

```hbs
{% raw %}
<div class="card{{hasImage ? ' card--image' : ''}}">
  {{#if hasImage}}
    <img class="card__image" src={{image.src}} />
  {{/if}}
</div>
{% endraw %}
```
