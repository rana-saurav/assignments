In the **Flexbox layout model**, the following properties are used to control the positioning, alignment, and behavior of items within a flex container. Each property plays a specific role in how flex items are arranged and how they interact with the container's size.

### 1. **`justify-content`**
**Role**: Defines the alignment of items along the **main axis** (horizontal axis by default, or vertical if `flex-direction` is set to `column`).

- **Purpose**: It helps distribute space between and around items in the flex container.
- **Common Values**:
  - **`flex-start`**: Aligns items at the start of the container (default).
  - **`flex-end`**: Aligns items at the end of the container.
  - **`center`**: Centers items in the container.
  - **`space-between`**: Distributes items evenly, with the first item at the start and the last item at the end.
  - **`space-around`**: Distributes items evenly with equal space around each item.
  - **`space-evenly`**: Distributes items evenly with equal space between them.

**Example**:
```css
.container {
  display: flex;
  justify-content: space-between; /* Items will be spaced evenly, with no space at the ends */
}
```

### 2. **`align-items`**
**Role**: Aligns items along the **cross axis** (perpendicular to the main axis, so vertically by default, or horizontally if `flex-direction` is set to `column`).

- **Purpose**: Controls the vertical alignment of items in a flex container (or horizontal alignment when using `flex-direction: column`).
- **Common Values**:
  - **`flex-start`**: Aligns items at the start of the cross axis.
  - **`flex-end`**: Aligns items at the end of the cross axis.
  - **`center`**: Centers items along the cross axis.
  - **`stretch`**: Stretches items to fill the container's height (default).
  - **`baseline`**: Aligns items such that their baselines align.

**Example**:
```css
.container {
  display: flex;
  align-items: center; /* Items will be centered vertically (in a row layout) */
}
```

### 3. **`gap`**
**Role**: Defines the space between **flex items** in the container.

- **Purpose**: Controls the gap between the flex items, whether they are laid out in a row or column. It’s a shorthand for `row-gap` and `column-gap` (which were previously used to specify space between rows and columns separately).
- **Common Values**:
  - A numeric value (`px`, `em`, `rem`, etc.) sets the spacing between items.
  
**Example**:
```css
.container {
  display: flex;
  gap: 10px; /* 10px space between items */
}
```

### 4. **`flex-direction`**
**Role**: Defines the **direction** of the main axis and the direction in which flex items are placed inside the container.

- **Purpose**: It controls whether items are placed in a row or column (or reversed versions of those).
- **Common Values**:
  - **`row`**: Default. Items are placed in a horizontal row (left to right in left-to-right languages).
  - **`row-reverse`**: Items are placed in a horizontal row but in reverse order (right to left).
  - **`column`**: Items are placed in a vertical column (top to bottom).
  - **`column-reverse`**: Items are placed in a vertical column but in reverse order (bottom to top).

**Example**:
```css
.container {
  display: flex;
  flex-direction: column; /* Items will be placed in a vertical column */
}
```

### 5. **`flex-wrap`**
**Role**: Controls whether **flex items** should wrap onto multiple lines if they don’t fit in one row or column.

- **Purpose**: By default, flex items are placed in a single line. `flex-wrap` allows the items to break into multiple lines when necessary.
- **Common Values**:
  - **`nowrap`**: Items will not wrap. This is the default.
  - **`wrap`**: Items will wrap onto multiple lines if they exceed the container’s size.
  - **`wrap-reverse`**: Items will wrap, but in reverse order (bottom to top in a column layout, right to left in a row layout).

**Example**:
```css
.container {
  display: flex;
  flex-wrap: wrap; /* Items will wrap into new lines if they overflow */
}
```

---



```html
<div class="flex-container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <div class="item">Item 4</div>
  <div class="item">Item 5</div>
</div>

<style>
  .flex-container {
    display: flex;
    flex-direction: row; 
    /* Arrange items horizontally */
    flex-wrap: wrap; 
    justify-content: space-between; /* Distribute items with space between them */
    align-items: center; /* Vertically center the items */
    gap: 10px; 
    /* 10px space between items */
    background-color: lightgray;
    padding: 20px;
  }

  .item {
    background-color: lightcoral;
    padding: 20px;
    width: 100px;
    text-align: center;
  }
</style>
```

