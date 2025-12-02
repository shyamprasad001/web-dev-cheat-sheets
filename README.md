# web-dev-cheat-sheets
# Bootstrap Notes

## Bootstrap Grid System

Bootstrap Grid System provides reusable layout utilities using
containers, rows, and columns. It works on a 12-column layout.

### 1. Container

Holds rows and columns.

``` html
<div class="container"></div>
```

### 2. Row

Wraps all the columns.

``` html
<div class="container">
  <div class="row"></div>
</div>
```

### 3. Column

Placed inside rows. You can specify width from 1 to 12.

``` html
<div class="container">
  <div class="row">
    <div class="col-12">I'm your content!</div>
  </div>
</div>
```

-   col-12 spans the full width.
-   col-\* decides the column size.

### 4. Column Wrapping

If column sizes exceed 12, extra columns wrap to the next line.

## Responsive Breakpoints

Bootstrap provides 5 breakpoints:

  Device        Width     Prefix
  ------------- --------- ---------
  Extra small   \<576px   col-
  Small         ≥576px    col-sm-
  Medium        ≥768px    col-md-
  Large         ≥992px    col-lg-
  Extra large   ≥1200px   col-xl-

Bootstrap follows a mobile-first approach.

Example:

``` html
<div class="col-6"></div>
```

You can combine classes:

``` html
<div class="col-12 col-md-6"></div>
```

## CSS Box Properties

### Margin

Used for spacing around elements.

Variants: - margin-top - margin-right - margin-bottom - margin-left

### Auto Margin

Centers elements.

``` css
.nav-items-center {
  margin: auto;
}
```

Align right:

``` css
.nav-items-right {
  margin-left: auto;
}
```

## Bootstrap Utilities

### 1. Spacing (Margin)

  CSS             Bootstrap
  --------------- -----------
  margin          m-\*
  margin-top      mt-\*
  margin-right    mr-\*
  margin-bottom   mb-\*
  margin-left     ml-\*

Values range from 0 to 5.

Spacing calculation example: - spacer = 16px\
- mb-3 = 16px\
- m-5 = 48px

Special values: - m-auto, ml-auto, mr-auto

### 2. Padding

Same pattern as margin: - p-* - pt-* - pb-\* - etc.

### 3. Background Colors

bg-primary, bg-secondary, bg-success, bg-info, bg-warning, bg-danger,\
bg-dark, bg-light, bg-white

### 4. Width Utilities

  Width   Class
  ------- -------
  25%     w-25
  50%     w-50
  75%     w-75
  100%    w-100

### 5. Shadows

shadow-none, shadow-sm, shadow, shadow-lg

### 6. Flex Order

order-1, order-2, ... order-12\
Responsive: order-md-2, order-lg-3

### 7. Display Utilities

Hide elements: - d-none - d-sm-none - d-md-none

Show elements: - d-block - d-md-inline - d-lg-block

### 8. Position Utilities

-   fixed-top
-   fixed-bottom

## Bootstrap Components

### 1. Navbar

``` html
<nav class="navbar navbar-expand-lg navbar-light bg-light"></nav>
```

Nav items:

``` html
<a class="nav-link active" href="#">Home</a>
```

Linking to sections:

``` html
<a href="#sectionId" class="nav-link">Go</a>

<div id="sectionId"></div>
```

### 2. Modal

``` html
<div class="modal fade" id="exampleModal">
  <div class="modal-dialog">
    <div class="modal-content">
      ...
    </div>
  </div>
</div>
```

## Bootstrap Containers

### 1. Container (fixed width)

  Device   Width
  -------- --------
  XS       100%
  SM       540px
  MD       720px
  LG       960px
  XL       1140px

### 2. Container Fluid

``` html
<div class="container-fluid"></div>
```

## HTML Elements

### Block-level

Start on a new line, take full width.

Examples: div, p, h1

### Inline

Take only required width.

Examples: a, img, button

## Span Element

Inline styling container.

``` html
<p>Food offers <span class="offers">50% OFF</span></p>
```

## CSS Selectors

### Class Selector

``` css
.paragraph { color: blue; }
```

### ID Selector

``` css
#population { color: blue; }
```
