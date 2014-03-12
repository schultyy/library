# web kung fu

## Position a div at bottom

In this case `inner` should be positioned below `outer`

```CSS

.outer {
  position: relative;
}

.inner {
  position: absolute;
  bottom: 0 px;
}

```

## Articles

The `article` tag represents an article which must be self contained. It should be possible to show the article without the surrounding page.

This means, it should include i.e. the header:


```HTML
<article>
  <h1>Yadda yadda</h1>
  <p>
    The awesome content here
  </p>
</article>
```

## Absolute positioning

When working with absolute positioning (`position: absolute`), then margin and padding don't have any effect and you can only work with `top`, `bottom`, `left` and `right`.


## Triangles

```CSS
.triangle {
  width: 0px;
  height: 0px;

  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
  border-right: 10px solid white;
}
```

## `background-color` on `div` has no effect

Symptom: Setting the `background-color` on a `div` element has no effect. This occurs, because
it has an height of `1px`.

```HTML
<div style="background-color: white;">
  <div style="float: left"></div>
  <div style="float: right"></div>
</div>
```

The surrounding `div` has a height of 0. To fix this, set a height or `overflow: hidden`.
