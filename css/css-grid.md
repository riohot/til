# CSS Grid

- CSS Grid is a new way for layout out information such as tables.
- Modern way to display series of information
- Likely that flex will be used more often

- LESSON 1
- DISPLAY: GRID ETC ETC GOES ON CONTAINER DIV
- STYLING: GOES ON COLLECTIVE ITEM DIVS

- GRID TEMPLATES SET THE GRID LINES
  -- You can actually turn these on in FF inspect mode

```bash
 --- --- ---
|   |   |   |
 --- --- ---
|   |   |   |
 --- --- ---
|   |   |   |
 --- --- ---
```

🖼 Think in terms of containers.

- Where all the container dimensions need to be specified. (if grid<items you'll have overlap)
- You can dynamically move items around the grid

```bash
.element {
	display: grid
	grid-template: col / row
}
```

_grid_

- Most sites usually set the grid contents seperately

```bash
  grid-template-row: You can set any combination of (Em, %px, Nfr) or repreat(N(quant), dimention)
  grid-template-column: ibid.
```

_dimensions_

Height: usually not always set for entire page but for individual divs
Width: Main container/site = 100%, div contents often have side margin

```bash

```

_content placing_

- Grid area moved the consttent of the grid with resepact to the grid lines
- Remember lines start at 0

```bash
	Grid-row-start: x/y
	Grid-column-end: x/y or x / span x
	Grid-area: (grs/gcs/gre/cre)
```

Grid area is to place the container within a set number of grid blocks
