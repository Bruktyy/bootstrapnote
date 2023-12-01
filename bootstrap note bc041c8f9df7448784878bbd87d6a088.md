# bootstrap note

# **Creating Responsive Fixed-width Containers**

You can simply use the `.container` class to create a responsive, fixed-width container. The width of the container will change at different breakpoints or screen sizes, as shown above.

```markup
<div class="container"><h1>This is a heading</h1><p>This is a paragraph of text.</p></div>
```

## **Responsive containers**

Responsive containers allow you to specify a class that is 100% wide until the specified breakpoint is reached, after which we apply `max-width`s for each of the higher breakpoints. For example, `.container-sm` is 100% wide to start until the `sm` breakpoint is reached, where it will scale up with `md`, `lg`, `xl`, and `xxl`.

`<div class="container-sm">100% wide until small breakpoint</div>
<div class="container-md">100% wide until medium breakpoint</div>
<div class="container-lg">100% wide until large breakpoint</div>
<div class="container-xl">100% wide until extra large breakpoint</div>
<div class="container-xxl">100% wide until extra extra large breakpoint</div>`

# Bootstrap

Bootstrap is a popular open-source front-end framework that helps developers build responsive and visually appealing websites and web applications. It provides a collection of pre-designed HTML, CSS, and JavaScript components and utilities that can be easily customized and integrated into projects.

Bootstrap compiled files include :

- Compiled and minified CSS bundles. it is a Sass file which provides additional features such as variables, nesting, mixing, and functions, which make it easier to write and maintain CSS code. It allows for reusable styles, easier management of color schemes and typography, and more flexible and modular stylesheets.
- Compiled and minified JavaScript plugins

Break points in bootstrap are the following:

| Breakpoint | Class infix | Dimensions |
| --- | --- | --- |
| Extra small | None | <576px |
| Small | sm | ≥576px |
| Medium | md | ≥768px |
| Large | lg | ≥992px |
| Extra large | xl | ≥1200px |
| Extra extra large | xxl | ≥1400px |

containers are used to create a consistent and centered layout for the content of a web page. They provide a way to control the width and responsiveness of the page content within a fixed or fluid container.

There are two types of containers in Bootstrap: **`.container`** and **`.container-fluid`**.

1. **`.container`**: This class creates a fixed-width container that adapts its width based on the viewport size. The content inside a **`.container`** is centered horizontally on the page. It has predefined maximum widths for different breakpoints, ensuring that the layout remains responsive.
2. **`.container-fluid`**: This class creates a full-width container that spans the entire width of the viewport. The content inside a **`.container-fluid`** extends to the edges of the screen. It adjusts its width dynamically as the viewport size changes.
3. *` .container-{breakpoint}, which is width: 100% until the specified breakpoint. Break points are the break point of the above

## Bootstrap grid

the bootstrap grid divide our container in to 12 equal columns And we can use the prefixes of the above containers to make our columns more responsive on different screen and sizes. we use all types of container for grid parent and then use .col classes to make divide the container in to needed sizes. we can also use prefixes of the container to make it responsive

### Columns

1. **`col`**: This is a generic column class that can be used for creating equal-width columns.
2. **`col-{breakpoint}-{number}`**: This class is used to create columns of specific width based on the specified breakpoint. For example, **`col-sm-4`** creates a column that occupies 4 units of the grid on small screens and above.
3. **`col-{breakpoint}-auto`**: This class creates a column that automatically adjusts its width based on the content within it.
4. **`col-{breakpoint}-offset-{number}`**: This class is used to offset columns horizontally by the specified number of units at the specified breakpoint.

### Gutters

are used to give space between grid columns horizontally and vertically

`.gx-*` classes can be used to control the horizontal gutter widths.

`.gy-*` classes can be used to control the vertical gutter widths within a row when columns wrap to new lines

## Bootstrap Components

Bootstrap provides a rich collection of pre-designed components that you can readily use to build various elements and features for your web pages. These components are designed to be responsive, customizable, and consistent in their appearance. Here are some commonly used Bootstrap components:

1. Navbar: A responsive navigation bar that can be easily customized and includes support for dropdown menus, buttons, forms, and more.
2. Buttons: A variety of button styles, including primary, secondary, success, warning, danger, and more, with options for different sizes and states.
3. Cards: Flexible and versatile content containers that can display various types of information, such as images, text, buttons, and more. Cards can be organized into responsive grids.
4. Forms: Pre-styled form elements such as input fields, checkboxes, radio buttons, select dropdowns, and more, along with support for form validation and customization.
5. Modals: Overlay windows that can be used to display additional content or prompts to the user. Modals can be easily customized and include support for animations and event handling.
6. Carousel: A slideshow component that allows you to showcase a series of images or content in an interactive and visually appealing manner.
7. Alerts: Dismissible alert messages that can be used to communicate important information, success messages, warnings, or errors to the user.
8. Tabs and Pills: Tabs and pills navigation components that allow you to organize content into separate sections or categories.
9. Accordion/Collapse: Collapsible content sections that allow you to present information in an expandable and collapsible manner, conserving space on the page.

## Bootstrap helper class

1. Text Alignment:
    - **`.text-left`**: Aligns text to the left.
    - **`.text-center`**: Centers text horizontally.
    - **`.text-right`**: Aligns text to the right.
    - **`.text-justify`**: Justifies text with consistent spacing.
2. Display and Visibility:
    - **`.d-none`**: Hides an element.
    - **`.d-block`**: Makes an element a block-level element.
    - **`.d-inline`**: Makes an element an inline-level element.
    - **`.d-inline-block`**: Makes an element an inline-block level element.
    - **`.invisible`**: Hides an element but preserves its layout.
3. Spacing and Margin:
    - **`.m-{size}`**: Adds margin to all sides of an element (e.g., **`.m-2`** adds margin of 0.5rem).
    - **`.mt-{size}`**: Adds margin to the top of an element.
    - **`.mr-{size}`**: Adds margin to the right of an element.
    - **`.mb-{size}`**: Adds margin to the bottom of an element.
    - **`.ml-{size}`**: Adds margin to the left of an element.
4. Padding:
    - **`.p-{size}`**: Adds padding to all sides of an element.
    - **`.pt-{size}`**: Adds padding to the top of an element.
    - **`.pr-{size}`**: Adds padding to the right of an element.
    - **`.pb-{size}`**: Adds padding to the bottom of an element.
    - **`.pl-{size}`**: Adds padding to the left of an element.
5. Text Formatting:
    - **`.text-uppercase`**: Converts text to uppercase.
    - **`.text-lowercase`**: Converts text to lowercase.
    - **`.text-capitalize`**: Capitalizes the first letter of each word in text.
6. Background Colors:
    - **`.bg-{color}`**: Adds a background color to an element (e.g., **`.bg-primary`** adds the primary color background).
7. Border:
    - **`.border`**: Adds a border to an element.
    - **`.rounded`**: Applies rounded corners to an element.
    - **`.border-{side}`**: Adds a border to a specific side of an element (e.g., **`.border-top`** adds a border to the top side).