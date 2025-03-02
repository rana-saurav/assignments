When you create a grid container with display: grid; and you don't explicitly define the size of certain rows or columns (using grid-template-rows or grid-template-columns), CSS will automatically create additional rows or columns. The grid-auto-rows and grid-auto-columns properties help define the size of those automatically generated rows or columns.

```html
<div class="grid-container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
  <div class="item">4</div>
  <div class="item">5</div>
</div>

```
```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* Defines two columns */
  grid-template-rows: 100px 100px; /* Defines two rows */
  grid-auto-rows: 150px; /* Any additional rows will be 150px tall */
  grid-auto-columns: 200px; /* Any additional columns will be 200px wide */
  gap: 10px; /* Adds some space between items */
}

.item {
  background-color: lightblue;
  padding: 20px;
  text-align: center;
  border: 1px solid black;
}

```