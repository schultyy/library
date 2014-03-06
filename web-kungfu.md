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
