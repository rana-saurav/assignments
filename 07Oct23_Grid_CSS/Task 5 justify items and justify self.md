1. justify-items
Scope: Applies to all grid items within a grid container.
Purpose: It aligns all the grid items horizontally (along the inline axis, i.e., left to right).
Usage: This property is used to set the alignment of all grid items within their respective grid cells.
```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center; /* Aligns all items horizontally to the center */
}

.grid-item {
  background-color: lightblue;
  padding: 20px;
}

```
2. justify-self
Scope: Applies to individual grid items.
Purpose: It allows you to align a specific grid item horizontally within its own grid cell, overriding the alignment set by justify-items for that particular item.
Usage: This property is used when you need different horizontal alignment for a single grid item than what is applied globally via justify-items.

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: start; /* Aligns all items horizontally to the start */
}

.grid-item-1 {
  background-color: lightblue;
  padding: 20px;
  justify-self: center; /* Aligns this specific item to the center horizontally */
}
```