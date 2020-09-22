# Sibling fade

Fades out the siblings of a hovered item.

## HTML

```
<div class="sibling-fade">
  <span>Item 1</span> <span>Item 2</span> <span>Item 3</span> <span>Item 4</span>
  <span>Item 5</span> <span>Item 6</span>
</div>
```

## CSS

```
span {
  padding: 0 1rem;
  transition: opacity 0.2s;
}

.sibling-fade:hover span:not(:hover) {
  opacity: 0.5;
}
```

## Demo

[URL](https://codepen.io/pen?&editable=true&editors=111)

```
<iframe class="sok-MarkdownCodepenPrefill-snippetPreviewRenderer" title="30 Seconds of Knowledge - Demo" sandbox="allow-scripts" allowfullscreen="" srcdoc="
			<html>
				<head>
					<style>span {
  padding: 0 1rem;
  transition: opacity 0.2s;
}

.sibling-fade:hover span:not(:hover) {
  opacity: 0.5;
}
</style>
				</head>
				<body>
					<div class=&quot;sibling-fade&quot;>
  <span>Item 1</span> <span>Item 2</span> <span>Item 3</span> <span>Item 4</span>
  <span>Item 5</span> <span>Item 6</span>
</div>

				</body>
			</html>
		"></iframe>
```

## Explanation
    - 1 - transition: opacity 0.2s specifies that changes to opacity will be transitioned over 0.2 seconds.
    - 2 - .sibling-fade:hover span:not(:hover) specifies that when the parent is hovered, select any span children that are not currently being hovered and change their opacity to 0.5.
