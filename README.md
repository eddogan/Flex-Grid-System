# Flex-Grid-System
  1. [HTML](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#html5-markup)
  2. [CSS](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#css3-classes)
  3. [Breakpoints](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#breakpoints)
  4. [Examples](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#examples)

## HTML5 Markup
Following structure should be followed in all sections in order to provide consistent padding/margin throughout the site.

```
<section class="margin">
    <c-33>
      <c-inner>
        ...
      </c-inner>
    </c-33>
    ...
</section>
```

### Sections
All sections are utilizing the full width of the browser. Narrow layouts should be handled with a container column type such as `c-90` or `c-80`.
```
<section class="margin">
  <c-80>
    <c-33>
      <c-inner>
        ...
      </c-inner>
    </c-33>
    ...
  </c-80>
</section>
```
By default sections have a flex layout that centers the content both vertically and horizontally. Further alignment options can be achieved by adding alignment classes.

All sections have `padding-left: 1.5vw;` and `  padding-right: 1.5vw;` in order to keep the distance between the columns and the right and left side of the page equal. 

### Columns
Start with a `c-` and then the percentage of the column.  
  1. `c-20`
  2. `c-25`
  3. `c-33`
  4. `c-40`
  5. `c-50`
  6. `c-60`
  7. `c-66`
  8. `c-75`
  9. `c-80`
  10. `c-90`
  11. `c-100`

### Inner columns
Provides an equal distance of top, bottom, right and left padding for the inner content of the columns. 

## CSS3 Classes
Following classes can be added to the grid elements
### Section-specific 
```
// SECTION
.vh100         {height: 100vh;}
.overflow      {overflow: visible;}
```
### Column-specific
`.flexed` class can be used with a column element, expecially useful when there's a container column.

```
@mixin flexed {display: flex; flex-wrap: wrap;}
.flexed {@include flexed;}
```

### Margin and padding classes
Adjusts the top and bottom margins and paddings. Adding padding or margin to the sides of the elements should be avoided in order to keep consistency throughout the site. 
```
// SECTION + COLUMN + INNER COLUMN 
.margin {margin-top: $gutter-vertical; margin-bottom: $gutter-vertical;}
.margin-none {margin-top: 0; margin-bottom: 0; margin-left: 0; margin-right: 0;}
.margin-top {margin-top: $gutter-vertical;}
.margin-bottom {margin-bottom: $gutter-vertical;}
.margin-horizontal {margin-left: $gutter-horizontal; margin-right: $gutter-horizontal;}
.padding {padding-top: $gutter-vertical; padding-bottom: $gutter-vertical;}
.padding-none {padding-top: 0; padding-bottom: 0; padding-left: 0; padding-right: 0;}
.padding-top {padding-top: $gutter-vertical;}
.padding-bottom {padding-bottom: $gutter-vertical;}
.padding-horizontal {padding-left: $gutter-horizontal; padding-right: $gutter-horizontal;}
```

## Breakpoints
1366px 
1024px 
768px 
480px 

## Examples
