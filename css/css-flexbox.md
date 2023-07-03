# CSS Flex

(Row) Justify-content = <------->
(Row) Align-items = vertical

- In flex: column these are reversed
- When the flex direction is a column, justify consttent changes to vertical and align-items to the horizontal

```bash
$ .element {
	display: flex;
	flex direction: row / column;
	flex-wrap:
	flex-flex: (flex direction, flex, wrap)
	Place-enter: (align content+justify-content)
}
```

- align-consttent: determines the spacing between lines
  Note: since Align-content is vertical if there is only one line it has no effect

- align-items: determines how the items as a whole are aligned within the container
