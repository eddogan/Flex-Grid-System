# Flex-Grid-System
  1. [HTML](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#html5-markup)
  2. [CSS](https://github.com/eddogan/Flex-Grid-System/blob/master/README.md#css3-classes)  

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
Start with a `c-` and then the percentage of the column. All column layouts are utilizing an `inline-flex` display property in order to be able to arrange the content within the column and also to directly use columns within columns. 
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
### Alignment classes
```
// SECTION + COLUMN 
.jc_center     {justify-content: center;}
.ai_center     {align-items: center;}
.jc_start      {justify-content: flex-start;}
.ai_start      {align-items: flex-start;}
.jc_end        {justify-content: flex-end;}
.ai_end        {align-items: flex-end;}
.jc_between    {justify-content: space-between;}
.ai_between    {align-items: space-between;}
.jc_around    {justify-content: space-around;}
.ai_around    {align-items: space-around;}
```
### Margin and padding classes
Adjusts the top and bottom margins and paddings. Adding padding or margin to the sides of the elements should be avoided in order to keep consistency throughout the site.
```
// SECTION + COLUMN + INNER COLUMN 
.margin        {margin-top: 8vh; margin-bottom: 8vh;}
.topmargin     {margin-top: 8vh;}
.bottommargin  {margin-bottom: 8vh;}
.padding       {padding-top: 8vh; padding-bottom: 8vh;}
.toppadding    {padding-top: 8vh;}
.bottompadding {padding-bottom: 8vh;}
```

