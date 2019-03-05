# Flex-Grid-System
is utilizing custom html5 elements, so your html markup is important! Check out the examples below for proper usage.   

## HTML5 Markup
Each component should start with a `<section>` with a **container** class, followed by a **column type** element and end with an **inner column** element. This structure should be followed in all sections in order to provide consistent padding/margin throughout the site.

```
<section class="container-class">
    <c-33>
      <c-inner>
        ...
      </c-inner>
    </c-33>
</section>
```

## Sections
All sections are utilizing the full width of the browser. Narrower components are handled with the column types. By default, it has a flex layout that centers the content both vertically and horizontally. All sections have `padding-left: 1.5vw;` and `  padding-right: 1.5vw;` in order to keep the distance between the columns and the right and left side of the page equal. 

### Container classes
Following classes can be added to the section in order to achieve the desired design features.
```
.fs            {height: 100vh;}
.narrow        {max-width: 90%; -ms-flex: 0 0 90%; flex: 0 0 90%;}
.margin        {margin: 8vh 0;}
.topmargin     {margin-top: 8vh;}
.bottommargin  {margin-bottom: 8vh;}
.padding       {padding: 8vh 1.5vw;}
.toppadding    {padding-top: 8vh;}
.bottompadding {padding-bottom: 8vh;}
.overflow      {overflow: visible;}
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
     
## Column Types
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
  
